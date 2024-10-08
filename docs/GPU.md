# GPU

UDS K3d comes with optional base images that provide GPU scheduling in the cluster to allow for GPU-accelerated workloads (e.g., LLMs). Currently, UDS K3d only supports NVIDIA CUDA-capable GPUs, with considerations for supporting for AMD and MLX workloads in the future.

## NVIDIA

### Pre-Requisites

### NVIDIA Drivers

- Ensure that the proper [NVIDIA drivers](https://www.nvidia.com/download/index.aspx) are installed (>=525.60).
- Follow the [driver download](https://www.nvidia.com/download/index.aspx) by identifying your hardware from the provided list.

### NVIDIA Container Toolkit

- [Read the pre-requisites for installation and follow the instructions](https://docs.nvidia.com/datacenter/cloud-native/container-toolkit/latest/install-guide.html#installing-with-apt) to download and install the NVIDIA container toolkit (>=1.14).
- After the successful installation off the toolkit, follow the [toolkit instructions](https://docs.nvidia.com/datacenter/cloud-native/container-toolkit/latest/install-guide.html#configuring-docker) to verify that your default Docker runtime is configured for NVIDIA:

  ```bash
  nvidia-ctk runtime configure --runtime=docker --config=$HOME/.config/docker/daemon.json
  ```

- Verify that `nvidia` is now a runtime available to the Docker daemon to use:

  ```bash
  # the expected output should be similar to: `Runtimes: io.containerd.runc.v2 nvidia runc`
  docker info | grep -i nvidia
  ```

- [Try out a sample CUDA workload](https://docs.nvidia.com/datacenter/cloud-native/container-toolkit/latest/sample-workload.html) to ensure your Docker containers have access to the GPUs after configuration.
- (OPTIONAL) You can configure Docker to use the `nvidia` runtime by default by adding the `--set-as-default` flag during the container toolkit post-installation configuration step by running the following command:

  ```bash
  nvidia-ctk runtime configure --runtime=docker --config=$HOME/.config/docker/daemon.json --set-as-default
  ```

- (OPTIONAL) Verify that the default runtime is changed by running the following command:

  ```bash
  # the expected output should be similar to: `Default Runtime: nvidia`
  docker info | grep "Default Runtime"
  ```

### Usage

#### Local Build

To use the NVIDIA CUDA K3s image when bootstrapping a UDS K3d cluster, execute the following:

```bash
uds run default-cuda
```

#### Remote

To use the NVIDIA CUDA K3s image when bootstrapping a UDS K3d cluster, execute the following:

<!-- x-release-please-start-version -->

```bash
export VERSION=0.9.2
uds zarf package deploy oci://justinthelaw/uds-k3d:${VERSION}-cuda --confirm
```

<!-- x-release-please-end -->

#### Windows (WSL2)

The following additional K3s arg must be provided to the UDS task:

```bash
uds run default-cuda --set K3D_EXTRA_ARGS="--gpus=all"
```

### Tests

This repository includes two CUDA workload tests that can be executed:

```bash
uds run validate-cuda # device info query
uds run validate-cuda --set CUDA_TEST="cuda-vector-add" # vector addition
```

### Troubleshooting

#### NVML Errors or Missing CUDA Dependencies

None of the following should ever error or return `unknown version`:

1. Check if your NVIDIA GPU drivers are installed:

    ```bash
    nvidia-smi
    ```

2. Check the version of your NVIDIA Container Toolkit:

    ```bash
    nvidia-ctk --version
    ```

3. Try looking at your Docker runtime information and make sure the following returns with several lines of information:

    ```bash
    docker info | grep "nvidia"
    ```

4. Try running a CUDA sample test in the cluster: [CUDA Vector Add](https://github.com/NVIDIA/k8s-device-plugin/blob/a6a7ce12d28618d343c251ca0941222d7b8a46d3/README.md?plain=1#L145).

#### Memory Errors or Process Locks

If you are, not deploying a fresh cluster or fresh packages (e.g., a GPU workload is already deployed) or you have a GPU that has other workloads on it (e.g., display), then there may not be enough resources to offload the workloads to the NVIDIA GPU.

1. To see what host-level processes are on your NVIDIA GPU(s) run the following:

    ```bash
    nvidia-smi
    ```

2. To check which pods are scheduled with GPU resources in particular, you can run the following `uds zarf tools yq` command:

    ```bash
    uds zarf tools kubectl get pods \
    --all-namespaces \
    --output=yaml \
    | uds zarf tools yq eval -o=json '
      ["Pod", "Namespace", "Container", "GPU"] as $header |
      [$header] + [
        .items[] |
        .metadata as $metadata |
        .spec.containers[] |
        select(.resources.requests["nvidia.com/gpu"]) |
        [
          $metadata.name,
          $metadata.namespace,
          .name,
          .resources.requests["nvidia.com/gpu"]
        ]
      ]' - \
    | uds zarf tools yq -r '(.[0] | @tsv), (.[1:][] | @tsv)' \
    | column -t -s $'\t'
    ```

When you reinstall or start a new GPU-dependent pod, the previous PID (process) on the GPU may not have been flushed yet.

1. Scale the previous GPU-dependent pod deployment down to 0, as the current `RollingUpdate` strategy for vLLM relies on back-up/secondary GPUs to be available for a graceful turnover
2. Use `nvidia-smi` to check if the process has been flushed upon Pod termination BEFORE you deploy a new GPU-dependent pod, and if not, use `kill -9 <PID>` to manually flush the process
