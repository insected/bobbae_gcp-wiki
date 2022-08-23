[Cloud Operations Suite](Operations-and-Stackdriver) is new name for [Stackdriver](https://cloud.google.com/products/operations) which includes Cloud Monitoring, Cloud logging, debugging, tracing, dashboarding, etc.

[Cloud Monitoring](https://cloud.google.com/monitoring) collects measurements of your service and of the Google Cloud resources that you use.  


[Cloud Monitoring](https://cloud.google.com/monitoring/docs/monitoring-overview) collects metrics, events, and metadata from Google Cloud, Amazon Web Services (AWS), hosted uptime probes, and application instrumentation.  You can use [Cloud Monitoring](https://cloud.google.com/monitoring/docs) tools to visualize and monitor these measurements.

## SRE

https://sre.google/sre-book/monitoring-distributed-systems/

### Four Golden Signals

https://sre.google/sre-book/monitoring-distributed-systems/#xref_monitoring_golden-signals

## Stackdriver

Cloud Monitoring [is part](Operations-and-Stackdriver) of [Google Cloud operations suite](https://cloud.google.com/stackdriver/docs).

## Google Cloud Metrics

https://cloud.google.com/monitoring/api/metrics_gcp

## Logging

[Cloud Logging](Logging) is a fully managed service that allows you to store, search, analyze, monitor, and alert on logging data and events from Google Cloud and Amazon Web Services. You can collect logging data from over 150 common application components, on-premises systems, and hybrid cloud systems.


### Node.js cloud logging library

https://cloud.google.com/blog/products/devops-sre/get-more-insights-with-the-new-version-of-the-nodejs-library


### Log alerting for Cloud SQL

https://cloud.google.com/blog/products/databases/cloud-sql-alerting

## Types of metrics

https://cloud.google.com/blog/products/operations/in-depth-explanation-of-operational-metrics-at-google-cloud

## Error Reporting

[Error Reporting](https://cloud.google.com/error-reporting/docs
) aggregates and displays errors produced in your running cloud services. Using the centralized error management interface, you can find your application's top or new errors so that you can fix the root causes faster.

https://cloud.google.com/blog/products/devops-sre/application-exceptions-surfaced-automatically

## snooze 

https://cloud.google.com/blog/products/devops-sre/snooze-your-alert-policies-cloud-monitoring


## Cloud Monitoring Tutorials

https://cloud.google.com/monitoring/tutorials

### Query metrics from Cloud Monitoring in Golang

https://medium.com/google-cloud/querying-metrics-from-google-cloud-monitoring-in-golang-2631ee3d33c1

## Cloud Monitoring Dashboard Samples

https://cloud.google.com/blog/products/operations/dashboards-cloud-monitoring-made-easier-samples

### GKE Monitoring

https://www.containiq.com/post/gke-monitoring

### Cloud monitoring for Vertex AI pipelines
https://medium.com/datatonic/vertex-ai-tips-and-tricks-setting-up-alerts-for-vertex-pipelines-with-google-cloud-monitoring-3e0a277795cf

### Network performance monitoring

https://medium.com/google-cloud/network-performance-diagnostics-with-gcp-performance-dashboard-52d93bc85a02

### Monarch

https://research.google/pubs/pub50652/

## Prometheus & Grafana

Open source projects like [Prometheus](https://prometheus.io/) and [Grafana](https://grafana.com/) are often used in Kubernetes along with [metrics server](https://github.com/kubernetes-sigs/metrics-server).


### Managed Prometheus

https://cloud.google.com/managed-prometheus

https://cloud.google.com/blog/products/devops-sre/easy-managed-prometheus-metrics-service-for-kubernetes

## ELK

[ELK Stack](https://www.elastic.co/what-is/elk-stack) provides similar features.

## Other Monitoring tools

There are [many other monitoring](https://github.com/crazy-canux/awesome-monitoring) tools that are used in different contexts.

### GCPing

https://github.com/GoogleCloudPlatform/gcping

## Examples

### Creating custom Google Chat notifications with Cloud Monitoring and Cloud Run

https://cloud.google.com/blog/products/operations/write-and-deploy-cloud-monitoring-alert-notifications-to-third-party-services

### Set up alert on GCP 
https://medium.com/@junxie2/setup-alert-at-gcp-on-services-bd10df26b692

### Webhook, Pub/Sub, and Slack Alerting notification channels

https://cloud.google.com/blog/products/operations/pub-sub-webook-and-slack-notifications-are-now-available

### Deliver exception messages through Slack and Webhooks

https://cloud.google.com/blog/products/devops-sre/use-slack-and-webhooks-for-notifications

### GCP Monitoring Operations Suite Alerts into Google Chat using Pubsub and Cloud Function

https://medium.com/cts-technologies/gcp-operations-suite-alerts-into-google-chat-1a3c39f84187
