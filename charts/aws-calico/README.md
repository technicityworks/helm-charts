# Calico on AWS

A Helm chart for aws-calico based on [aws-calico](https://github.com/aws/eks-charts/tree/c3452adcb698e5ce865166f41462c74854a27b9d/stable/aws-calico)with updated CRD API version to `v1` instead of `v1beta1`.

## Prerequisites

- Kubernetes 1.8+ with Beta APIs enabled

## Get Repo Info

```sh
helm repo add technicityworks https://technicityworks.github.io/helm-charts
helm repo update
```

_See [helm repo](https://helm.sh/docs/helm/helm_repo/) for command documentation._

## Install Chart

```sh
# Helm 3
helm install [RELEASE_NAME] technicityworks/aws-calico

# Helm 2
helm install --name [RELEASE_NAME] technicityworks/aws-calico
```

_See [configuration](#configuration) below._

_See [helm install](https://helm.sh/docs/helm/helm_install/) for command documentation._

## Uninstall Chart

```sh
# Helm 3
helm uninstall [RELEASE_NAME]

# Helm 2
helm delete --purge [RELEASE_NAME]
```

This removes all the Kubernetes components associated with the chart and deletes the release.

_See [helm uninstall](https://helm.sh/docs/helm/helm_uninstall/) for command documentation._

## Upgrading Chart

```sh
# Helm 3 or 2
helm upgrade [RELEASE_NAME] [CHART] --install
```

_See [helm upgrade](https://helm.sh/docs/helm/helm_upgrade/) for command documentation._

## Configuration

See [Customizing the Chart Before Installing](https://helm.sh/docs/intro/using_helm/#customizing-the-chart-before-installing). To see all configurable options with detailed comments, visit the chart's [values.yaml](./values.yaml), or run these configuration commands:

```sh
# Helm 2
helm inspect values technicityworks/aws-calico

# Helm 3
helm show values technicityworks/aws-calico
```
