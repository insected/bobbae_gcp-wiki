
### GKE Basics

[Kubernetes in Google Cloud](https://www.qwiklabs.com/quests/29?catalog_rank=%7B%22rank%22%3A1%2C%22num_filters%22%3A1%2C%22has_search%22%3Atrue%7D&search_id=7467715)


### GKE Solutions

Containerized applications have changed the game and are here to stay. With Kubernetes, you can orchestrate containers with ease, and integration with the Google Cloud Platform is seamless. In this advanced-level quest, you will be exposed to a wide range of Kubernetes use cases and will get hands-on practice architecting solutions over the course of 8 labs. From building Slackbots with NodeJS, to deploying game servers on clusters, to running the Cloud Vision API, Kubernetes Solutions will show you first-hand how agile and powerful this container orchestration system is.

[Kubernetes Solutions](https://www.qwiklabs.com/quests/45?catalog_rank=%7B%22rank%22%3A2%2C%22num_filters%22%3A1%2C%22has_search%22%3Atrue%7D&search_id=7467715)


##### GKE Deploy

Kubernetes is the most popular container orchestration system, and Google Kubernetes Engine was designed specifically to support managed Kubernetes deployments in Google Cloud. In this advanced-level quest, you will get hands-on practice configuring Docker images, containers, and deploying fully-fledged Kubernetes Engine applications. This quest will teach you the practical skills needed for integrating container orchestration into your own workflow. 

[Deploy to Kubernetes in Google Cloud](https://www.qwiklabs.com/quests/116?catalog_rank=%7B%22rank%22%3A3%2C%22num_filters%22%3A1%2C%22has_search%22%3Atrue%7D&search_id=7467715)


### Security in GKE

The following hands-on labs focus on [security at scale](https://cloud.google.com/anthos/docs/concepts/anthos-overview#service_management) when deploying and managing production GKE environments -- specifically role-based access control, hardening, VPC networking, and binary authorization. 

[Secure Workloads in Google Kubernetes Engine](https://www.qwiklabs.com/quests/142?catalog_rank=%7B%22rank%22%3A4%2C%22num_filters%22%3A1%2C%22has_search%22%3Atrue%7D&search_id=7467715)

[Google Kubernetes Engine Best Practices: Security](https://www.qwiklabs.com/quests/64?catalog_rank=%7B%22rank%22%3A5%2C%22num_filters%22%3A1%2C%22has_search%22%3Atrue%7D&search_id=7467715)


##### Deploying Python Apps on GKE

Google Kubernetes Engine provides a managed environment for deploying, managing, and scaling your containerized applications using Google infrastructure. The environment Kubernetes Engine provides consists of multiple machines (specifically, Compute Engine instances) grouped together to form a cluster. Kubernetes provides the mechanisms through which you interact with your cluster. You use Kubernetes commands and resources to deploy and manage your applications, perform administration tasks and set policies, and monitor the health of your deployed workloads. In this lab, you deploy the Quiz application into Kubernetes Engine, leveraging Google Cloud resources, including Container Builder and Container Registry, and Kubernetes resources, such as Deployments, Pods, and Services.

[App Dev: Deploying the Application into Kubernetes Engine - Python](https://www.qwiklabs.com/focuses/1073?catalog_rank=%7B%22rank%22%3A30%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&parent=catalog&search_id=7467972)


### Cloud Logging on GKE

Cloud Logging can be used aggregate logs from all Google Cloud resources, as well as any custom resources on other platforms, to allow for one centralized store for all logs and metrics. Logs are aggregated and then viewable within the provided Cloud Logging UI. They can also be [exported to Sinks](https://cloud.google.com/logging/docs/export/configure_export_v2) to support more specialized use cases. Currently, Cloud Logging supports exporting to the following sinks:



*   Cloud Storage
*   Pub/Sub
*   BigQuery

In this lab you will deploy a sample application to Kubernetes Engine that forwards log events to [Cloud Logging](https://cloud.google.com/logging/) using [Terraform](https://www.terraform.io/), a declarative [Infrastructure as Code](https://en.wikipedia.org/wiki/Infrastructure_as_Code) tool that enables configuration files to automate the deployment and evolution of infrastructure in the cloud. The configuration will also create a Cloud Storage bucket and a BigQuery dataset for exporting log data to. This lab was created by GKE Helmsman engineers to give you a better understanding of Cloud Logging. You can view this demo on Github [here](https://github.com/GoogleCloudPlatform/gke-binary-auth-demo.git). 

[Cloud Logging on Kubernetes Engine](https://www.qwiklabs.com/focuses/10910?catalog_rank=%7B%22rank%22%3A10%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&parent=catalog&search_id=7468028)


### Migrating to GKE

Containers are quickly becoming an industry standard for deployment of software applications. The business and technological advantages of containerized workloads are driving many teams towards moving their applications to containers. This lab provides a basic walkthrough of migrating a stateless application from running on a VM to running on [Kubernetes Engine (GKE)](https://cloud.google.com/kubernetes-engine/). It demonstrates the lifecycle of an application transitioning from a typical VM/OS-based deployment to a specialized os for containers to a platform for containers better known as [GKE](https://cloud.google.com/kubernetes-engine/).

[Migrating to GKE Containers](https://www.qwiklabs.com/focuses/12768?catalog_rank=%7B%22rank%22%3A7%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&parent=catalog&search_id=7467835)


##### Java Application Development

In this advanced-level quest, you will learn the ins and outs of developing GCP applications in Java. The first labs will walk you through the basics of environment setup and application data storage with Cloud Datastore. Once you have a handle on the fundamentals, you will get hands-on practice deploying Java applications on Kubernetes and App Engine (the latter is the same framework that powers Snapchat!) With specialized bonus labs that teach user authentication and backend service development, this quest will give you practical experience so you can start developing robust Java applications straight away.

[Application Development - Java](https://www.qwiklabs.com/quests/42?catalog_rank=%7B%22rank%22%3A1%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&search_id=7467936)


### Operations Suite on GKE

In this fundamental-level quest, you will learn the ins and outs of Google Cloud's operations suite running on Google Kubernetes Engine, an important service for generating insights into the health of your applications. It provides a wealth of information in application monitoring, report logging, and diagnoses. The labs in this quest will give you hands-on practice with and will teach you how to monitor virtual machines, generate logs and alerts, and create custom metrics for application data.

[Google Cloud's Operations Suite on GKE](https://www.qwiklabs.com/quests/133?catalog_rank=%7B%22rank%22%3A5%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&search_id=7468028)


##### Deploy Kubernetes Load Balancer with Terraform

In Terraform, a Provider is the logical abstraction of an upstream API. This lab will show you how to set up a Kubernetes cluster and deploy a Load Balancer type NGINX service on it.

A favorite lab.

[https://www.qwiklabs.com/focuses/1205?parent=catalog](https://www.qwiklabs.com/focuses/1205?parent=catalog)


