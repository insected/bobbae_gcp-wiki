

## Hybrid and Multi-cloud

<img src="https://cloud.google.com/anthos/images/anthos-arch.svg" width="800">

### Anthos

Anthos is a modern application management platform that provides a consistent development and operations experience for cloud and on-premises environments. This page provides an overview of each layer of the Anthos infrastructure and shows how you can leverage its features.

[https://cloud.google.com/anthos/docs](https://cloud.google.com/anthos/docs)

Getting started with Anthos.

[https://www.youtube.com/watch?v=DM8p_cnc6ZY](https://www.youtube.com/watch?v=DM8p_cnc6ZY)

A sample deployment for Anthos. 

[https://www.youtube.com/watch?v=qgg1ceR6-es](https://www.youtube.com/watch?v=qgg1ceR6-es)

VM instances can exist on premises, managed by products such as VMWare vSphere, and in public clouds such as AWS or Azure, in addition to Google Cloud Compute Engine instances.

https://www.youtube.com/watch?v=XB52jRLHeko&list=PLIivdWyY5sqL8p1URcr6h1OkeJ01Myz57


### Anthos Technical Overview

<img src="https://cloud.google.com/anthos/images/anthos-15-components.svg" width="800">


https://cloud.google.com/anthos/docs/concepts/overview

### Anthos Deployments

GKE on-prem is hybrid cloud software that brings Google Kubernetes Engine (GKE) to on-premises data centers. GKE on-prem is a reliable, efficient, and secured way to run Kubernetes clusters anywhere.

[https://cloud.google.com/anthos/gke/docs/on-prem](https://cloud.google.com/anthos/gke/docs/on-prem)


### Anthos Config Management

Anthos Config Management is a key component of Anthos. With Anthos Config Management, you can create a common configuration across all your infrastructure, including custom policies, and apply it both on-premises and in the cloud. Anthos Config Management evaluates changes and rolls them out to all Kubernetes clusters so that your desired state is always reflected.

[https://cloud.google.com/anthos-config-management/docs](https://cloud.google.com/anthos-config-management/docs)

Learn how you can manage your Anthos deployments at scale, using Anthos Config Management.

[https://www.youtube.com/watch?v=nhXJzjITgMA](https://www.youtube.com/watch?v=nhXJzjITgMA)


### Cloud Run for Anthos

Create a cluster enabled for Cloud Run for Anthos on Google Cloud and then deploy a prebuilt sample container to the cluster.

[https://cloud.google.com/run/docs/quickstarts/prebuilt-deploy-gke](https://cloud.google.com/run/docs/quickstarts/prebuilt-deploy-gke)

Learn how Cloud Run lets you adopt the simplicity of serverless on your own terms: on Google’s fully-managed infrastructure, or in your Anthos clusters. 

[https://www.youtube.com/watch?v=0T5UliS9j8A](https://www.youtube.com/watch?v=0T5UliS9j8A)


### Migrate for Anthos

With Migrate for Anthos, you can migrate your VMs from [supported source platforms](https://cloud.google.com/migrate/anthos/docs/migration-prerequisites) to Google Kubernetes Engine or [Anthos](https://cloud.google.com/anthos).

[https://cloud.google.com/migrate/anthos/docs/getting-started](https://cloud.google.com/migrate/anthos/docs/getting-started)

Migrating and modernizing enterprise workloads using Migrate for Anthos.

[https://www.youtube.com/watch?v=8Q1kqWVbKQY](https://www.youtube.com/watch?v=8Q1kqWVbKQY)

A video about migration  and modernization a legacy on-premises application to GKE while gaining better observability and other benefits.

[https://www.youtube.com/watch?v=inEaRCFwovU](https://www.youtube.com/watch?v=inEaRCFwovU)


### Google Cloud Marketplace for Anthos

A Kubernetes app is a containerized application that you can run on your Kubernetes cluster. The Kubernetes apps in Cloud Marketplace include container images and configuration files, such as a kubectl configuration or a Helm chart. When you deploy an app from Cloud Marketplace, the Kubernetes resources are created in your cluster, and you can manage the resources as a group.

[https://cloud.google.com/marketplace/docs/kubernetes-apps](https://cloud.google.com/marketplace/docs/kubernetes-apps)


### Anthos on AWS

Anthos is Google's managed platform for application modernization and delivery, providing consistent automated operations so that an Enterprise can write once and deploy anywhere. This session will provide an overview and technical deep dive into "Extending Anthos to AWS", including capabilities that facilitate automation best practices that span across multi-cloud environments and the freedom to run, deploy and manage applications on the cloud of your choice.

[https://www.youtube.com/watch?v=qnlrEXOGFz4](https://www.youtube.com/watch?v=qnlrEXOGFz4)


### Connect

Connect allows you to connect any of your Kubernetes clusters to Google Cloud. This enables access to cluster and to workload management features, including a unified user interface, [Cloud Console](https://cloud.google.com/cloud-console), to interact with your cluster.

If your network is configured to allow outbound requests, you can configure the Connect Agent to traverse NATs, egress proxies, and firewalls to establish a long-lived, encrypted connection between your cluster's Kubernetes API server and your Google Cloud project. Once this connection is enabled, you can use your own credentials to log back into your clusters and access details about their Kubernetes resources. This effectively replicates the UI experience that is otherwise only available to GKE clusters.

After the connection is established, the Connect Agent software can exchange account credentials, technical details, and metadata about connected infrastructure and workloads necessary to manage them with Google Cloud, including the details of resources, applications, and hardware.

This cluster service data is associated with your Google Cloud project and/or account. Google uses this data to maintain a control plane between your cluster and Google Cloud, to provide you with any Google Cloud services and features you request, including facilitating support, billing, providing updates, and to measure and improve the reliability, quality, capacity, and functionality of Connect and Google Cloud services available through Connect.

You remain in control of what data is sent through Connect.

[https://cloud.google.com/anthos/multicluster-management/connect](https://cloud.google.com/anthos/multicluster-management/connect)


### Qwiklabs


#### Migrate for Anthos

[Anthos](https://cloud.google.com/anthos) is an open source application platform that enables you to modernize your existing applications on your hybrid or multi-cloud environment. You can build new VMs and run them anywhere in a secure manner. Anthos is built on open source technologies pioneered by Google — including Kubernetes, Istio, and Knative — and enables consistency between on-premises and cloud environments.

[Migrate for Anthos: Qwik Start](https://www.qwiklabs.com/focuses/10268?catalog_rank=%7B%22rank%22%3A6%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&parent=catalog&search_id=7467866)


#### Anthos Service Mesh

This intermediate-level quest is unique among Qwiklabs quests. These labs have been curated to give operators hands-on practice with Anthos—a new, open application modernization platform on GCP. Anthos enables you to build and manage modern hybrid applications. Tasks include: installing service mesh, collecting telemetry, and securing your microservices with service mesh policies. 

[Anthos: Service Mesh](https://www.qwiklabs.com/quests/100?catalog_rank=%7B%22rank%22%3A1%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&search_id=7482852)

