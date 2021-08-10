Cloud Logging is a fully managed service that allows you to store, search, analyze, monitor, and alert on logging data and events from Google Cloud and Amazon Web Services. You can collect logging data from over 150 common application components, on-premises systems, and hybrid cloud systems.

## Logs Explorer

Cloud Logging has introduced a new version of its interface for analyzing logs data, the Logs Explorer. It is more responsive and introduces new features for letting you quickly and efficiently retrieve, view, and analyze logs from your queries.

While the Logs Explorer is being enhanced, the Legacy Logs Viewer will continue to be maintained. You can switch back and forth between the Legacy Logs Viewer and the Logs Explorer when analyzing logs.



https://cloud.google.com/logging/docs/view/logs-viewer-interface


### Dashboard

The Logs Dashboard provides a high-level overview into the health of the systems that are running within a Google Cloud project. It provides you with a visualization of the log severity fields for each resource within the Cloud project over time. This enables you to spot trends in the behavior of your systems, helping you monitor your workloads, and diagnose and resolve problems.

https://cloud.google.com/logging/docs/view/dashboard

### Exploring external logs

To view the logs that you are sending from an Amazon Web Services (AWS) account to Logging, select the [AWS connector project](https://cloud.google.com/monitoring/settings/aws-accounts#connector-project) in the Google Cloud Console project picker and then use the [Legacy Logs Viewer](https://cloud.google.com/logging/docs/view/overview). The AWS connector project stores the Amazon Resource Name (ARN) for your AWS account and links your AWS account to Google Cloud services. For more information, see [Viewing metrics for AWS accounts](https://cloud.google.com/monitoring/settings/aws-accounts).

## API


The Cloud Logging API lets you programmatically read and write log entries, set up exclusions, create logs-based metrics, and manage export sinks. This section provides reference pages for the API.

There is  a [REST version](https://cloud.google.com/logging/docs/reference/v2/rest) and the [gRPC version](https://cloud.google.com/logging/docs/reference/v2/rpc) of the API.

https://cloud.google.com/logging/docs/reference/api-overview

### Client libraries

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

### Managing Log buckets

https://cloud.google.com/logging/docs/buckets

## Queries

https://cloud.google.com/logging/docs/view/building-queries

## Log Router

https://cloud.google.com/logging/docs/routing/overview

## Ops Agent

https://cloud.google.com/logging/docs/agent/ops-agent

## Logs based metrics

https://cloud.google.com/logging/docs/logs-based-metrics

## Routing logs

Cloud Logging receives log entries through the Cloud Logging API where they pass through the Log Router. The sinks in the Log Router check each log entry against existing inclusion and exclusion filters that determine if the log entry should be sent to storage destinations, including in Cloud Logging buckets, or excluded entirely from ingestion by Cloud Logging. You can use sinks to route logs to multiple destinations.

To reliably route logs, the Log Router also stores the logs temporarily, which buffers against temporary disruptions on any sink. Note that the Log Router's temporary storage is distinct from the longer term storage provided by Logging buckets.

Using sinks, you can route some or all of your logs to supported destinations or exclude log entries from being stored in Cloud Logging. 

https://cloud.google.com/logging/docs/export


[[https://cloud.google.com/logging/docs/images/logs-router-image.png]]

https://cloud.google.com/logging/docs/routing/overview


### Supported destinations

https://cloud.google.com/logging/docs/export#supported-destinations

### Log sinks

Sinks route log entries to storage destinations and are also used to exclude log entries from being written to Cloud Logging. Log sinks combine a filter expression and a destination.

Cloud Logging provides two predefined log sinks for each Google Cloud project: _Required and _Default. All logs that are generated in a Google Cloud project are automatically processed through these two log sinks and then are stored in the correspondingly named _Required and _Default log buckets.

Log sinks act independently of each other. Regardless of how the predefined log sinks process your log entries, you can create your own log sinks to route some or all of your logs to various supported destinations or to exclude them entirely from being stored by Cloud Logging.

### How sinks work

All log entries written to the Cloud Logging API pass through the Log Router. Every time a log entry arrives in a Cloud project, folder, billing account, or organization resource, Logging compares the log entry to the filters of the sinks associated with the resource.

https://cloud.google.com/logging/docs/export#overview

Cloud Logging provides two predefined log sinks for each Google Cloud project: _Required and _Default. All logs that are generated in a Google Cloud project are automatically processed through these two log sinks and then are stored in the correspondingly named _Required and _Default log buckets.



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
