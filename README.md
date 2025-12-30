# OpenCloud Helm Chart

This is a fork of the archived **OpenCloud Helm Charts** repository for personal use.

## 📑 Table of Contents

- [Prerequisites](#prerequisites)
- [Version Stability Notice](#⚠️-version-stability-notice)
- [Available Charts](#-available-charts)
  - [Production Chart](#production-chart-chartsopencloud)
- [License](#-license)

## Prerequisites

- Kubernetes 1.19+
- Helm 3.2.0+
- PV provisioner support in the underlying infrastructure (if persistence is enabled)
- External ingress controller (e.g., Cilium Gateway API) for routing traffic to the services

## ⚠️ Version Stability Notice

**Important**: These Helm charts are currently at version `0.x.x`, which according to [Semantic Versioning 2.0](https://semver.org/spec/v2.0.0.html#spec-item-4) means:
- The charts are still under heavy development
- Breaking changes may occur at any time
- The public API should not be considered stable
- Use with caution in production environments

We recommend pinning to specific chart versions and thoroughly testing updates before applying them.

## 📦 Available Charts

This repository contains the following charts:

### Production Chart (`charts/opencloud`)

The complete OpenCloud deployment with all components for production use:

- Full microservices architecture
- Keycloak for authentication
- MinIO for object storage
- Document editing with Collabora and/or OnlyOffice
- Full Gateway API integration

[View Production Chart Documentation](./charts/opencloud/README.md)

## 📜 License

This project is licensed under the **AGPLv3** license. See the [LICENSE](LICENSE) file for more details.
