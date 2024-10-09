# UDS K3d Environment

> [!IMPORTANT]
> This package should only be used for development and testing purposes. It is not intended for production use and all data is overwritten when the package is re-deployed.

This zarf package serves as a universal dev (local & remote) and test environment for testing [UDS Core](https://github.com/defenseunicorns/uds-core), individual UDS Capabilities, and UDS capabilities aggregated via the [UDS CLI](https://github.com/defenseunicorns/uds-cli). If working with a remote cluster over SSH, you can use SSH port-forwarding to connect:

```console
# Non-standard ports
ssh -N -L 8080:localhost:80 -L 8443:localhost:443 -L 6550:localhost:6550 <your-remote-host>

# Standard ports (requires sudo)
sudo ssh -N -L 80:localhost:80 -L 443:localhost:443 -L 6550:localhost:6550 <your-remote-host>
```

> [!NOTE]
> UDS K3d intentionally does not address airgap concerns for K3d or the load balancer logic deployed in this package. This allows running `zarf init` or deploying a Zarf Init Package via a UDS Bundle after the UDS K3d environment is deployed.

## Pre-Requisites

- [UDS CLI](https://github.com/defenseunicorns/uds-cli/blob/main/README.md#install) & [K3d](https://k3d.io/#installation) using the versions specified in the [uds-common repo](https://github.com/defenseunicorns/uds-common/blob/main/README.md#supported-tool-versions)
- [Docker](https://docs.docker.com/get-docker/) or [Podman](https://podman.io/getting-started/installation) for running K3d
- See the [GPU Configuration](./docs/GPU.md) information for more details on enabling NVIDIA GPU support within the cluster

## Deploy

<!-- x-release-please-start-version -->

`uds zarf package deploy oci://defenseunicorns/uds-k3d:0.11.1`

<!-- x-release-please-end -->

## Create

This package is published via CI, but can be created locally with the following command:

`uds zarf package create`

## Remove

`k3d cluster delete uds` (uds is the default cluster name).

## Start and Stop

To stop and start an existing UDS K3d cluster gracefully, use the following prior to host hibernation, suspension, restart, or shutoff:

```bash
# to stop the default UDS cluster
k3d cluster stop uds

# to start the default UDS cluster
k3d cluster start uds
```

## Additional Info

You can set extra K3d arguments by setting the deploy-time `ZARF_VAR_K3D_EXTRA_ARGS`. See below `zarf-config.yaml` example below for K3d args examples:

```yaml
package:
  deploy:
    set:
      k3d_extra_args: --k3s-arg "--<arg2>=<value>@server:*" --gpus=all
```

### Configure MinIO

- [Configuring Minio](docs/MINIO.md)

### DNS Assumptions

- [DNS Assumptions](docs/DNS.md)

### Enabling GPU Support

- [GPU Workload Configuration](docs/GPU.md)
