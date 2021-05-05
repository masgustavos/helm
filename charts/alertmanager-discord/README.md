# alertmanager-discord

![Version: 0.0.4](https://img.shields.io/badge/Version-0.0.4-informational?style=flat-square) ![Type: application](https://img.shields.io/badge/Type-application-informational?style=flat-square)

A Helm chart for masgustavos/alertmanager-discord

**Homepage:** <https://github.com/masgustavos/helm/tree/main/charts/alertmanager-discord>

## Maintainers

| Name | Email | Url |
| ---- | ------ | --- |
| Gustavo Stein | gustavosteinmattos@gmail.com | https://github.com/masgustavos |

## Values

| Key | Type | Default | Description |
|-----|------|---------|-------------|
| config | object | `{}` | See https://github.com/masgustavos/alertmanager-discord/blob/master/config.example.yaml |
| configAsSecret | object | `{}` | If you don't want to expose your webhooks, create the config as a secret with the key "config" |
| env | object | `{}` |  |
| fullnameOverride | string | `""` |  |
| hpa.enabled | bool | `false` |  |
| hpa.maxReplicas | int | `3` |  |
| hpa.minReplicas | int | `1` |  |
| hpa.targetCpu | int | `70` |  |
| image | string | `nil` |  |
| imagePullPolicy | string | `"IfNotPresent"` |  |
| imagePullSecrets | list | `[]` |  |
| ingress.annotations | object | `{}` |  |
| ingress.enabled | bool | `false` |  |
| ingress.hosts | list | `[]` |  |
| ingress.paths./ | object | `{}` |  |
| ingress.tls | list | `[]` |  |
| livenessProbe.failureThreshold | int | `3` |  |
| livenessProbe.initialDelaySeconds | int | `15` |  |
| livenessProbe.path | string | `"/"` |  |
| livenessProbe.periodSeconds | int | `30` |  |
| livenessProbe.successThreshold | int | `1` |  |
| livenessProbe.timeoutSeconds | int | `10` |  |
| nameOverride | string | `""` |  |
| nodeAffinity | object | `{}` |  |
| pdb.maxUnavailable | int | `1` |  |
| podAnnotations | object | `{}` |  |
| readinessProbe.failureThreshold | int | `6` |  |
| readinessProbe.initialDelaySeconds | int | `15` |  |
| readinessProbe.path | string | `"/"` |  |
| readinessProbe.periodSeconds | int | `30` |  |
| readinessProbe.successThreshold | int | `1` |  |
| readinessProbe.timeoutSeconds | int | `10` |  |
| replicaCount | int | `1` |  |
| resources | object | `{}` |  |
| rollingUpdate.maxSurge | int | `1` |  |
| service.port | int | `80` |  |
| service.targetPort | int | `8080` |  |
| service.type | string | `"ClusterIP"` |  |
| tolerations | list | `[]` |  |

