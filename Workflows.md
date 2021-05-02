

There are [many kinds of tools](https://github.com/pditommaso/awesome-pipeline) to implement different [types of workflows](https://github.com/meirwah/awesome-workflow-engines).


Google Cloud’s first general purpose workflow orchestration tool was [Cloud Composer](https://cloud.google.com/composer).

Based on [Apache Airflow](https://airflow.apache.org/), Cloud Composer is great for data engineering pipelines like ETL orchestration, big data processing or machine learning workflows, and integrates well with data products like BigQuery or Dataflow. 

For example, Cloud Composer is a natural choice if your workflow needs to run a series of jobs in a data warehouse or big data cluster, and save results to a storage bucket.


https://github.com/bobbae/gcp/wiki/Composer

# Google Cloud Workflows

However, if you want to process events or chain APIs in a serverless way—or have workloads that are bursty or latency-sensitive— it may be better to use  [Workflows](https://cloud.google.com/workflows).


[Workflows](https://cloud.google.com/workflows) scales to zero when you’re not using it, incurring no costs when it’s idle. 

It is a Serverless Orchestration Engine.


Pricing is based on the number of steps in the workflow, so you only pay if your workflow runs. And because Workflows doesn’t charge based on execution time, if a workflow pauses for a few hours in between tasks, you don’t pay for this either. 

Workflows scale up automatically with very low startup time and no “cold start” effect. Also, it transitions quickly between steps, supporting latency-sensitive applications. 



You can orchestrate and automate Google Cloud and HTTP-based API services with [serverless workflows](https://cloud.google.com/blog/products/application-development/get-to-know-google-cloud-workflows).

It’s fully serverless and requires no infrastructure management.

https://cloud.google.com/workflows

## Serverless Orchestration Engine

[Workflows](https://cloud.google.com/workflows) is Google Cloud's serverless orchestration engine: https://cloud.google.com/blog/products/application-development/get-to-know-google-cloud-workflows


https://cloud.google.com/community/tutorials/ml-pipeline-with-workflows

## Connectors

Workflows publishes [connectors](https://cloud.google.com/workflows/docs/connectors) to make it easier to access other Google Cloud products within a workflow. 

For a detailed reference of available connectors, see the Connectors reference. For workflow samples that demonstrate how to use a connector, see [Connectors Samples](https://cloud.google.com/workflows/docs/connectors-samples).

Connectors can be used to connect to other Google Cloud APIs within a workflow, helping you integrate your workflows with other Google Cloud products. 

For example, you can use connectors to publish Pub/Sub messages, read or write data to a Firestore database, or retrieve authentication keys from Secret Manager.

# Google Cloud Composer

https://github.com/bobbae/gcp/wiki/Composer

The [Cloud Composer](https://cloud.google.com/composer) is a fully managed workflow orchestration built on [Apache Airflow](https://airflow.apache.org/). 

 

## Automating infrastructure with Cloud Composer

This example shows how to schedule automated backups of Compute Engine virtual machine (VM) instances.

https://cloud.google.com/solutions/automating-infrastructure-using-cloud-composer




# Google Dataproc Workflow 

https://github.com/bobbae/gcp/wiki/Dataproc

The Dataproc [WorkflowTemplates](https://cloud.google.com/dataproc/docs/reference/rest/v1/projects.regions.workflowTemplates) API provides a flexible and easy-to-use mechanism for managing and executing workflows. 

A Workflow Template is a reusable workflow configuration. It defines a graph of jobs with information on where to run those jobs.

[Here](https://garystafford.medium.com/using-the-google-cloud-dataproc-workflowtemplates-api-to-automate-spark-and-hadoop-workloads-on-gcp-95b02f54b5f2) is a great tutorial on Dataproc workflow templates by Gary Stafford.

# Kubeflow & AI Hub

ML workflows tools.

https://github.com/bobbae/gcp/wiki/Kubeflow

https://github.com/bobbae/gcp/wiki/AI-Hub

# Workflow Tools Comparison and Alternatives

A survey of pipeline & workflow tools.

[https://github.com/pditommaso/awesome-pipeline](https://github.com/pditommaso/awesome-pipeline)

## Airflow vs. Luigi vs. Argo vs. MLFlow vs. KubeFlow

[https://www.datarevenue.com/en-blog/airflow-vs-luigi-vs-argo-vs-mlflow-vs-kubeflow](https://www.datarevenue.com/en-blog/airflow-vs-luigi-vs-argo-vs-mlflow-vs-kubeflow)


