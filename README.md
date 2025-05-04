# Typesense-Kubernetes-Operator-Charts
Helm chart repo for [Typesense-Kubernetes-Operator](https://github.com/sai3010/Typesense-Kubernetes-Operator)

## Installation

To install the chart with the release name `my-release`:

```bash
helm repo add typesense-operator https://sai3010.github.io/Typesense-Kubernetes-Operator-Charts/
helm install my-release tko/typesense-kubernetes-operator
```

## Values

The following table lists the configurable parameters of the chart and their default values:

| Parameter                  | Description                                     | Default                |
|----------------------------|-------------------------------------------------|------------------------|
| `image.typesenseImage`         | Operator container image repository            | `sai3010/typesense-operator:3.2`   |
| `nodeSelector`                | Configure nodeselector                | `kubernetes.io/os: linux`               |
| `image.pullPolicy`         | Image pull policy                              | `IfNotPresent`         |
| `resources`                | Resource requests and limits                   | `{}`

For a full list of configurable values, refer to the `values.yaml` file.

## Uninstallation

To uninstall the chart:

```bash
helm uninstall my-release
```

This removes all the Kubernetes components associated with the chart and deletes the release.

## Contributing

Contributions are welcome! Please open an issue or submit a pull request for any changes or improvements.

## License

This project is licensed under the MIT License. See the `LICENSE` file for details.