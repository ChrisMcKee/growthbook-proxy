
Growthbook-proxy
===========

A Helm chart for deploying growthbook-proxy


## Configuration

The following table lists the configurable parameters of the Growthbook-proxy chart and their default values.

| Parameter                | Description             | Default        |
| ------------------------ | ----------------------- | -------------- |
| `replicaCount` |  | `1` |
| `image.repository` |  | `"growthbook/proxy"` |
| `image.pullPolicy` |  | `"IfNotPresent"` |
| `image.tag` |  | `""` |
| `imagePullSecrets` |  | `[]` |
| `nameOverride` |  | `""` |
| `fullnameOverride` |  | `""` |
| `apiKey` |  | `""` |
| `apiHost` |  | `"https://api.growthbook.io"` |
| `cacheEngine` |  | `"memory"` |
| `cacheConnectionUrl` |  | `""` |
| `cacheStaleTtl` |  | `"60"` |
| `cacheExpiresTtl` |  | `"600"` |
| `enableRemoteEval` |  | `true` |
| `useHttp2` |  | `"false"` |
| `httpsCert` |  | `""` |
| `httpsKey` |  | `""` |
| `maxPayloadSize` |  | `"2mb"` |
| `verboseDebugging` |  | `false` |
| `redisCluster.enabled` |  | `false` |
| `redisCluster.redisRootNodes` |  | `""` |
| `redisCluster.redisRootNodesJson` |  | `{}` |
| `redisCluster.redisOptionsJson` |  | `{}` |
| `mongoDb.enabled` |  | `false` |
| `mongoDb.databaseName` |  | `""` |
| `mongoDb.collectionName` |  | `""` |
| `horizontalScaling.publishPayloadToChannel` |  | `false` |
| `streaming.enabled` |  | `true` |
| `streaming.maxDuration` |  | `60000` |
| `streaming.pingInterval` |  | `30000` |
| `serviceAccount.create` |  | `true` |
| `serviceAccount.annotations` |  | `{}` |
| `serviceAccount.name` |  | `""` |
| `podAnnotations` |  | `{}` |
| `podSecurityContext` |  | `{}` |
| `securityContext` |  | `{}` |
| `service.type` |  | `"ClusterIP"` |
| `service.port` |  | `3300` |
| `ingress.enabled` |  | `false` |
| `ingress.className` |  | `""` |
| `ingress.annotations` |  | `{}` |
| `ingress.hosts` |  | `[{"host": "chart-example.local", "paths": [{"path": "/", "pathType": "ImplementationSpecific"}]}]` |
| `ingress.tls` |  | `[]` |
| `resources` |  | `{}` |
| `autoscaling.enabled` |  | `false` |
| `autoscaling.minReplicas` |  | `1` |
| `autoscaling.maxReplicas` |  | `100` |
| `autoscaling.targetCPUUtilizationPercentage` |  | `80` |
| `nodeSelector.kubernetes.io/arch` |  | `"amd64"` |
| `nodeSelector.kubernetes.io/os` |  | `"linux"` |
| `tolerations` |  | `[]` |
| `affinity` |  | `{}` |
