# userdata

![Version: 0.1.0](https://img.shields.io/badge/Version-0.1.0-informational?style=flat-square) ![AppVersion: 1.0](https://img.shields.io/badge/AppVersion-1.0-informational?style=flat-square)

A Helm chart for Kubernetes

**Homepage:** <https://github.com/tidepool-org/development/charts>

## Values

| Key | Type | Default | Description |
|-----|------|---------|-------------|
| affinity | object | `{}` |  |
| nodeSelector | object | `{}` |  |
| secret.data_.UserIdSalt | string | `""` | plaintext user id salt |
| secret.data_.UserPasswordSalt | string | `""` | plaintext user password salt |
| secret.enabled | bool | `false` | whether to create userdata secret |
| tolerations | list | `[]` |  |
