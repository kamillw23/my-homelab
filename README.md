# My Homelab Configuration

This repository stores the configurations for my personal homelab environment. It uses GitOps principles to manage the desired state of the homelab, primarily leveraging Flux CD for continuous deployment.

## Structure

- `apps/`: Contains Kubernetes manifests and HelmReleases for applications deployed in the homelab.
- `clusters/`: Defines the cluster-specific configurations, including Flux CD installations and their synchronization settings.
  - `homelab/`: Configuration specific to the main homelab Kubernetes cluster.
    - `flux-system/`: Bootstrap manifests for Flux CD, defining its installation and pointing to the Git repository for other configurations.

## Technologies Used

- **Kubernetes**: Container orchestration platform.
- **Flux CD**: GitOps continuous delivery solution for Kubernetes.
- **Helm**: Package manager for Kubernetes, used via HelmReleases with Flux.

## Getting Started

To get started with this homelab configuration, you will need a running Kubernetes cluster. Once you have a cluster, you can bootstrap Flux CD to apply the configurations from this repository.

Further instructions will be provided for specific applications and cluster setup within their respective directories.

## Contributing

Feel free to open issues or pull requests if you have suggestions or improvements for this homelab setup.
