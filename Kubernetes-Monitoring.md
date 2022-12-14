## Kubelet

The kubelet is the primary "node agent" that runs on each node. 


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

## GKE Monitoring

https://www.containiq.com/post/gke-monitoring


 
## Prometheus

Prometheus is an open-source systems monitoring and alerting toolkit originally built at SoundCloud. Since its inception in 2012, many companies and organizations have adopted Prometheus, and the project has a very active developer and user community. It is inspired by Google Borg Monitor.

https://prometheus.io/

[https://www.youtube.com/watch?v=h4Sl21AKiDg](https://www.youtube.com/watch?v=h4Sl21AKiDg)

[https://www.youtube.com/watch?v=XToKHYXSUyc](https://www.youtube.com/watch?v=XToKHYXSUyc)

### Monitoring applications on Google managed prometheus
https://blog.searce.com/monitor-your-applications-on-google-managed-prometheus-4416070f9fd0

## Jaeger

Jaeger is a tracing system released by Uber Technologies; it's used for troubleshooting and monitoring transactions in complex distributed systems.

https://github.com/jaegertracing/jaeger

## Kubewatch

Kubewatch is a Kubernetes watcher that publishes event notifications in a Slack channel. This tool allows you to specify the resources you want to monitor. It is written in Golang and uses a Kubernetes client library to interact with a Kubernetes API server.

https://github.com/bitnami-labs/kubewatch




## Grafana

[https://grafana.com/](https://grafana.com/)

The Grafana project was started by Torkel ??degaard in 2014 and has become one of the most popular open source projects on GitHub. It allows you to query, visualize, and alert on metrics and logs no matter where they are stored.

Grafana has a pluggable data source model and comes bundled with rich support for many of the most popular time series databases like Graphite, Prometheus, Elasticsearch, OpenTSDB, and InfluxDB. It also has built-in support for cloud monitoring vendors like Google Stackdriver, Amazon Cloudwatch, and Microsoft Azure, and SQL databases like MySQL and Postgres. Grafana is the only tool that can combine data from so many places into a single dashboard.


## Weave Scope

Weave Scope is a zero-configuration monitoring tool developed by Weaveworks. It generates a map of processes, containers, and hosts in a Kubernetes cluster to help understand Docker containers in real time. It can also be used to manage containers and run diagnostic commands on containers without leaving the graphical UI.

https://github.com/weaveworks/scope
