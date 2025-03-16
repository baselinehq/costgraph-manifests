# Grafana on Costgraph
This repository contains the Grafana dashboards that are used in the Costgraph ecosystem.

## Table of Contents
- [Grafana Dashboards](#grafana-dashboards)

## Grafana Dashboards
The Grafana dashboards are used to visualize the data collected by the Prometheus server. The dashboards are used to provide insights into the cost of resources in the cluster.

### Installation
To install the Grafana, you can use the following commands:

```shell
helm repo add grafana https://grafana.github.io/helm-charts
helm repo update
helm install grafana grafana/grafana --namespace monitoring --create-namespace -f values.yaml 
```

This dashboard requires plugins to be installed. You can view those plugins in the [values.yaml](./values.yaml) file.

### Configuration
The Grafana dashboards are configured to use the Prometheus server as the data source.

### Usage
The Grafana dashboards can be accessed by navigating to the Grafana URL. The dashboards are pre-configured to use the Prometheus server as the data source.

You can use the pre-configured dashboards in [dashboard.json](./dashboard.json) to visualize the data collected by the Prometheus server.

### Contributing
If you have a use case you would like to share, please submit a PR to this repository.