# another-ldap-auth

![Version: 0.2.0](https://img.shields.io/badge/Version-0.2.0-informational?style=flat-square) ![Type: application](https://img.shields.io/badge/Type-application-informational?style=flat-square) ![AppVersion: 2.0.2](https://img.shields.io/badge/AppVersion-2.0.2-informational?style=flat-square)

A Helm chart using another-ldap-auth to enable AD or LDAP based basic-authentication for ingress resources

**Homepage:** <https://github.com/dignajar/another-ldap-auth>

## Source Code

* <https://github.com/dignajar/another-ldap-auth>

## Values

| Key | Type | Default | Description |
|-----|------|---------|-------------|
| affinity | object | `{}` |  |
| autoscaling.enabled | bool | `false` |  |
| autoscaling.maxReplicas | int | `100` |  |
| autoscaling.minReplicas | int | `1` |  |
| autoscaling.targetCPUUtilizationPercentage | int | `80` |  |
| fullnameOverride | string | `""` |  |
| image.pullPolicy | string | `"IfNotPresent"` |  |
| image.repository | string | `"dignajar/another-ldap-auth"` |  |
| image.tag | string | `"1.9"` |  |
| imagePullSecrets | list | `[]` |  |
| ldap.cacheExpiration | int | `10` |  |
| ldap.endpoint | string | `"ldaps://testmyldap.com:636"` |  |
| ldap.existingSecret | string | `nil` |  |
| ldap.httpsSupport | string | `"enabled"` |  |
| ldap.logLevel | string | `"INFO"` |  |
| ldap.managerDnUsername | string | `"CN=john,OU=Administrators,DC=TESTMYLDAP,DC=COM"` |  |
| ldap.searchBase | string | `"DC=TESTMYLDAP,DC=COM"` |  |
| ldap.searchFilter | string | `"(sAMAccountName={username})"` |  |
| ldap.bindDN | string | `"{username}@TESTMYLDAP.com"` |  |
| nameOverride | string | `""` |  |
| nodeSelector | object | `{}` |  |
| podAnnotations | object | `{}` |  |
| podSecurityContext | object | `{}` |  |
| replicaCount | int | `1` |  |
| resources.limits.cpu | string | `"500m"` |  |
| resources.limits.memory | string | `"256Mi"` |  |
| resources.requests.cpu | string | `"50m"` |  |
| resources.requests.memory | string | `"64Mi"` |  |
| securityContext | object | `{}` |  |
| service.containerPort | int | `9000` |  |
| service.port | int | `80` |  |
| service.protocol | string | `"TCP"` |  |
| service.type | string | `"ClusterIP"` |  |
| serviceAccount.annotations | object | `{}` |  |
| serviceAccount.create | bool | `true` |  |
| serviceAccount.name | string | `""` |  |
| tolerations | list | `[]` |  |

----------------------------------------------
Autogenerated from chart metadata using [helm-docs v1.5.0](https://github.com/norwoodj/helm-docs/releases/v1.5.0)
