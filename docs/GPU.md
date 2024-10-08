# GPU

UDS K3d comes with optional base images that provide GPU scheduling in the cluster to allow for GPU-accelerated workloads (e.g., LLMs). Currently, UDS K3d only supports NVIDIA CUDA-capable GPUs, with considerations for supporting for AMD and MLX workloads in the future.

## NVIDIA

To use the NVIDIA CUDA K3s image when bootstrapping a UDS K3d cluster, execute the following:

<!-- x-release-please-start-version -->

`uds zarf package deploy oci://justinthelaw/uds-k3d:0.9.0 --confirm`

<!-- x-release-please-end -->

This package is published via CI, but can be created locally with the following command:

`uds zarf package create --flavor cuda --confirm`

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
