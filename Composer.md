

Cloud [Composer](https://cloud.google.com/composer/) is a managed [Apache Airflow](https://airflow.apache.org/) service that helps you create, schedule, monitor and manage [workflows](Workflows). 

[Cloud Composer](   https://cloud.google.com/composer/docs ) automation helps you [create Airflow environment](https://cloud.google.com/composer/docs/how-to/managing/creating)s quickly and use Airflow-native tools, such as the powerful Airflow web interface and command line tools.


[Cloud Composer](  https://www.youtube.com/watch?v=bwZOAXnCMf8 ) is a [managed workflow orchestration service](https://cloud.google.com/blog/products/data-analytics/cloud-composer-is-now-in-beta-build-and-run-practical-workflows-with-minimal-effort
) built on [Apache Airflow](https://airflow.apache.org/). 


Google runs this open source orchestration platform on top of a Google Kubernetes Engine (GKE) cluster. 

This cluster manages the Airflow workers, and opens up a host of integration opportunities with other Google Cloud products.


## Environment

[Environment](https://cloud.google.com/composer/docs/concepts/architecture) is a core concept in Cloud Composer. 

You can create one or more Cloud Composer environments inside of a project. 

Environments are self-contained Airflow deployments based on Google Kubernetes Engine which can [scale](https://cloud.google.com/composer/docs/environment-scaling).  You can scale composer environments by adjusting [number of nodes or schedulers](https://cloud.google.com/composer/docs/scale-environments).

These environments work with Google Cloud services through connectors that are built into Airflow. You create Cloud Composer environments in [supported regions](https://cloud.google.com/about/locations), and the environments run within a Compute Engine zone. 

For simple use cases, you can create one environment in one region. For complex use cases, you can create multiple environments within a single region or across multiple regions. 

Airflow communicates with other Google Cloud products through the products' public APIs.

### Airflow 2 vs 1

https://dsstream.com/differences-between-airflow-1-10-x-and-2-0/

### Airflow 2 development environment on GCP Cloud Shell

https://medium.com/badal-io/airflow-2-development-environment-on-gcp-cloud-shell-5534b829e19a

### Composer 2 GKE Autopilot Environment


https://cloud.google.com/composer/docs/composer-2/environment-architecture

## Integration with Other GCP Services 

Cloud Composer lets you author workflows with a Python API, schedule them to run automatically 
or start them manually, and monitor the execution of their tasks in real time through a graphical UI.

Built-in integration with  BigQuery, Dataflow, Dataproc, Datastore, Cloud Storage, Pub/Sub, AI Platform.

During environment creation, Cloud Composer provides the following configuration options: Cloud Composer environment with a route-based GKE cluster (default), Private IP Cloud Composer environment, Cloud Composer environment with a VPC Native GKE cluster using alias IP addresses, Shared VPC.

## Writing DAGs


https://cloud.google.com/composer/docs/how-to/using/writing-dags

## Data Pipelines with Cloud Composer

[https://www.youtube.com/watch?v=GeNFEtt-D4k](https://www.youtube.com/watch?v=GeNFEtt-D4k)


## Cloud Composer best practices

[https://www.youtube.com/watch?v=RrKXZcKOz4A](https://www.youtube.com/watch?v=RrKXZcKOz4A)

## Tuning

https://mkuthan.github.io/blog/2022/03/15/gcp-cloud-composer-tuning/

## Tutorials

[https://cloud.google.com/composer/docs/tutorials](https://cloud.google.com/composer/docs/tutorials)



# Apache Airflow 

[Airflow](https://airflow.apache.org/) is a platform to programmatically author, schedule and monitor workflows.

Use Airflow to author workflows as Directed Acyclic Graphs (DAGs) of tasks. The Airflow scheduler executes your tasks on an array of workers while following the specified dependencies. 

[Rich command line utilities make performing complex surgeries on DAGs a snap](   https://towardsdatascience.com/airflow-how-and-when-to-use-it-2e07108ac9f5   ). The rich user interface makes it easy to visualize pipelines running in production, monitor progress, and troubleshoot issues when needed. 

Airflow is a micro-service architected framework. To deploy Airflow in a distributed setup, Cloud Composer provisions several Google Cloud components, which are collectively known as a Cloud Composer environment.

## Automating infrastructure using Airflow

Stop VM, take snapshots, start VMs, using python API and airflow.   Each step is put into an operator.  Collection of operators are put into a Plugin.  DAGs are composed of each step operator put into a pipeline. DAGs and Plugins are copied into Cloud Storage and run as Cloud Composer jobs.

[https://cloud.google.com/solutions/automating-infrastructure-using-cloud-composer](https://cloud.google.com/solutions/automating-infrastructure-using-cloud-composer)





## Airflow Concepts

[https://airflow.apache.org/docs/stable/concepts.html](https://airflow.apache.org/docs/stable/concepts.html)


## Apache Airflow for Beginners

[https://www.youtube.com/watch?v=YWtfU0MQZ_4](https://www.youtube.com/watch?v=YWtfU0MQZ_4)


## Developing workflows with Apache Airflow

[http://michal.karzynski.pl/blog/2017/03/19/developing-workflows-with-apache-airflow/](http://michal.karzynski.pl/blog/2017/03/19/developing-workflows-with-apache-airflow/)


## Airflow Operators

 An [Operator](  https://github.com/apache/airflow/tree/master/airflow/operators ) is an atomic block of workflow logic, which performs a single action. Operators are written as Python classes (subclasses of BaseOperator), where the __init__ function can be used to configure settings for the task and a method named execute is called when the task instance is executed.




### Airflow XCom

[https://airflow.apache.org/docs/stable/concepts.html#xcoms](https://airflow.apache.org/docs/stable/concepts.html#xcoms)

## Industrialization of a Machine Learning model using Apache Airflow and Apache BEAM.

[https://medium.com/swlh/industrialization-of-a-ml-model-using-airflow-and-apache-beam-5a5338f20184](https://medium.com/swlh/industrialization-of-a-ml-model-using-airflow-and-apache-beam-5a5338f20184)

## Airflow Executors and Issues

https://medium.com/flyr-labs-blog/why-were-switching-off-airflow-sort-of-780c4f58a660

## Composer vs Astronomer

https://itsvit.com/blog/google-cloud-composer-vs-astronomer-what-to-choose/

## Airflow alternatives

https://towardsdatascience.com/why-you-should-try-something-else-than-airflow-for-data-pipeline-orchestration-7a0a2c91c341


## Examples

### Setup Apache Airflow in Multiple Nodes in Google Cloud Platform


https://medium.com/data-folks-indonesia/setup-apache-airflow-in-multiple-nodes-in-google-cloud-platform-cdc33591d002

### Automating infrastructure with Cloud Composer


https://cloud.google.com/architecture/automating-infrastructure-using-cloud-composer

### Launching Dataflow pipelines with Cloud Composer

https://cloud.google.com/composer/docs/how-to/using/using-dataflow-template-operator

### Health checking your Cloud Composer environment

https://cloud.google.com/composer/docs/tutorials/health-check

### Setting up a CI/CD for your data processing workflow

https://cloud.google.com/architecture/cicd-pipeline-for-data-processing

### Dataproc workflow using Cloud Composer

https://cloud.google.com/dataproc/docs/tutorials/workflow-composer

### Use case LoveHolidays.com

https://tech.loveholidays.com/out-of-the-data-tar-pit-how-loveholidays-escaped-from-a-legacy-reporting-system-and-kept-the-data-331c5e1f0ee2

### Composing invoking long-running services

https://medium.com/@kolban1/composer-invoking-long-running-services-4de2dfa5e33a

### Sendgrid and Secrets

https://medium.com/google-cloud/composer-sendgrid-and-secrets-75e4b6e7581e

## Qwiklabs

### GSP283

Cloud Composer: [Copying BigQuery Tables Across Different Locations](https://cloud.google.com/blog/products/data-analytics/how-to-transfer-bigquery-tables-between-locations-with-cloud-composer
)


https://www.qwiklabs.com/focuses/3528?parent=catalog

Note that creating Composer Environment will allocate VMs, create Kubernetes cluster on them, create Cloud Storage bucket (named in a pattern as in region-composer-env-name-number) where the DAGs and code are stored. Creation of Composer environment can take a while and deleting the Environment afterwards will clean up most of the resources, including the VMs and Kubernetes clusters. But they will not delete the BigQuery data created as a result. Deleting Composer Environment also does not delete the auto-created GCS bucket. It has do be deleted manually.
