

Cloud [Composer](https://cloud.google.com/composer/) is a managed [Apache Airflow](https://airflow.apache.org/) service that helps you create, schedule, monitor and manage [workflows](Workflows). 

[Cloud Composer](   https://cloud.google.com/composer/docs ) automation helps you create Airflow environments quickly and use Airflow-native tools, such as the powerful Airflow web interface and command line tools, so you can focus on your workflows and not your infrastructure.



[Cloud Composer](  https://www.youtube.com/watch?v=bwZOAXnCMf8 ) is a managed workflow orchestration service built on Apache Airflow. 


Google runs this open source orchestration platform on top of a Google Kubernetes Engine (GKE) cluster. 

This cluster manages the Airflow workers, and opens up a host of integration opportunities with other Google Cloud products.




Environments are a core concept in Cloud Composer. You can create one or more Cloud Composer environments inside of a project. 

Environments are self-contained Airflow deployments based on Google Kubernetes Engine. 

These environments work with Google Cloud services through connectors that are built into Airflow. You create Cloud Composer environments in [supported regions](https://cloud.google.com/about/locations), and the environments run within a Compute Engine zone. 

For simple use cases, you can create one environment in one region. For complex use cases, you can create multiple environments within a single region or across multiple regions. 

Airflow communicates with other Google Cloud products through the products' public APIs.


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


## Tutorials

[https://cloud.google.com/composer/docs/tutorials](https://cloud.google.com/composer/docs/tutorials)



# Apache Airflow 

[Airflow](https://airflow.apache.org/) is a platform to programmatically author, schedule and monitor workflows.

Use Airflow to author workflows as Directed Acyclic Graphs (DAGs) of tasks. The Airflow scheduler executes your tasks on an array of workers while following the specified dependencies. 

[Rich command line utilities make performing complex surgeries on DAGs a snap](. The rich user interface makes it easy to visualize pipelines running in production, monitor progress, and troubleshoot issues when needed. 

Airflow is a micro-service architected framework. To deploy Airflow in a distributed setup, Cloud Composer provisions several Google Cloud components, which are collectively known as a Cloud Composer environment.

## Automating infrastructure using Airflow

Stop VM, take snapshots, start VMs, using python API and airflow.   Each step is put into an operator.  Collection of operators are put into a Plugin.  DAGs are composed of each step operator put into a pipeline. DAGs and Plugins are copied into Cloud Storage and run as Cloud Composer jobs.

[https://cloud.google.com/solutions/automating-infrastructure-using-cloud-composer](https://cloud.google.com/solutions/automating-infrastructure-using-cloud-composer)





## Concepts

[https://airflow.apache.org/docs/stable/concepts.html](https://airflow.apache.org/docs/stable/concepts.html)


## Apache Airflow for Beginners

[https://www.youtube.com/watch?v=YWtfU0MQZ_4](https://www.youtube.com/watch?v=YWtfU0MQZ_4)


## Developing workflows with Apache Airflow

[http://michal.karzynski.pl/blog/2017/03/19/developing-workflows-with-apache-airflow/](http://michal.karzynski.pl/blog/2017/03/19/developing-workflows-with-apache-airflow/)


## Operators

 An [Operator](  https://github.com/apache/airflow/tree/master/airflow/operators ) is an atomic block of workflow logic, which performs a single action. Operators are written as Python classes (subclasses of BaseOperator), where the __init__ function can be used to configure settings for the task and a method named execute is called when the task instance is executed.




### XCom

[https://airflow.apache.org/docs/stable/concepts.html#xcoms](https://airflow.apache.org/docs/stable/concepts.html#xcoms)

## Industrialization of a Machine Learning model using Apache Airflow and Apache BEAM.

[https://medium.com/swlh/industrialization-of-a-ml-model-using-airflow-and-apache-beam-5a5338f20184](https://medium.com/swlh/industrialization-of-a-ml-model-using-airflow-and-apache-beam-5a5338f20184)




