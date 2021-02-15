# Workflows

There are [many kinds of tools to implement different types of workflows](https://github.com/meirwah/awesome-workflow-engines).
Google Cloud’s first general purpose workflow orchestration tool was [Cloud Composer](https://cloud.google.com/composer).

Based on [Apache Airflow](https://airflow.apache.org/), Cloud Composer is great for data engineering pipelines like ETL orchestration, big data processing or machine learning workflows, and integrates well with data products like BigQuery or Dataflow . For example, Cloud Composer is a natural choice if your workflow needs to run a series of jobs in a data warehouse or big data cluster, and save results to a storage bucket.

However, if you want to process events or chain APIs in a serverless way—or have workloads that are bursty or latency-sensitive— it may be better to use  [Workflows](https://cloud.google.com/workflows). 

[Workflows](https://cloud.google.com/workflows) scales to zero when you’re not using it, incurring no costs when it’s idle. Pricing is based on the number of steps in the workflow, so you only pay if your workflow runs. And because Workflows doesn’t charge based on execution time, if a workflow pauses for a few hours in between tasks, you don’t pay for this either. 

Workflows scale up automatically with very low startup time and no “cold start” effect. Also, it transitions quickly between steps, supporting latency-sensitive applications. 

## Google Cloud Workflows

Orchestrate and automate Google Cloud and HTTP-based API services with [serverless workflows](https://cloud.google.com/blog/products/application-development/get-to-know-google-cloud-workflows).
 It’s fully serverless and requires no infrastructure management.

https://cloud.google.com/workflows

### Serverless Orchestration Engine
[Workflows](https://cloud.google.com/workflows) is Google Cloud's serverless orchestration engine: https://cloud.google.com/blog/products/application-development/get-to-know-google-cloud-workflows


https://cloud.google.com/community/tutorials/ml-pipeline-with-workflows


## Cloud Composer

The [Cloud Composer](https://cloud.google.com/composer) is a fully managed workflow orchestration built on [Apache Airflow](https://airflow.apache.org/). 
Google runs this open source orchestration platform on top of a Google Kubernetes Engine (GKE) cluster. 
 This cluster manages the Airflow workers, and opens up a host of integration opportunities with other Google Cloud products.
Cloud Composer lets you author workflows with a Python API, schedule them to run automatically 
or start them manually, and monitor the execution of their tasks in real time through a graphical UI.
Built-in integration with  BigQuery, Dataflow, Dataproc, Datastore, Cloud Storage, Pub/Sub, AI Platform.
During environment creation, Cloud Composer provides the following configuration options: Cloud Composer environment with a route-based GKE cluster (default), Private IP Cloud Composer environment, Cloud Composer environment with a VPC Native GKE cluster using alias IP addresses, Shared VPC.

### Automating infrastructure with Cloud Composer

This example shows how to schedule automated backups of Compute Engine virtual machine (VM) instances.

https://cloud.google.com/solutions/automating-infrastructure-using-cloud-composer


### Writing DAGs
This guide shows you how to write an Apache Airflow directed acyclic graph (DAG) that runs in a Cloud Composer environment.

https://cloud.google.com/composer/docs/how-to/using/writing-dags


## Dataproc Workflow 

The Dataproc [WorkflowTemplates](https://cloud.google.com/dataproc/docs/reference/rest/v1/projects.regions.workflowTemplates) API provides a flexible and easy-to-use mechanism for managing and executing workflows. A Workflow Template is a reusable workflow configuration. It defines a graph of jobs with information on where to run those jobs.

[Here](https://garystafford.medium.com/using-the-google-cloud-dataproc-workflowtemplates-api-to-automate-spark-and-hadoop-workloads-on-gcp-95b02f54b5f2) is a great tutorial on Dataproc workflow templates by Gary Stafford.

## 