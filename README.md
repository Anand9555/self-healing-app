# Self-Healing App — GitOps Deployment Template

A Kubernetes/Argo CD-oriented starter repository for exploring GitOps deployment patterns and operational safeguards. This repository is a fork of [devopsbyraham/self-healing-app](https://github.com/devopsbyraham/self-healing-app); please distinguish upstream work from any changes made in this fork.

> **Status:** Learning/portfolio project. Verify the manifests and environment-specific settings before using them. This is not a claim of production readiness.

## Repository layout

- `apps/` — application-related resources
- `argocd/` — Argo CD configuration
- `monitoring/` — monitoring-related configuration
- `network/` — network-related resources
- `docs/` — project documentation

Check each directory's manifests and documentation for the current implementation; this README describes the repository structure, not a guarantee that every component is fully configured.

## Getting started

1. Review the manifests and prerequisites in `docs/` and the relevant directories.
2. Configure your own cluster, namespaces, image references, and credentials. Do not commit credentials or production secrets.
3. Validate manifests with the tooling appropriate to your cluster before applying them.
4. Deploy only in a test environment first, then verify application health, Argo CD sync status, and monitoring behavior.

The exact deployment commands depend on your cluster and configuration, so avoid applying these resources blindly to a production cluster.

## What I’m learning

- Organizing Kubernetes resources for GitOps workflows
- Managing application delivery through Argo CD
- Separating application, networking, and monitoring configuration
- Documenting validation and operational steps

## Attribution

This project is forked from [devopsbyraham/self-healing-app](https://github.com/devopsbyraham/self-healing-app). See the upstream repository for its original implementation. Any original changes in this fork should be documented here as they are made.

## License

Check the upstream license and repository files before reuse or redistribution.
