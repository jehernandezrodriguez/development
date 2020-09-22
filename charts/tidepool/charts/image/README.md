# image

![Version: 0.1.0](https://img.shields.io/badge/Version-0.1.0-informational?style=flat-square) ![AppVersion: 1.0](https://img.shields.io/badge/AppVersion-1.0-informational?style=flat-square)

A Helm chart for Kubernetes

**Homepage:** <https://github.com/tidepool-org/development/charts>

## Values

| Key | Type | Default | Description |
|-----|------|---------|-------------|
| affinity | object | `{}` |  |
| deployment.env.store.file.directory | string | `"_data/image"` | directory to use when storing images on file storage |
| deployment.env.store.file.prefix | string | `"images"` | file prefix to use when storing images on file storage |
| deployment.env.store.s3.bucket | string | `"data"` | S3 bucket where image data is written |
| deployment.env.store.s3.prefix | string | `"images"` |  |
| deployment.env.store.type | string | `"file"` | if `s3`, store image data in Amazon S3. If `file` store image data in local file |
| deployment.image | string | `"tidepool/platform-image:master-latest"` | Docker image |
| deployment.replicas | int | `1` |  |
| hpa.enabled | bool | `false` | whether to create a horizontal pod autoscalers for all pods of given deployment |
| hpa.maxReplicas | string | `nil` | maximum number of replicas that HPA will maintain |
| hpa.minReplicas | int | `1` | minimum number of replicas that HPA will maintain |
| iamRole | string | `""` |  |
| mongo.secretName | string | `"mongo"` |  |
| nodeSelector | object | `{}` |  |
| pdb.enabled | bool | `false` |  |
| pdb.minAvailable | string | `"50%"` |  |
| podAnnotations | object | `{}` |  |
| podSecurityContext | object | `{}` |  |
| resources | object | `{}` |  |
| secret.data_.ServiceAuth | string | `""` | plaintext service authorization secret |
| secret.enabled | bool | `false` | whether to create image secret |
| securityContext | object | `{}` |  |
| serviceAccount.create | bool | `false` |  |
| tolerations | list | `[]` |  |
