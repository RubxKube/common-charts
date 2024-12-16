# common

![Version: v0.3.12](https://img.shields.io/badge/Version-v0.3.12-informational?style=flat-square) ![AppVersion: 0](https://img.shields.io/badge/AppVersion-0-informational?style=flat-square)

Helm chart for generic app on Kubernetes

**Homepage:** <https://github.com/RubxKube/common-charts>

## Maintainers

| Name | Email | Url |
| ---- | ------ | --- |
| QJOLY | <github@une-pause-cafe.fr> |  |

## Source Code

* <https://github.com/RubxKube/common-charts>

## Requirements

Kubernetes: `>= 1.18`

## Values

| Key | Type | Default | Description |
|-----|------|---------|-------------|
| define | int | `80` |  |
| deployment.args | list | `[]` |  |
| deployment.cpuLimit | string | `nil` |  |
| deployment.cpuRequest | string | `nil` |  |
| deployment.emptyDir | list | `[]` |  |
| deployment.initContainers | list | `[]` |  |
| deployment.memoryLimit | string | `nil` |  |
| deployment.memoryRequest | string | `nil` |  |
| deployment.minReplicas | int | `1` |  |
| deployment.port | int | `80` |  |
| deployment.strategy.type | string | `"Recreate"` |  |
| hpa.avgCpuUtilization | int | `50` |  |
| hpa.enabled | bool | `false` |  |
| hpa.maxReplicas | int | `2` |  |
| hpa.minReplicas | int | `1` |  |
| image.pullPolicy | string | `"Always"` |  |
| image.repository | string | `"nginx"` |  |
| image.repositorySettings.isPrivate | bool | `false` |  |
| image.repositorySettings.secretName | string | `nil` |  |
| image.tag | string | `"latest"` |  |
| ingress.annotations | object | `{}` |  |
| ingress.enabled | bool | `false` |  |
| ingress.extraLabels | object | `{}` |  |
| ingress.hostName | string | `"toto.lan"` |  |
| ingress.ingressClassName | string | `"istio"` |  |
| ingress.tls.enabled | bool | `true` |  |
| ingress.tls.secretName | string | `""` |  |
| livenessProbe | object | `{}` |  |
| livenessProbeEnabled | bool | `false` |  |
| name | string | `"my-app"` |  |
| persistence.enabled | bool | `true` |  |
| persistence.extraVolumes | list | `[]` |  |
| persistence.volumes | list | `[]` |  |
| readinessProbe | object | `{}` |  |
| readinessProbeEnabled | bool | `false` |  |
| service.containerPort | int | `80` |  |
| service.enabled | bool | `true` |  |
| service.extraLabels | object | `{}` |  |
| service.servicePort | int | `80` |  |
| service.type | string | `"ClusterIP"` |  |
| startupProbe | object | `{}` |  |
| startupProbeEnabled | bool | `false` |  |
| tests.classicHttp.enabled | bool | `false` |  |
| tests.curlHostHeader.enabled | bool | `false` |  |
| tests.curlHostHeader.path | string | `""` |  |
| variables.configMap.existingConfigMap | list | `[]` |  |
| variables.nonSecret | object | `{}` |  |
| variables.secret.data | object | `{}` |  |
| variables.secret.existingSecret | list | `[]` |  |
| variables.secret.extraExistingSecrets | list | `[]` |  |

