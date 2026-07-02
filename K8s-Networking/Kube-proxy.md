## Deployment vs DaemonSet
| Deployment                                        | DaemonSet                                     |
| ------------------------------------------------- | --------------------------------------------- |
| You specify the number of replicas.               | Kubernetes creates one Pod per eligible node. |
| Used for applications (Spring Boot, React, etc.). | Used for node-level infrastructure.           |
| Pods can all end up on a subset of nodes.         | Every eligible node gets one Pod.             |
| Example: Payment Service.                         | Example: kube-proxy, Fluentd, Node Exporter.  |
