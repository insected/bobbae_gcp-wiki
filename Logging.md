Cloud Logging is a fully managed service that allows you to store, search, analyze, monitor, and alert on logging data and events from Google Cloud and Amazon Web Services. You can collect logging data from over 150 common application components, on-premises systems, and hybrid cloud systems.

## Logs Explorer

https://cloud.google.com/logging/docs/view/logs-viewer-interface

## API

https://cloud.google.com/logging/docs/reference/api-overview

## log buckets

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


Using sinks, you can route some or all of your logs to supported destinations or exclude log entries from being stored in Cloud Logging. 

https://cloud.google.com/logging/docs/export

### Supported destinations

https://cloud.google.com/logging/docs/export#supported-destinations

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
