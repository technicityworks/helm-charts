# prometheus-kafka-exporter

A Prometheus exporter for [Apache Kafka](https://kafka.apache.org/) metrics.

This chart bootstraps a [Kafka Exporter](https://github.com/danielqsj/kafka_exporter) deployment on a [Kubernetes](http://kubernetes.io) cluster using the [Helm](https://helm.sh) package manager.

## Prerequisites

- Kubernetes 1.8+ with Beta APIs enabled
- Prometheus ServiceMonitor CRD enabled

## Get Repo Info

```sh
helm repo add technicityworks https://technicityworks.github.io/helm-charts
helm repo update
```

_See [helm repo](https://helm.sh/docs/helm/helm_repo/) for command documentation._

## Install Chart

```sh
# Helm 3
helm install [RELEASE_NAME] technicityworks/prometheus-kafka-exporter

# Helm 2
helm install --name [RELEASE_NAME] technicityworks/prometheus-kafka-exporter
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
helm inspect values technicityworks/prometheus-kafka-exporter

# Helm 3
helm show values technicityworks/prometheus-kafka-exporter
```

## Dashboard

Link to dashboard can be found @ [grafana/technicityworks](https://grafana.com/grafana/dashboards/15465)
