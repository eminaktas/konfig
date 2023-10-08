# Konfig

[![Open in GitHub Codespaces](https://github.com/codespaces/badge.svg)](https://github.com/codespaces/new?hide_repo_select=true&ref=main&repo=488867056&machine=standardLinux32gb&devcontainer_path=.devcontainer.json)

[English](README.md) | [Chinese](README-zh.md)

Konfig is the mono repository of the infra configuration in KCL(Kusion Configuration Language).

Konfig provides users with an out-of-the-box, highly abstract configuration interface. The original starting point of the model library is to improve the efficiency and experience of YAML users. We hope to simplify the writing of user-side configuration code by abstracting and encapsulating the model with more complex code into a unified model.

For more details, please refer to: [Model Overview](https://kcl-lang.io/docs/user_docs/guides/working-with-konfig/overview)

## Directory Structure

The overall structure of the configuration library is as follows:

```bash
.
├── LICENSE
├── Makefile
├── README-zh.md
├── README.md
├── examples            # konfig examples
├── kcl.mod             # konfig package metadata file
├── kcl.mod.lock        # konfig package metadata lock file
└── models
    ├── commons         # Common models
    ├── kube            # Cloud-native resource core models
    │   ├── backend         # Back-end models
    │   ├── frontend        # Front-end models
    │   │   ├── common          # Common front-end models
    │   │   ├── configmap       # ConfigMap
    │   │   ├── container       # Container
    │   │   ├── ingress         # Ingress
    │   │   ├── resource        # Resource
    │   │   ├── secret          # Secret
    │   │   ├── service         # Service
    │   │   ├── sidecar         # Sidecar
    │   │   ├── strategy        # strategy
    │   │   ├── volume          # Volume
    │   │   └── server.k        # The `Server` model
    │   ├── metadata        # Kubernetes metadata
    │   ├── mixins          # Mixin
    │   ├── render          # Front-to-back-end renderers.
    │   ├── templates       # Data template
    │   └── utils
    └── metadata           # Common metadata
```

## Prerequisites

Install [kpm](https://kcl-lang.io/docs/user_docs/guides/package-management/installation)

## Quick Start

See [here](https://kcl-lang.io/docs/user_docs/guides/working-with-konfig/guide)

## License

Apache License Version 2.0
