# Telemetry-Prometheus

Tool that scrapes metrics (ex: Cpu, memory and disk usage) from the cluster's components

## Usage

[Helm](https://helm.sh) must be installed to use the charts.
Please refer to Helm's [documentation](https://helm.sh/docs/) to get started.

- prometheus · prometheus/prometheus-community (https://artifacthub.io/packages/helm/prometheus-community/prometheus)

Once Helm is set up properly, add the repo as follows:

## Get Repo Info

```console
$ helm repo add prometheus-community https://prometheus-community.github.io/helm-charts
$ helm repo add kube-state-metrics https://kubernetes.github.io/kube-state-metrics
$ helm repo update
```

## Installing the Chart

To install the chart with the release name `prometheus`:

```console
$ helm install prometheus --version <version> prometheus-community/prometheus -f chart/values.yaml
```

## Uninstalling the Chart

To uninstall/delete the prometheus deployment:

```console
$ helm delete prometheus
```

The command removes all the Kubernetes components associated with the chart and deletes the release.
