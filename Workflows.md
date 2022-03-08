[Cloud Workflows](https://cloud.google.com/workflows) let you orchestrate and automate Google Cloud and HTTP-based API services with [serverless](Serverless) workflows.

There are [many kinds of tools](https://github.com/pditommaso/awesome-pipeline) to implement different [types of workflows](https://github.com/meirwah/awesome-workflow-engines).


Google Cloud’s first general purpose workflow orchestration tool was [Cloud Composer](composer).  Based on [Apache Airflow](https://airflow.apache.org/), Cloud Composer is great for data engineering pipelines like ETL orchestration, big data processing or machine learning workflows, and integrates well with data products like [BigQuery](BigQuery) or [Dataflow](Dataflow). Cloud [Composer](Composer) is a natural choice if your workflow needs to run a series of jobs in a data warehouse or big data cluster, and save results to a storage bucket.

If you want to process events or chain APIs in a [serverless](Serverless) way, or have workloads that are bursty or latency-sensitive, it may be better to use  [Workflows](https://cloud.google.com/workflows).

https://cloud.google.com/blog/products/application-development/get-to-know-google-cloud-workflows


## Orchestration vs Choreography

Google Cloud provides services supporting both [Orchestration and Choreography approaches](https://cloud.google.com/blog/topics/developers-practitioners/better-service-orchestration-workflows). 

[Pub/Sub](https://cloud.google.com/pubsub) and [Eventarc](Eventarc)  are both suited for choreography of event-driven services, whereas Workflows is suited for [centrally orchestrated services](https://cloud.google.com/blog/topics/developers-practitioners/better-service-orchestration-workflows). 

[Workflows](http://cloud.google.com/workflows) is a service to orchestrate not only Google Cloud services, such as Cloud Functions and Cloud Run, but also external services. Should there be a central orchestrator controlling all interactions between services or should each service work independently and only interact through events? This is the central question in Orchestration vs Choreography debate. 

In Orchestration, a central service defines and controls the flow of communication between services. With centralization, it becomes easier to change and monitor the flow and apply consistent timeout and error policies. 

In Choreography, each service registers for and emits events as they need. There’s usually a central event broker to pass messages around, but it does not define or direct the flow of communication. This allows services that are truly independent at the expense of less traceable and manageable flow and policies. 


## Connectors

Workflows publishes [connectors](https://cloud.google.com/workflows/docs/connectors) to make it easier to access other Google Cloud products within a workflow.  Connectors can be used to connect to other Google Cloud APIs within a workflow, helping you integrate your workflows with other Google Cloud products. For example, you can use connectors to publish Pub/Sub messages, read or write data to a [Firestore](Firestore) database, or retrieve authentication keys from [Secret Manager](Secret-Manager).

https://cloud.google.com/workflows/docs/reference/googleapis

### Connectors Samples 

https://cloud.google.com/workflows/docs/connectors-samples

### Connectors Workflows Samples on github

https://github.com/GoogleCloudPlatform/workflows-samples/tree/main/src/connectors

### Connectors Workflows demos

https://github.com/GoogleCloudPlatform/workflows-demos/tree/master/connector-compute

### Callbacks

https://cloud.google.com/blog/topics/developers-practitioners/introducing-workflows-callbacks

### Replicate data from BigQuery to Cloud SQL using Cloud Workflows

https://medium.com/google-cloud/replicate-data-from-bigquery-to-cloud-sql-2b23a08c52b1

## Other tools related to workflows

### Google Cloud Composer

The [Cloud Composer](https://cloud.google.com/composer) is a fully managed workflow orchestration built on [Apache Airflow](https://airflow.apache.org/). 

### Google Dataproc Workflow 

The [Dataproc](DataProc) [WorkflowTemplates](https://cloud.google.com/dataproc/docs/reference/rest/v1/projects.regions.workflowTemplates) API provides a flexible and easy-to-use mechanism for managing and executing workflows. A Workflow Template is a reusable workflow configuration. It defines a graph of jobs with information on where to run those jobs.

https://garystafford.medium.com/using-the-google-cloud-dataproc-workflowtemplates-api-to-automate-spark-and-hadoop-workloads-on-gcp-95b02f54b5f2

### Dataflow

[Dataflow](Dataflow)  is a managed service for executing a wide variety of data processing patterns. 


### Kubeflow & AI Hub

[Kubeflow](Kubeflow) Pipelines is a platform for building and deploying portable, scalable machine learning (ML) workflows based on containers.
[AI Hub](AI-Hub) has support for [Kubeflow](Kubeflow) Pipelines.


### Workflow Tools Comparison and Alternatives

A [survey of pipeline & workflow tools](https://github.com/pditommaso/awesome-pipeline).

### Choosing the right Orchestrator for Google Cloud

Orchestration often refers to the automated configuration, coordination, and management of computer systems and services. 

In the context of service-oriented architectures, orchestration can range from executing a single service at a specific time and day, to a more sophisticated approach of automating and monitoring multiple services over longer periods of time, with the ability to react and handle failures as they crop up. In the data engineering context, orchestration is central to coordinating the services and workflows that prepare, ingest, and transform data. It can go beyond data processing and also involve a workflow to train a machine learning (ML) model from the data.

Google Cloud Platform offers a number of tools and services for orchestration:

* [Cloud Scheduler](Cloud-Scheduler) for schedule driven single-service orchestration
* [Workflows](https://cloud.google.com/workflows) for complex multi-service orchestration 
* [Cloud Composer](Composer) for orchestration of your data workloads


https://cloud.google.com/blog/topics/developers-practitioners/choosing-right-orchestrator-google-cloud

### Saga pattern to deal with failures in Workflows

https://cloud.google.com/blog/topics/developers-practitioners/implementing-saga-pattern-workflows

### Send email using Sendgrid in Workflows

https://glaforge.appspot.com/article/sending-an-email-with-sendgrid-from-workflows

### Loading JSON data from GCS in Workflows

https://glaforge.appspot.com/article/load-and-use-json-data-in-your-workflow-from-gcs

### Using Secret Manager Connector for Workflows

https://glaforge.appspot.com/article/using-the-secret-manager-connector-for-workflows-to-call-an-authenticated-service

### Data Orchestration using Workflows

https://medium.com/datatonic/lightweight-data-orchestration-using-cloud-workflows-and-dataform-52f3bc5203d3


### Airflow vs. Luigi vs. Argo vs. MLFlow vs. Kubeflow

[Review the comparisons of Airflow, Luigi, Argo, MLflow and Kubeflow](https://www.datarevenue.com/en-blog/airflow-vs-luigi-vs-argo-vs-mlflow-vs-kubeflow)

### Prefect

https://github.com/PrefectHQ/prefect


### Snakemake

https://github.com/snakemake/snakemake

### Visual Editor

https://medium.com/@kolban1/gcp-workflows-visual-editor-9876fb1c823f


### Bioinformatics workflow tools

https://github.com/danielecook/Awesome-Bioinformatics#workflow-managers



### Pipelines


https://github.com/pditommaso/awesome-pipeline



### Using Makefile for workflows

https://blog.sellorm.com/2018/06/02/first-steps-with-data-pipelines/

#### Make map reduce pipeline

https://www.benevolent.com/engineering-blog/make-reduce-how-to-use-makefiles-to-run-a-simple-map-reduce-data-pipeline


#### Reproducibility with Make

https://the-turing-way.netlify.app/reproducible-research/make.html

#### Make tutorial

https://github.com/kyclark/make-tutorial

#### Parallel


https://www.gnu.org/software/parallel/


## Examples

### Use GCP Workflows to load data from GCS to BigQuery


https://cloud.google.com/architecture/serverless-orchestration-loading-data-from-cloud-storage-to-biquery-using-workflows


### Reading and writing JSON file from a Workflow

https://medium.com/google-cloud/day-16-with-workflows-reading-in-and-writing-a-json-file-to-a-storage-bucket-from-a-workflow-48b85c12d225

### ML Pipelines with Workflows

https://cloud.google.com/community/tutorials/ml-pipeline-with-workflows


### Large-scale bioinformatics in the cloud with GCP, Kubernetes and Snakemake

Perform a [large metagenomics sequencing experiment – 96 10X Genomics linked read libraries sequenced across 25 lanes on a HiSeq4000](https://www.bsiranosian.com/bioinformatics/large-scale-bioinformatics-in-the-cloud-with-gcp-kubernetes-and-snakemake/) in GCP.

### Cromwell

https://medium.com/google-cloud/cromwell-hello-gcp-833c18df3caf

### Analyzing Twitter sentiment 

https://cloud.google.com/blog/topics/developers-practitioners/analyzing-twitter-sentiment-new-workflows-processing-capabilities
