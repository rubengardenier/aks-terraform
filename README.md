# aks-terraform

Terraform code for provisioning Azure Kubernetes Service (AKS) with GitOps, CNPG, monitoring, and multi-tenant n8n workloads.

## Phases

| Phase | Directory | Description |
|-------|-----------|-------------|
| 1 | `phase-1-vm/` | Initial VM setup on Azure |
| 2 | `phase-2-modules/` | Reusable Terraform modules for customer infrastructure |
| 3 | `phase-3-aks/` | AKS cluster provisioning with Kubernetes manifests |
| 4 | `phase-4-k8s-infra/` | Kubernetes infrastructure (cert-manager, Traefik, CNPG) |
| 5 | `phase-5-gitops/` | Flux-based GitOps setup |
| 6 | `phase-6-cnpg/` | CloudNativePG database clusters with backups |
| 7 | `phase-7-aks-hardening/` | AKS security hardening |
| 8 | `phase-8-production-n8n/` | Production-ready n8n deployment with network policies |
| 9 | `phase-9-monitoring/` | Monitoring with kube-prometheus-stack and Grafana alerting |
| 10 | `phase-10-onboarding/` | Customer onboarding automation (staging + production) |

## Prerequisites

- [Terraform](https://www.terraform.io/) >= 1.0
- [Azure CLI](https://docs.microsoft.com/en-us/cli/azure/)
- An active Azure subscription
