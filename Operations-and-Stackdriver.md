





## Cloud Operations

[AKA Stackdriver](https://cloud.google.com/products/operations)


### Introduction

[Monitor](Monitoring), [trace](Tracing), troubleshoot, and improve application performance on your Google Cloud environment.

[https://cloud.google.com/stackdriver/docs](https://cloud.google.com/stackdriver/docs)

Introduction to basic logging and monitoring with Stackdriver with a quick demo.

[https://www.youtube.com/watch?v=LVFr5qW4wO4](https://www.youtube.com/watch?v=LVFr5qW4wO4)


### Cloud Logging

Cloud Logging allows you to store, search, analyze, monitor, and alert on logging data and events from Google Cloud and Amazon Web Services. Using Cloud Logging includes access to the [BindPlane service](https://bluemedora.com/products/bindplane/bindplane-for-stackdriver/), which you can use to collect logging data from over 150 common application components, on-premises systems, and hybrid cloud systems.

[https://cloud.google.com/logging/docs](https://cloud.google.com/logging/docs)

GCP Essentials: Cloud Logging.

[https://www.youtube.com/watch?v=gyDp-Cl_MdA](https://www.youtube.com/watch?v=gyDp-Cl_MdA)

### Types of metrics

https://cloud.google.com/blog/products/operations/in-depth-explanation-of-operational-metrics-at-google-cloud

### Cloud Monitoring

Cloud Monitoring collects metrics, events, and metadata from Google Cloud, Amazon Web Services (AWS), hosted uptime probes, and application instrumentation. Google Cloud's operations suite ingests that data and generates insights via dashboards, charts, and alerts. 

[https://cloud.google.com/monitoring/docs](https://cloud.google.com/monitoring/docs)

#### Getting started with Cloud Monitoring

[https://www.youtube.com/watch?v=wY8cmFY4ua8](https://www.youtube.com/watch?v=wY8cmFY4ua8)


#### Cloud Monitoring Agents

The Cloud Monitoring agent is a collectd-based daemon that gathers system and application metrics from virtual machine instances and sends them to Monitoring. By default, the Monitoring agent collects disk, CPU, network, and process metrics.

[https://cloud.google.com/monitoring/agent](https://cloud.google.com/monitoring/agent)


#### Dashboards

[https://cloud.google.com/monitoring/charts/dashboards](https://cloud.google.com/monitoring/charts/dashboards)


#### Metrics Explorer

[https://cloud.google.com/monitoring/charts/metrics-explorer](https://cloud.google.com/monitoring/charts/metrics-explorer)


### Cloud Trace

Cloud Trace is a distributed tracing system for Google Cloud that collects latency data from applications and displays it in near real-time in the [Google Cloud Console](https://console.cloud.google.com/).

[https://cloud.google.com/trace/docs](https://cloud.google.com/trace/docs)

Cloud Trace is a feature of the Google Cloud Platform that allows you to view the RPCs (remote procedure calls) invoked by your App Engine application and to view and analyze the time taken to complete each RPC and the overall latency of processing your applications requests.

[https://www.youtube.com/watch?v=NCFDqeo7AeY](https://www.youtube.com/watch?v=NCFDqeo7AeY)


### Cloud Debugger

Cloud Debugger is a feature of Google Cloud Platform that lets you inspect the state of an application, at any code location, without stopping or slowing down the running app. Cloud Debugger makes it easier to view the application state without adding logging statements.

[https://cloud.google.com/debugger/docs](https://cloud.google.com/debugger/docs)

Cloud Debugger makes it easier to view the application state at any point in the code without any modifications to your code.  

[https://www.youtube.com/watch?v=DCtLE6zPMdQ](https://www.youtube.com/watch?v=DCtLE6zPMdQ)


### Cloud Profiler

Cloud Profiler is a statistical, low-overhead profiler that continuously gathers CPU usage and memory-allocation information from your production applications. It attributes that information to the application's source code, helping you identify the parts of the application consuming the most resources, and otherwise illuminating the performance characteristics of the code.

[https://cloud.google.com/profiler/docs](https://cloud.google.com/profiler/docs)

#### Introduction to Stackdriver Profiler

[https://www.youtube.com/watch?v=KXjPhadwr8k](https://www.youtube.com/watch?v=KXjPhadwr8k)


### Error Reporting

Error Reporting aggregates and displays errors produced in your running cloud services.

[https://cloud.google.com/error-reporting/docs](https://cloud.google.com/error-reporting/docs)

Error reporting can be useful in identifying and resolving bugs in your application. 

[https://www.youtube.com/watch?v=GANi9eRxhHs](https://www.youtube.com/watch?v=GANi9eRxhHs)


### Service Level Monitoring

Service monitoring and the SLO API help you manage your services like Google manages its own services. 

[https://cloud.google.com/stackdriver/docs/solutions/slo-monitoring](https://cloud.google.com/stackdriver/docs/solutions/slo-monitoring)

Basics of Service Level Monitoring.

[https://www.youtube.com/watch?v=u84TKyX8SfU](https://www.youtube.com/watch?v=u84TKyX8SfU)


### Qwiklabs


#### Operations Suite

In this fundamental-level quest, you will learn the ins and outs of Google Cloud's operations suite, an important service for generating insights into the health of your applications. It provides a wealth of information in application monitoring, report logging, and diagnoses. The labs in this quest will give you hands-on practice with and will teach you how to monitor virtual machines, generate logs and alerts, and create custom metrics for application data.

[Google Cloud's Operations Suite](https://www.qwiklabs.com/quests/35?catalog_rank=%7B%22rank%22%3A6%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&search_id=7468028)


#### Cloud Monitoring

In this fundamental-level quest, you will learn the ins and outs of Google Cloud's operations suite, an important service for generating insights into the health of your applications. It provides a wealth of information in application monitoring, report logging, and diagnoses. The labs in this quest will give you hands-on practice with and will teach you how to monitor virtual machines, generate logs and alerts, and create custom metrics for application data. 

[Monitor and Log with Google Cloud Operations Suite](https://www.qwiklabs.com/quests/143?catalog_rank=%7B%22rank%22%3A2%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&search_id=7468028)


#### Cloud Trace

When supporting a production system that services HTTP requests or provides an API, it is important to measure the latency of your endpoints to detect when a system's performance is not operating within specification. In monolithic systems this single latency measure may be useful to detect and diagnose deteriorating behavior. With modern microservice architectures, however, this becomes much more difficult because a single request may result in numerous additional requests to other systems before the request can be fully handled. Deteriorating performance in an underlying system may impact all other systems that rely on it. While latency can be measured at each service endpoint, it can be difficult to correlate slow behavior in the public endpoint with a particular sub-service that is misbehaving.

[Using Cloud Trace on Kubernetes Engine](https://www.qwiklabs.com/focuses/5159?catalog_rank=%7B%22rank%22%3A19%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&parent=catalog&search_id=7468017)


#### Cloud Logging

Cloud Logging is a fully managed service that performs at scale. It can ingest application and system log data from thousands of VMs and, even better, analyze all that log data in real time. In this fundamental-level Quest, you learn how to store, search, analyze, monitor, and alert on log data and events from Google Cloud. 

[Cloud Logging](https://www.qwiklabs.com/quests/81?catalog_rank=%7B%22rank%22%3A1%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&search_id=7468028)


#### Application Logs

In this hands-on lab, you learn how to use Cloud Logging to accumulate application logs in a single place, filter to reach the required log, understand how to create logs based metrics for advanced analysis, examine the audit logs use case, and export logs for compliance and/or advanced analysis needs.

[Fundamentals of Cloud Logging](https://www.qwiklabs.com/focuses/10911?catalog_rank=%7B%22rank%22%3A12%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&parent=catalog&search_id=7468061)


#### BigQuery Logging

In this lab you view the BigQuery logs inside Cloud Logging, setup a sink to export them back into BigQuery, and then use SQL to analyze the logs.

[Using BigQuery and Cloud Logging to Analyze BigQuery Usage](https://www.qwiklabs.com/focuses/6100?catalog_rank=%7B%22rank%22%3A15%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&parent=catalog&search_id=7468061)

## grafana

Using stackdriver with grafana. 

https://grafana.com/docs/grafana/latest/datasources/google-cloud-monitoring/