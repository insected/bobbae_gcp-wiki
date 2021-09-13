[Cloud Logging](https://cloud.google.com/logging) is a fully managed service that allows you to store, search, analyze, monitor, and alert on logging data and events from Google Cloud and Amazon Web Services. You can collect logging data from over 150 common application components, on-premises systems, and hybrid cloud systems.

## Cloud Monitoring


[Cloud Monitoring](Monitoring) collects metrics, events, and metadata from Google Cloud, Amazon Web Services (AWS), hosted uptime probes, and application instrumentation. Using the [BindPlane service](https://bluemedora.com/products/bindplane/bindplane-for-stackdriver/), you can also collect this data from over 150 common application components, on-premise systems, and hybrid cloud systems. Google Cloud's operations suite ingests that data and generates insights via dashboards, charts, and alerts. BindPlane is included with your Google Cloud project at no additional cost.

To collect metrics data from your Compute Engine instances, [create an Agent Policy](https://cloud.google.com/stackdriver/docs/solutions/managing-agent-policies) that automatically installs and maintains the Google Cloud's operations suite agents across your fleet of VMs.

https://cloud.google.com/monitoring/docs

## Error Reporting

Error Reporting aggregates and displays errors produced in your running cloud services. Using the centralized error management interface, you can find your application's top or new errors so that you can fix the root causes faster.



https://cloud.google.com/error-reporting/docs


## Cloud Operations Suite

[Cloud Operations Suite](Operations-and-Stackdriver) is new name for [Stackdriver](https://cloud.google.com/products/operations) which includes Cloud Monitoring, Cloud logging, debugging, tracing, dashboarding, etc.

https://cloud.google.com/products/operations

## Cloud Logging Concepts

https://cloud.google.com/logging/docs/concepts

## Cloud Logs Explorer

Cloud Logging has introduced a new version of its interface for analyzing logs data, the Logs Explorer. It is more responsive and introduces new features for letting you quickly and efficiently retrieve, view, and analyze logs from your queries.

While the Logs Explorer is being enhanced, the Legacy Logs Viewer will continue to be maintained. You can switch back and forth between the Legacy Logs Viewer and the Logs Explorer when analyzing logs.



https://cloud.google.com/logging/docs/view/logs-viewer-interface



### Cloud Logs Dashboard

The Logs Dashboard provides a high-level overview into the health of the systems that are running within a Google Cloud project. It provides you with a visualization of the log severity fields for each resource within the Cloud project over time. This enables you to spot trends in the behavior of your systems, helping you monitor your workloads, and diagnose and resolve problems.

https://cloud.google.com/logging/docs/view/dashboard

### Exploring external logs

To view the logs that you are sending from an Amazon Web Services (AWS) account to Logging, select the [AWS connector project](https://cloud.google.com/monitoring/settings/aws-accounts#connector-project) in the Google Cloud Console project picker and then use the [Legacy Logs Viewer](https://cloud.google.com/logging/docs/view/overview). 

The AWS connector project stores the Amazon Resource Name (ARN) for your AWS account and links your AWS account to Google Cloud services. 

For more information, see [Viewing metrics for AWS accounts](https://cloud.google.com/monitoring/settings/aws-accounts).

#### On-premise and hybrid cloud logging

Google Cloud partners with [Blue Medora](https://www.bluemedora.com/) to provide [Bindplane](https://bluemedora.com/products/bindplane/) to Logging users at no additional cost. Users can collect their own data from their on-premise and hybrid cloud platforms and send it to Cloud Logging for analysis.



https://cloud.google.com/logging/docs/blue-medora/on-premise-hybrid-logging


## API


The Cloud Logging API lets you programmatically read and write log entries, set up exclusions, create logs-based metrics, and manage export sinks. This section provides reference pages for the API.

There is  a [REST version](https://cloud.google.com/logging/docs/reference/v2/rest) and the [gRPC version](https://cloud.google.com/logging/docs/reference/v2/rpc) of the API.

https://cloud.google.com/logging/docs/reference/api-overview

### Client libraries

Cloud Logging client libraries are idiomatic interfaces around the API. Client libraries provide an integration option with Logging, in addition to the [Logging agent](https://cloud.google.com/logging/docs/agent) available by default in most Google Cloud services. To learn more about setting up Logging using a language runtime, see [Setting up Language Runtimes](https://cloud.google.com/logging/docs/setup).



https://cloud.google.com/logging/docs/reference/libraries

### Exporting Logs in the API

https://cloud.google.com/logging/docs/api/tasks/exporting-logs

## CLI

https://cloud.google.com/logging/docs/reference/tools/gcloud-logging

## log buckets

Cloud Logging uses log buckets as containers in your Google Cloud projects to store and organize your logs data. The logs that you store in Cloud Logging are indexed, optimized, and delivered to let you analyze your logs in real time. These are different storage entities than the similarly named Cloud Storage buckets.

You can create sinks to route all, or just a subset, of your logs to any log bucket. This flexibility allows you to choose the Cloud project in which your logs are stored and what other logs are stored with them.

Cloud Logging provides every Cloud project with the _Required and _Default log buckets. In the default configuration, all logs generated in a Cloud project are stored in the _Required and _Default log buckets, which live in the Cloud project that the logs are generated in. You can also create custom log buckets.



https://cloud.google.com/logging/docs/buckets

### User defined Log buckets

By applying log sinks to your user-defined log buckets, you can route any subset of your logs to any log bucket, letting you choose which Cloud project your logs are stored in and which other logs are stored with them.

For example, for any log generated in Project-A, you can configure a sink to route that log to user-defined buckets in Project-A or Project-B.

https://cloud.google.com/logging/docs/storage#user-buckets

## Policy

https://cloud.google.com/resource-manager/docs/organization-policy/overview

### Resource locations restriction

https://cloud.google.com/resource-manager/docs/organization-policy/defining-locations

#### Regionalization

https://cloud.google.com/logging/docs/storage#regionalization

#### Regionalized logs

https://cloud.google.com/logging/docs/regionalized-logs

### Custom retention for buckets

https://cloud.google.com/logging/docs/buckets#custom-retention

## Queries

https://cloud.google.com/logging/docs/view/building-queries

## Log Router

Cloud Logging receives log entries through the Cloud Logging API where they pass through the Log Router. The sinks in the Log Router check each log entry against existing inclusion and exclusion filters that determine if the log entry should be sent to storage destinations, including in Cloud Logging buckets, or excluded entirely from ingestion by Cloud Logging. You can use sinks to route logs to multiple destinations.

To reliably route logs, the Log Router also stores the logs temporarily, which buffers against temporary disruptions on any sink. Note that the Log Router's temporary storage is distinct from the longer term storage provided by Logging buckets.

https://cloud.google.com/logging/docs/routing/overview

## Log Agent

Log collecting agents  for  Linux and Windows VM instances.


https://cloud.google.com/logging/docs/agent

### Ops Agent


The Ops Agent is the primary agent for collecting telemetry from your Compute Engine instances. Combining logging and metrics into a single agent, the Ops Agent uses [Fluent Bit](https://fluentbit.io/) for logs, which supports high-throughput logging, and the [OpenTelemetry Collector](https://opentelemetry.io/docs/collector/) for metrics.

https://cloud.google.com/logging/docs/agent/ops-agent

#### OpenTelemetry

https://opentelemetry.io/

OpenTelemetry is a collection of tools, APIs, and SDKs. You can use it to instrument, generate, collect, and export telemetry data (metrics, logs, and traces).

#### sqlcommenter

https://cloud.google.com/blog/topics/developers-practitioners/introducing-sqlcommenter-open-source-orm-auto-instrumentation-library





#### Fluentbit

https://github.com/fluent/fluent-bit

### Legacy Logging Agent

Legacy Log Agents are based on [fluentd](https://www.fluentd.org/) that runs on your virtual machine (VM) instances.


It is a best practice to run the Logging agent on all your VM instances. The agent runs under both Linux and Windows.


If you are running specialized logging workloads that require higher throughput and/or improved resource-efficiency compared to the standard Cloud Logging agent, consider using the Ops agent.



https://cloud.google.com/logging/docs/agent/logging


### Logging Agent Source Code

https://github.com/GoogleCloudPlatform/google-fluentd


## Structured logging

In Cloud Logging, structured logs refer to log entries that use the jsonPayload field to add structure to their payloads.

If you use the Cloud Logging API or the gcloud command-line tool, you can control the structure of your payloads. See Writing structured logs for examples.

If you use the Cloud Logging agent to get your log entries, you can specify that the Logging agent convert your payloads to JSON format.


https://cloud.google.com/logging/docs/structured-logging#source


## Logs based metrics

Logs-based metrics are based on the content of log entries. For example, the metrics can record the number of log entries containing particular messages, or they can extract latency information reported in log entries. You can use logs-based metrics in Cloud Monitoring charts and alerting policies.

https://cloud.google.com/logging/docs/logs-based-metrics

## Logs based alerts

You can use log-based alerts to notify you whenever a specific message appears in your included logs. This document describes how to do the following:

- Create and test a log-based alert.
- Edit a log-based alert.
- Delete a log-based alert.

https://cloud.google.com/logging/docs/alerting/log-based-alerts

## Routing logs

Cloud Logging receives log entries through the Cloud Logging API where they pass through the Log Router. The sinks in the Log Router check each log entry against existing inclusion and exclusion filters that determine if the log entry should be sent to storage destinations, including in Cloud Logging buckets, or excluded entirely from ingestion by Cloud Logging. You can use sinks to route logs to multiple destinations.

To reliably route logs, the Log Router also stores the logs temporarily, which buffers against temporary disruptions on any sink. Note that the Log Router's temporary storage is distinct from the longer term storage provided by Logging buckets.

Using sinks, you can route some or all of your logs to supported destinations or exclude log entries from being stored in Cloud Logging. 

https://cloud.google.com/logging/docs/export



https://cloud.google.com/logging/docs/routing/overview


### Supported destinations

https://cloud.google.com/logging/docs/export#supported-destinations

### Log sinks

Sinks route log entries to storage destinations and are also used to exclude log entries from being written to Cloud Logging. Log sinks combine a filter expression and a destination.

Cloud Logging provides two predefined log sinks for each Google Cloud project: _Required and _Default. All logs that are generated in a Google Cloud project are automatically processed through these two log sinks and then are stored in the correspondingly named _Required and _Default log buckets.

Log sinks act independently of each other. Regardless of how the predefined log sinks process your log entries, you can create your own log sinks to route some or all of your logs to various supported destinations or to exclude them entirely from being stored by Cloud Logging.

https://cloud.google.com/logging/docs/api/tasks/exporting-logs#introduction_to_sinks

### How sinks work

All log entries written to the Cloud Logging API pass through the Log Router. Every time a log entry arrives in a Cloud project, folder, billing account, or organization resource, Logging compares the log entry to the filters of the sinks associated with the resource.

https://cloud.google.com/logging/docs/export#overview

Cloud Logging provides two predefined log sinks for each Google Cloud project: _Required and _Default. All logs that are generated in a Google Cloud project are automatically processed through these two log sinks and then are stored in the correspondingly named _Required and _Default log buckets.


## Tutorials

https://cloud.google.com/logging/tutorials

## Quickstarts

### Quickstart using Logs Explorer

https://cloud.google.com/logging/docs/view/logs-viewer-interface

### Quickstart using Logging tools

https://cloud.google.com/logging/docs/quickstart-sdk

### Quickstart using python

https://cloud.google.com/logging/docs/quickstart-python

## Code Samples

https://cloud.google.com/logging/docs/how-to#code-samples


## How-to

https://cloud.google.com/logging/docs/how-to


## Aggregation

A common way to manage your logs is to aggregate them from across your organization into a single log bucket. This guide walks through this process, using the example of aggregating all audit logs.

This process involves the following steps:

- Creating the log bucket for storing the aggregated logs.

- Creating the sink at the organization level to route the logs to the new logs bucket.

- Configuring read access to the new log bucket.

- Searching logs from the Logs Explorer page.


https://cloud.google.com/logging/docs/central-log-storage


## GKE Multi-tenant logging

It's common for multiple teams to share a single GKE cluster. Sharing a cluster provides multiple advantages including easier service discovery, simplified security, and it means that cluster administrators have fewer clusters to maintain. Individual application teams often have their own separate project, however. This structure, having a main GKE cluster, but separate namespaces for each application team, is called multi-tenancy. The application team's project is called the tenant.

With Google Cloud, GKE cluster admins can create a system where logs for the cluster remain in the main GKE project, and tenant logs are distributed to tenant projects. To configure your logs this way, utilize the Cloud Logging Log Router. The Log Router gives you control over how logs flow within your Google Cloud project and how logs flow to other Google Cloud projects.

https://cloud.google.com/stackdriver/docs/solutions/gke/multi-tenant-logging


## Data Governance

https://cloud.google.com/resources/data-governance-logs-best-practices-whitepaper


## Compliance

https://services.google.com/fh/files/misc/whitepaper_data_governance_logs_how_to.pdf

#### Regionalized logs

https://cloud.google.com/logging/docs/regionalized-logs

## List of Logs Related Resources

### List of Log Analysis Research materials

https://github.com/logpai/awesome-log-analysis

### List of Monitoring and Logging tools

https://github.com/Enapiuz/awesome-monitoring

### List of Log Analysis and Incident Management Tools

https://github.com/meirwah/awesome-incident-response

### List of Monitoring tools

https://github.com/adriannovegil/awesome-observability

### List of Log and Anomaly Detection tools

https://github.com/WeibinMeng/log-anomaly-detection

