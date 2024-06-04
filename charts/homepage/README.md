# Homepage

A modern (fully static, fast), secure (fully proxied), highly customizable application dashboard with integrations for more than 25 services and translations for over 15 languages. Easily configured via YAML files (or discovery via docker labels).

[Homepage](https://gethomepage.dev)

## Introduction

This chart bootstraps a [Homepage](https://github.com/gethomepage/homepage) deployment on a [Kubernetes](https://kubernetes.io) cluster using the [Helm](https://helm.sh) package manager and it manage secrets using [Helm Secrets](https://github.com/jkroepke/helm-secrets) plugin.

## Prerequisites

- Kubernetes 1.28+
- Helm 3.14+
- Helm Secrets 4.6.0+

## Installing the Chart

To install the chart with the release name 'my-release':

```bash
helm secrets install my-release homepage -f secrets_enc.yaml
```

The command deploys Homepage on the Kubernetes cluster in the default configuration.

> **Tip**: List all releases using `helm list`

## Test the Chart
After the installation is possible to test the chart using the following command

```bash
helm test homepage
```
## Uninstalling the Chart

To uninstall/delete the `my-release` deployment:

```bash
helm uninstall my-release
```