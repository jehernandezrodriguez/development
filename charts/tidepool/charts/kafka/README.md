# kafka

![Version: 0.1.0](https://img.shields.io/badge/Version-0.1.0-informational?style=flat-square) ![AppVersion: 1.0](https://img.shields.io/badge/AppVersion-1.0-informational?style=flat-square)

A Helm chart for Kubernetes

**Homepage:** <https://github.com/tidepool-org/development/charts>

## Values

| Key | Type | Default | Description |
|-----|------|---------|-------------|
| affinity | object | `{}` |  |
| configmap.Brokers | string | `"kafka-kafka-bootstrap.kafka.svc.cluster.local:9092"` |  |
| configmap.EmailsTopic | string | `"emails"` |  |
| configmap.TopicPrefix | string | `""` |  |
| configmap.enabled | bool | `true` |  |
| nodeSelector | object | `{}` |  |
| tolerations | list | `[]` |  |
