## Kubelet

The kubelet is the primary "node agent" that runs on each node. It can register the node with the apiserver using one of: the hostname; a flag to override the hostname; or specific logic for a cloud provider.

The kubelet works in terms of a PodSpec. A PodSpec is a YAML or JSON object that describes a pod. The kubelet takes a set of PodSpecs that are provided through various mechanisms (primarily through the apiserver) and ensures that the containers described in those PodSpecs are running and healthy. The kubelet doesn't manage containers which were not created by Kubernetes.

In a Kubernetes cluster, Kubelet acts as a bridge between the master and the nodes. It is the primary node agent that runs on each node and maintains a set of pods. Kubelet watches for PodSpecs via the Kubernetes API server and collects resource utilization statistics and pod and events status.

Kubelet fetches individual container usage statistics from Docker's Container Advisor (cAdvisor). But Kubelet also accepts PodSpecs provided through different mechanisms and ensures that the containers described in those PodSpecs are up and running. These aggregated pod resource usage statistics are exposed via a REST API.

https://kubernetes.io/docs/reference/command-line-tools-reference/kubelet/

## Kubernetes dashboard

Kubernetes Dashboard is a general purpose, web-based UI for Kubernetes clusters. It allows users to manage applications running in the cluster and troubleshoot them, as well as manage the cluster itself.

https://github.com/kubernetes/dashboard

## cAdvisor

cAdvisor is a container resource usage and performance analysis agent; it's integrated into the Kubelet binary. cAdvistor auto-discovers all containers in a machine and collects statistics about memory, network usage, filesystem, and CPU. cAdvisor has native support for Docker containers. It does not operate at the pod level, but on each node.

https://github.com/google/cadvisor

## Kube state metrics


Kube-state-metrics listens to the Kubernetes API server and generates metrics about the state of numerous Kubernetes objects, including cron jobs, config maps, pods, and nodes. These metrics are unmodified, unlike kubectl metrics that use the same Kubernetes API but apply some heuristics to display comprehensible and readable messages

https://github.com/kubernetes/kube-state-metrics

Kube-state-metrics uses the Golang Prometheus client to export metrics in the Prometheus metrics exposition format and expose metrics on an HTTP endpoint. Prometheus can consume the web endpoint.

## Metrics server

Metrics Server is a scalable, efficient source of container resource metrics for Kubernetes built-in autoscaling pipelines.

Metrics Server collects resource metrics from Kubelets and exposes them in Kubernetes apiserver through Metrics API for use by Horizontal Pod Autoscaler and Vertical Pod Autoscaler. Metrics API can also be accessed by kubectl top, making it easier to debug autoscaling pipelines.

https://github.com/kubernetes-sigs/metrics-server
 
## Prometheus

Prometheus is an open-source systems monitoring and alerting toolkit originally built at SoundCloud. Since its inception in 2012, many companies and organizations have adopted Prometheus, and the project has a very active developer and user community. It is inspired by Google Borg Monitor.

https://prometheus.io/

[https://www.youtube.com/watch?v=h4Sl21AKiDg](https://www.youtube.com/watch?v=h4Sl21AKiDg)

[https://www.youtube.com/watch?v=XToKHYXSUyc](https://www.youtube.com/watch?v=XToKHYXSUyc)

## Jaeger

Jaeger is a tracing system released by Uber Technologies; it's used for troubleshooting and monitoring transactions in complex distributed systems.

https://github.com/jaegertracing/jaeger

## Kubewatch

Kubewatch is a Kubernetes watcher that publishes event notifications in a Slack channel. This tool allows you to specify the resources you want to monitor. It is written in Golang and uses a Kubernetes client library to interact with a Kubernetes API server.

https://github.com/bitnami-labs/kubewatch




## Grafana

[https://grafana.com/](https://grafana.com/)

The Grafana project was started by Torkel Ödegaard in 2014 and has become one of the most popular open source projects on GitHub. It allows you to query, visualize, and alert on metrics and logs no matter where they are stored.

Grafana has a pluggable data source model and comes bundled with rich support for many of the most popular time series databases like Graphite, Prometheus, Elasticsearch, OpenTSDB, and InfluxDB. It also has built-in support for cloud monitoring vendors like Google Stackdriver, Amazon Cloudwatch, and Microsoft Azure, and SQL databases like MySQL and Postgres. Grafana is the only tool that can combine data from so many places into a single dashboard.


## Weave Scope

Weave Scope is a zero-configuration monitoring tool developed by Weaveworks. It generates a map of processes, containers, and hosts in a Kubernetes cluster to help understand Docker containers in real time. It can also be used to manage containers and run diagnostic commands on containers without leaving the graphical UI.

https://github.com/weaveworks/scope
