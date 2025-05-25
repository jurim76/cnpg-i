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

---

## NB! Node should be labeled with "rabbitmq=true" label to match nodeAffinity condition
See `values.test.yaml` for more options

---

### Useful links

https://www.rabbitmq.com/kubernetes/operator/using-operator.html

https://www.rabbitmq.com/kubernetes/operator/troubleshooting-operator.html

https://docs.bitnami.com/kubernetes/infrastructure/rabbitmq-cluster-operator/configuration/

https://github.com/rabbitmq/cluster-operator/tree/main/observability/

https://github.com/rabbitmq/cluster-operator/blob/main/docs/examples/

https://www.rabbitmq.com/java-tools.html

https://github.com/bitnami/charts/tree/main/bitnami/rabbitmq-cluster-operator/

https://github.com/bitnami/containers/tree/main/bitnami/rabbitmq#configuration

---

## Values

| Key | Type | Default | Description |
|-----|------|---------|-------------|
| affinity | object | `{}` |  |
| cert-manager.enabled | bool | `false` | Install cert-manager together. # ref: https://cert-manager.io/docs/installation/kubernetes/#installing-with-helm |
| crds.enabled | bool | `true` |  |
| crds.keep | bool | `true` |  |
| customLabels.owner_team | string | `"ops-dba"` |  |
| image.pullPolicy | string | `"IfNotPresent"` |  |
| image.repository | string | `"ghcr.io/cloudnative-pg/plugin-barman-cloud"` |  |
| image.tag | string | `""` |  |
| imagePullSecrets | list | `[]` |  |
| nodeSelector | object | `{}` |  |
| podAnnotations | object | `{}` |  |
| podLabels.owner_team | string | `"ops-dba"` |  |
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
