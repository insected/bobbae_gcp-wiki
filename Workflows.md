

There are [many kinds of tools](https://github.com/pditommaso/awesome-pipeline) to implement different [types of workflows](https://github.com/meirwah/awesome-workflow-engines).


Google Cloud’s first general purpose workflow orchestration tool was [Cloud Composer](https://cloud.google.com/composer).

Based on [Apache Airflow](https://airflow.apache.org/), Cloud Composer is great for data engineering pipelines like ETL orchestration, big data processing or machine learning workflows, and integrates well with data products like BigQuery or Dataflow. 

For example, Cloud [Composer](Composer) is a natural choice if your workflow needs to run a series of jobs in a data warehouse or big data cluster, and save results to a storage bucket.




# Google Cloud Workflows

However, if you want to process events or chain APIs in a serverless way—or have workloads that are bursty or latency-sensitive— it may be better to use  [Workflows](https://cloud.google.com/workflows).



[Workflows](https://cloud.google.com/workflows) is Google Cloud's serverless orchestration engine: https://cloud.google.com/blog/products/application-development/get-to-know-google-cloud-workflows


https://cloud.google.com/community/tutorials/ml-pipeline-with-workflows

[Workflows](https://cloud.google.com/workflows) scales to zero when you’re not using it, incurring no costs when it’s idle. 

It is a [Serverless Orchestration Engine](https://codelabs.developers.google.com/codelabs/cloud-workflows-intro) and requires no infrastructure management.


Pricing is based on the number of steps in the workflow, so you only pay if your workflow runs. And because Workflows doesn’t charge based on execution time, if a workflow pauses for a few hours in between tasks, you don’t pay for this either. 

Workflows scale up automatically with very low startup time and no “cold start” effect. Also, it transitions quickly between steps, supporting latency-sensitive applications. 



You can orchestrate and automate Google Cloud and HTTP-based API services with [serverless workflows](https://cloud.google.com/blog/products/application-development/get-to-know-google-cloud-workflows).

## Orchestration vs Choreography

Should there be a central orchestrator controlling all interactions between services or should each service work independently and only interact through events? This is the central question in Orchestration vs Choreography debate. 

In Orchestration, a central service defines and controls the flow of communication between services. With centralization, it becomes easier to change and monitor the flow and apply consistent timeout and error policies. 

In Choreography, each service registers for and emits events as they need. There’s usually a central event broker to pass messages around, but it does not define or direct the flow of communication. This allows services that are truly independent at the expense of less traceable and manageable flow and policies. 

Google Cloud provides services supporting both Orchestration and Choreography approaches. [Pub/Sub](https://cloud.google.com/pubsub) and [Eventarc](https://cloud.google.com/blog/topics/developers-practitioners/eventarc-unified-eventing-experience-google-cloud)  are both suited for choreography of event-driven services, whereas Workflows is suited for [centrally orchestrated services](https://cloud.google.com/blog/topics/developers-practitioners/better-service-orchestration-workflows). 


## Connectors

Workflows publishes [connectors](https://cloud.google.com/workflows/docs/connectors) to make it easier to access other Google Cloud products within a workflow. 

For a detailed reference of available connectors, see the Connectors reference. For workflow samples that demonstrate how to use a connector, see [Connectors Samples](https://cloud.google.com/workflows/docs/connectors-samples), [github Workflows demo repo](https://github.com/GoogleCloudPlatform/workflows-demos/tree/master/connector-compute) and [Workflows samples](https://github.com/GoogleCloudPlatform/workflows-samples/tree/main/src/connectors).

Connectors can be used to connect to other Google Cloud APIs within a workflow, helping you integrate your workflows with other Google Cloud products. 

For example, you can use connectors to publish Pub/Sub messages, read or write data to a Firestore database, or retrieve authentication keys from Secret Manager.

# Google Cloud Composer


The [Cloud Composer](https://cloud.google.com/composer) is a fully managed workflow orchestration built on [Apache Airflow](https://airflow.apache.org/). 

 






# Google Dataproc Workflow 



The [Dataproc](DataProc) [WorkflowTemplates](https://cloud.google.com/dataproc/docs/reference/rest/v1/projects.regions.workflowTemplates) API provides a flexible and easy-to-use mechanism for managing and executing workflows. 

A Workflow Template is a reusable workflow configuration. It defines a graph of jobs with information on where to run those jobs.

[Check out](https://garystafford.medium.com/using-the-google-cloud-dataproc-workflowtemplates-api-to-automate-spark-and-hadoop-workloads-on-gcp-95b02f54b5f2) is a great tutorial on Dataproc workflow templates by Gary Stafford.

# [Kubeflow](Kubeflow) & [AI Hub](AI-Hub)


[Kubeflow](Kubeflow) Pipelines is a platform for building and deploying portable, scalable machine learning (ML) workflows based on containers.
[AI Hub](AI-Hub) has support for [Kubeflow](Kubeflow) Pipelines.


# Workflow Tools Comparison and Alternatives

A [survey of pipeline & workflow tools](https://github.com/pditommaso/awesome-pipeline).

## Choosing the right Orchestrator for Google Cloud

Orchestration often refers to the automated configuration, coordination, and management of computer systems and services. 

In the context of service-oriented architectures, orchestration can range from simply executing a single service at a specific time and day, to a more sophisticated approach of automating and monitoring multiple services over longer periods of time, with the ability to react and handle failures as they crop up. 

In the data engineering context, orchestration is central to coordinating the services and workflows that prepare, ingest, and transform data. It can go beyond data processing and also involve a workflow to train a machine learning (ML) model from the data.

Google Cloud Platform offers a number of tools and services for orchestration:

* [Cloud Scheduler](Cloud-Scheduler) for schedule driven single-service orchestration
* Workflows for complex multi-service orchestration 
* [Cloud Composer](Composer) for orchestration of your data workloads

<img src="https://storage.googleapis.com/gweb-cloudblog-publish/images/Screen_Shot_2021-04-21_at_9.45.28_AM.max-1000x1000.png" width="600">

https://cloud.google.com/blog/topics/developers-practitioners/choosing-right-orchestrator-google-cloud


## Airflow vs. Luigi vs. Argo vs. MLFlow vs. Kubeflow

[Review the comparisons of Airflow, Luigi, Argo, MLflow and Kubeflow](https://www.datarevenue.com/en-blog/airflow-vs-luigi-vs-argo-vs-mlflow-vs-kubeflow)


