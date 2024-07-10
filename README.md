# Kubernetes Platform Apps GitOps

This repository demonstrates how to set up Renovate for automating updates of Kubernetes platform applications in a GitOps workflow.

## Repository Structure

```
.
├── README.md
├── renovate.json
└── platform/
    ├── ingress-nginx/
    │   ├── kustomization.yaml
    │   └── values.yaml
    └── reloader/
        └── kustomization.yaml
```

## Platform Applications

This repository includes configurations for the following platform applications:

- Ingress-Nginx: Kubernetes ingress controller
- Reloader: Kubernetes controller to watch changes in ConfigMaps and Secrets and do rolling upgrades on Pods

## Renovate Setup

This repository uses Renovate to automate dependency updates. The configuration can be found in `renovate.json`.

## GitOps Workflow

This repository is designed to be used with a GitOps tool like Argo CD. The `platform` directory contains the configurations for different platform applications.

## Getting Started

1. Clone this repository
2. Install the Renovate GitHub App on your repository
3. Configure your GitOps tool (e.g., Argo CD) to sync this repository with your Kubernetes cluster

For more detailed instructions, please refer to the [Setting Up Renovate](#) section in our documentation.
