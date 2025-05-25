# cnpg-i

![Version: 0.4.0](https://img.shields.io/badge/Version-0.4.0-informational?style=flat-square) ![AppVersion: v0.4.0](https://img.shields.io/badge/AppVersion-v0.4.0-informational?style=flat-square)

Barman Cloud CNPG-I plugin for CloudNativePG

**Homepage:** <https://cloudnative-pg.io/plugin-barman-cloud/>

## Maintainers

| Name | Email | Url |
| ---- | ------ | --- |
| Juri Malinovski |  |  |

## Source Code

* <https://github.com/cloudnative-pg/plugin-barman-cloud>

## Requirements

| Repository | Name | Version |
|------------|------|---------|
| https://charts.jetstack.io | cert-manager | ~1.17.x |

## Values

| Key | Type | Default | Description |
|-----|------|---------|-------------|
| affinity | object | `{}` |  |
| cert-manager.enabled | bool | `false` | Install cert-manager together. # ref: https://cert-manager.io/docs/installation/kubernetes/#installing-with-helm |
| crds.enabled | bool | `true` |  |
| crds.keep | bool | `true` |  |
| customLabels | object | `{}` |  |
| image.pullPolicy | string | `"IfNotPresent"` |  |
| image.repository | string | `"ghcr.io/cloudnative-pg/plugin-barman-cloud"` |  |
| image.tag | string | `""` |  |
| imagePullSecrets | list | `[]` |  |
| nodeSelector | object | `{}` |  |
| podAnnotations | object | `{}` |  |
| podLabels | object | `{}` |  |
| podSecurityContext.allowPrivilegeEscalation | bool | `false` |  |
| podSecurityContext.capabilities.drop[0] | string | `"ALL"` |  |
| podSecurityContext.readOnlyRootFilesystem | bool | `true` |  |
| podSecurityContext.runAsGroup | int | `10001` |  |
| podSecurityContext.runAsUser | int | `10001` |  |
| podSecurityContext.seccompProfile.type | string | `"RuntimeDefault"` |  |
| rbac.create | bool | `true` |  |
| replicaCount | int | `1` |  |
| resources | object | `{}` |  |
| securityContext.runAsNonRoot | bool | `true` |  |
| securityContext.seccompProfile.type | string | `"RuntimeDefault"` |  |
| service.port | int | `9090` |  |
| service.type | string | `"ClusterIP"` |  |
| serviceAccount.annotations | object | `{}` |  |
| serviceAccount.automount | bool | `true` |  |
| serviceAccount.create | bool | `true` |  |
| serviceAccount.name | string | `""` |  |
| strategy.type | string | `"Recreate"` |  |
| tolerations | list | `[]` |  |
