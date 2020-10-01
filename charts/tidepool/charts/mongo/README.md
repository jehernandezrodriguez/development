# mongo

![Version: 0.1.0](https://img.shields.io/badge/Version-0.1.0-informational?style=flat-square) ![AppVersion: 1.0](https://img.shields.io/badge/AppVersion-1.0-informational?style=flat-square)

A Helm chart for Kubernetes

**Homepage:** <https://github.com/tidepool-org/development/charts>

## Values

| Key | Type | Default | Description |
|-----|------|---------|-------------|
| affinity | object | `{}` |  |
| nodeSelector | object | `{}` |  |
| secret.data_.Addresses | string | `""` | plaintext comma-separated list of Mongo `host[:port]` addresses |
| secret.data_.Database | string | `""` | plaintext Mongo database name |
| secret.data_.OptParams | string | `""` | plaintext additional Mongo connection params |
| secret.data_.Password | string | `""` | plaintext Mongo password |
| secret.data_.Scheme | string | `""` | plaintext Mongo DB scheme, either `mongodb` or `mongodb+srv` |
| secret.data_.Tls | string | `""` | plaintext, If true, use SSL on Mongo connection |
| secret.data_.Username | string | `""` | plaintext, If non-empty, Mongo username |
| secret.enabled | bool | `false` | whether to create mongo secret |
| tolerations | list | `[]` |  |