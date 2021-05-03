

## Introduction

[Dataflow](https://cloud.google.com/dataflow/docs)   is a managed service for executing a wide variety of data processing patterns. The documentation on this site shows you how to deploy your batch and streaming data processing pipelines using Dataflow, including directions for using service features.



Google Cloud Dataflow makes it easy to process and analyze real-time streaming data so that you can derive insights and react to new information in real-time. Learn how it is used in conjunction with other technologies, like PubSub, Kafka, BigQuery, Bigtable, or Datastore, to build end-to-end streaming architectures. Learn how these architectures enable diverse use cases such as real-time ingestion and ETL, real-time reporting & analytics, real-time alerting, or fraud detection.

[https://www.youtube.com/watch?v=7lJyq1hw_KI](https://www.youtube.com/watch?v=7lJyq1hw_KI)

Google Cloud customers are increasingly looking to leverage streaming data (customer interactions, sales transactions, machine logs) for building new innovative features, increasing sales, and protecting against risks. AI/ML (artificial intelligence/machine learning) technologies make it possible to amp up the detection of insights in large volumes of data: insights that otherwise would be impossible to gain with manual inspection. Learn how Dataflow together with TensorFlow Extended (TFX) and Cloud AI are enabling the extraction of label and classification information from video clips and natural text, predicting probabilities and detecting anomalies, fraud, and patterns in streams of business data.

[https://www.youtube.com/watch?v=cqDBnOaS6O4](https://www.youtube.com/watch?v=cqDBnOaS6O4)


## Apache beam

The Apache Beam SDK is an open source programming model that enables you to develop both batch and streaming pipelines. You create your pipelines with an Apache Beam program and then run them on the Dataflow service. The [Apache Beam documentation](https://beam.apache.org/documentation/) provides in-depth conceptual information and reference material for the Apache Beam programming model, SDKs, and other runners.

[https://github.com/apache/beam](https://github.com/apache/beam)

Cloud Dataflow is certainly not the first big data processing engine, its not the only one available on Google Cloud Platform. For example, one alternative is to run Apache Spark in Google Cloud Dataproc Service. So, why would you choose Dataflow?
There are a few reasons :

* Serverless: We don’t have to manage computing resources. It automatically spins up and down a cluster of virtual machines while running the processing jobs. We can just focus on building the code instead of building the cluster. Apache Spark, on the other hand, requires more configuration even if it is running on Cloud Dataproc.
* Processing code is separate from the execution environment: In 2016, Google donated open-source Dataflow SDK and a set of data connectors to access Google Cloud Platform which added additional features to the Apache Beam project. We can write beam programs and run them on the local system or Cloud Dataflow service. When we look at the Dataflow documentation, it suggests the Apache Beam website for the latest version of the Software Development Kit.
* Processing batch and stream mode with the same programming model: Other Big data SDKs require different codes depending on whether data comes in batch or streaming form. On the other hand, Apache Beam addresses it with a unified programming model. Competitors like Spark are considering it but they are not quite there yet.

[https://beam.apache.org/documentation/programming-guide/](https://beam.apache.org/documentation/programming-guide/)


## Example Notebook

In this notebook, we set up your development environment and work through a simple example using the [DirectRunner](https://beam.apache.org/documentation/runners/direct/). You can explore other runners with the [Beam Capability Matrix](https://beam.apache.org/documentation/runners/capability-matrix/).

[https://colab.research.google.com/github/apache/beam/blob/master/examples/notebooks/get-started/try-apache-beam-py.ipynb](https://colab.research.google.com/github/apache/beam/blob/master/examples/notebooks/get-started/try-apache-beam-py.ipynb)


## Word Count Example

[https://beam.apache.org/get-started/wordcount-example/](https://beam.apache.org/get-started/wordcount-example/)


#### Dataflow Templates 

These Dataflow templates are an effort to solve simple, but large, in-Cloud data tasks, including data import/export/backup/restore and bulk API operations, without a development environment. The technology under the hood which makes these operations possible is the [Google Cloud Dataflow](https://cloud.google.com/dataflow/) service combined with a set of [Apache Beam](https://beam.apache.org/) SDK templated pipelines.

[https://github.com/GoogleCloudPlatform/DataflowTemplates](https://github.com/GoogleCloudPlatform/DataflowTemplates)


#### Creating a pipeline

Using the Apache Beam interactive runner with JupyterLab notebooks lets you iteratively develop pipelines, inspect your pipeline graph, and parse individual PCollections in a read-eval-print-loop (REPL) workflow. These Apache Beam notebooks are made available through [AI Platform Notebooks](https://cloud.google.com/ai-platform/notebooks/docs), a managed service that hosts notebook virtual machines pre-installed with the latest data science and machine learning frameworks.

[https://cloud.google.com/dataflow/docs/guides/interactive-pipeline-development](https://cloud.google.com/dataflow/docs/guides/interactive-pipeline-development)


## Using provided Dataflow templates

Google provides a set of [open-source](https://github.com/GoogleCloudPlatform/DataflowTemplates) Dataflow templates. 

[https://cloud.google.com/dataflow/docs/guides/templates/provided-templates](https://cloud.google.com/dataflow/docs/guides/templates/provided-templates)


## Creating Dataflow templates

Dataflow [templates](https://cloud.google.com/dataflow/docs/templates/overview) use runtime parameters to accept values that are only available during pipeline execution. To customize the execution of a templated pipeline, you can pass these parameters to functions that run within the pipeline (such as a DoFn).

To create a template from your Apache Beam pipeline, you must modify your pipeline code to support runtime parameters.

[https://cloud.google.com/dataflow/docs/guides/templates/creating-templates](https://cloud.google.com/dataflow/docs/guides/templates/creating-templates)

[https://cloud.google.com/dataflow/docs/guides/templates/running-templates](https://cloud.google.com/dataflow/docs/guides/templates/running-templates)


#### Using Dataflow Flex templates

Dataflow Flex templates use docker containers.

[https://cloud.google.com/dataflow/docs/guides/templates/using-flex-templates#python](https://cloud.google.com/dataflow/docs/guides/templates/using-flex-templates#python)


## Migrating from App  Engine Map/reduce to Dataflow

[https://cloud.google.com/dataflow/docs/guides/gae-mapreduce-migration](https://cloud.google.com/dataflow/docs/guides/gae-mapreduce-migration)

[ETL From Relational DB into BigQuery using DataFlow](https://cloud.google.com/solutions/performing-etl-from-relational-database-into-bigquery)


## Dataflow Mobile Gaming Example

[https://beam.apache.org/get-started/mobile-gaming-example/](https://beam.apache.org/get-started/mobile-gaming-example/)
