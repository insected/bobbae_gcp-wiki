

## Introduction

[Dataflow](https://cloud.google.com/dataflow/docs)   is a managed service for executing a wide variety of data processing patterns. 

Google Cloud Dataflow makes it easy to process and analyze real-time streaming data so that you can derive insights and react to new information in real-time. 

[https://www.youtube.com/watch?v=7lJyq1hw_KI](https://www.youtube.com/watch?v=7lJyq1hw_KI)



[https://www.youtube.com/watch?v=cqDBnOaS6O4](https://www.youtube.com/watch?v=cqDBnOaS6O4)


## Apache beam

The [Apache Beam](https://github.com/apache/beam)    SDK is an open source programming model that enables you to develop both batch and streaming pipelines.

You create your pipelines with an Apache Beam program and then run them on the Dataflow service. 

The [Apache Beam documentation](https://beam.apache.org/documentation/) provides in-depth conceptual information and reference material for the Apache Beam programming model, SDKs, and other runners.



Cloud Dataflow is certainly not the first big data processing engine, its not the only one available on Google Cloud Platform. For example, one alternative is to run Apache Spark in Google Cloud Dataproc Service. So, why would you choose Dataflow?
There are a few reasons :

* Serverless: We don’t have to manage computing resources
* Processing code is separate from the execution environment
* Processing batch and stream mode with the same programming model

[https://beam.apache.org/documentation/programming-guide/](https://beam.apache.org/documentation/programming-guide/)


## Example Notebook

In [this notebook]( https://colab.research.google.com/github/apache/beam/blob/master/examples/notebooks/get-started/try-apache-beam-py.ipynb  ), we set up your development environment and work through a simple example using the [DirectRunner](https://beam.apache.org/documentation/runners/direct/). You can explore other runners with the [Beam Capability Matrix](https://beam.apache.org/documentation/runners/capability-matrix/).




## Word Count Example

[https://beam.apache.org/get-started/wordcount-example/](https://beam.apache.org/get-started/wordcount-example/)


## Dataflow Templates 

The [Dataflow templates]( https://github.com/GoogleCloudPlatform/DataflowTemplates  ) are an effort to solve simple, but large, in-Cloud data tasks, including data import/export/backup/restore and bulk API operations, without a development environment. The technology under the hood which makes these operations possible is the [Google Cloud Dataflow](https://cloud.google.com/dataflow/) service combined with a set of [Apache Beam](https://beam.apache.org/) SDK templated pipelines.




## Creating a pipeline

Using the Apache Beam interactive runner with JupyterLab notebooks lets you [iteratively develop pipelines]( https://cloud.google.com/dataflow/docs/guides/interactive-pipeline-development ), inspect your pipeline graph, and parse individual PCollections in a read-eval-print-loop (REPL) workflow. These Apache Beam notebooks are made available through [AI Platform Notebooks](https://cloud.google.com/ai-platform/notebooks/docs), a managed service that hosts notebook virtual machines pre-installed with the latest data science and machine learning frameworks.




## Using provided Dataflow templates

Google [provides](  https://cloud.google.com/dataflow/docs/guides/templates/provided-templates ) a set of [open-source](https://github.com/GoogleCloudPlatform/DataflowTemplates) Dataflow templates. 




## Creating Dataflow templates

Dataflow [templates](https://cloud.google.com/dataflow/docs/templates/overview) use runtime parameters to accept values that are only available during pipeline execution. To customize the execution of a templated pipeline, you can pass these parameters to functions that run within the pipeline (such as a DoFn).

To create a template from your Apache Beam pipeline, you must modify your pipeline code to support runtime parameters.

[https://cloud.google.com/dataflow/docs/guides/templates/creating-templates](https://cloud.google.com/dataflow/docs/guides/templates/creating-templates)

[https://cloud.google.com/dataflow/docs/guides/templates/running-templates](https://cloud.google.com/dataflow/docs/guides/templates/running-templates)


## Using Dataflow Flex templates

Dataflow Flex templates use docker containers.

[https://cloud.google.com/dataflow/docs/guides/templates/using-flex-templates#python](https://cloud.google.com/dataflow/docs/guides/templates/using-flex-templates#python)


## Migrating from App  Engine Map/reduce to Dataflow

[https://cloud.google.com/dataflow/docs/guides/gae-mapreduce-migration](https://cloud.google.com/dataflow/docs/guides/gae-mapreduce-migration)

[ETL From Relational DB into BigQuery using DataFlow](https://cloud.google.com/solutions/performing-etl-from-relational-database-into-bigquery)


## Dataflow Mobile Gaming Example

[https://beam.apache.org/get-started/mobile-gaming-example/](https://beam.apache.org/get-started/mobile-gaming-example/)

## Stopping

You cannot delete a Dataflow job; you can only stop it.

https://cloud.google.com/dataflow/docs/guides/stopping-a-pipeline
