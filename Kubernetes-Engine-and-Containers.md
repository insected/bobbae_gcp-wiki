- [Containers](#containers)
  * [What is a container?](#what-is-a-container-)
    + [Containers vs. VMs](#containers-vs-vms)
    + [Three ways to run containers in GCP](#three-ways-to-run-containers-in-gcp)
  * [Namespaces](#namespaces)
  * [Google Kubernetes Engine (GKE)](#google-kubernetes-engine--gke-)
    + [An introduction to Kubernetes](#an-introduction-to-kubernetes)
    + [Kubectl](#kubectl)
      - [Kustomize](#kustomize)
    + [How to create a GKE cluster](#how-to-create-a-gke-cluster)
    + [Building small containers](#building-small-containers)
    + [Organizing with Kubernetes namespaces](#organizing-with-kubernetes-namespaces)
    + [Upgrading with zero down time](#upgrading-with-zero-down-time)
    + [Mapping external services](#mapping-external-services)
    + [Terminating with Grace](#terminating-with-grace)
    + [Health check](#health-check)
    + [Google GKE Documentation](#google-gke-documentation)
    + [Kubernetes URLs](#kubernetes-urls)
    + [Resource Limits](#resource-limits)
    + [RBAC](#rbac)
    + [Deployment & Service](#deployment---service)
    + [Configmaps & Secrets](#configmaps---secrets)
    + [Stateful Sets](#stateful-sets)
    + [DaemonSet](#daemonset)
    + [CRD](#crd)
    + [Operator Pattern](#operator-pattern)
      - [Operator Hub](#operator-hub)
      - [Operator Sprawl](#operator-sprawl)
    + [Kubernetes Networking](#kubernetes-networking)
    + [Kubernetes Storage](#kubernetes-storage)
    + [Persistent Volume Claim](#persistent-volume-claim)
    + [Authentication and Authorization in Kubernetes](#authentication-and-authorization-in-kubernetes)
    + [Ingress](#ingress)
    + [GKE HA and Stateful Application, PVC](#gke-ha-and-stateful-application--pvc)
    + [Kubernetes applications on Google Cloud Marketplace](#kubernetes-applications-on-google-cloud-marketplace)
    + [GKE Operations](#gke-operations)
    + [Cloud Build & Cloud Code with Containers](#cloud-build---cloud-code-with-containers)
      - [Cloud Code](#cloud-code)
      - [Cloud Build](#cloud-build)
      - [Container Registry](#container-registry)
    + [Batch on GKE](#batch-on-gke)
    + [Prometheus](#prometheus)
    + [Grafana](#grafana)
    + [Configuration as Data](#configuration-as-data)
    + [Binary Authorizations](#binary-authorizations)
    + [HPA: Horizontal Pod Autoscaling](#hpa--horizontal-pod-autoscaling)
    + [Qwiklabs](#qwiklabs)
      - [GKE](#gke)
      - [GKE Solutions](#gke-solutions)
      - [GKE Deploy](#gke-deploy)
      - [Security in GKE](#security-in-gke)
      - [Deploying Python Apps on GKE](#deploying-python-apps-on-gke)
      - [Cloud Logging on GKE](#cloud-logging-on-gke)
      - [Migrating to GKE](#migrating-to-gke)
      - [Java Application Development](#java-application-development)
      - [Operations Suite on GKE](#operations-suite-on-gke)
      - [Deploy Kubernetes Load Balancer with Terraform](#deploy-kubernetes-load-balancer-with-terraform)
  * [Service Mesh](#service-mesh)
    + [Istio](#istio)
      - [Istiod vs microservices](#istiod-vs-microservices)
    + [Envoy](#envoy)
    + [Apigee Envoy](#apigee-envoy)
    + [Ambassador Edge Stack and Consul Service Mesh](#ambassador-edge-stack-and-consul-service-mesh)
    + [Linkerd](#linkerd)

<small><i><a href='http://ecotrust-canada.github.io/markdown-toc/'>Table of contents generated with markdown-toc</a></i></small>

## Containers


### What is a container?

A container is a standard unit of software that packages up code and all its dependencies so the application runs quickly and reliably from one computing environment to another. A Docker container image is a lightweight, standalone, executable package of software that includes everything needed to run an application: code, runtime, system tools, system libraries and settings.

[https://www.docker.com/resources/what-container](https://www.docker.com/resources/what-container)


#### Containers vs. VMs

Virtual machines and containers differ in several ways, but the primary difference is that containers provide a way to virtualize an OS so that multiple workloads can run on a single OS instance. With VMs, the hardware is being virtualized to run multiple OS instances. Containers’ speed, agility, and portability make them yet another tool to help streamline software development.

 
Comparison of containerizing vs using VMs.

[https://www.youtube.com/watch?v=TvnZTi_gaNc](https://www.youtube.com/watch?v=TvnZTi_gaNc)


#### Three ways to run containers in GCP

Find out the top three ways you can run your containers on Google Cloud! Google Kubernetes Engine for a container orchestration solution, Cloud Run for a fully serverless approach and Compute Engine to simply use Virtual Machines.

[https://www.youtube.com/watch?v=jh0fPT-AWwM](https://www.youtube.com/watch?v=jh0fPT-AWwM)


### Namespaces
Namespaces are a feature of the Linux kernel that partitions kernel resources such that one set of processes sees one set of resources while another set of processes sees a different set of resources. The feature works by having the same namespace for a set of resources and processes, but those namespaces refer to distinct resources. Resources may exist in multiple spaces. Examples of such resources are process IDs, hostnames, user IDs, file names, and some names associated with network access, and interprocess communication.

Namespaces are a fundamental aspect of containers on Linux.

The term "namespace" is often used for a type of namespace (e.g. process ID) as well as for a particular space of names.

A Linux system starts out with a single namespace of each type, used by all processes. Processes can create additional namespaces and join different namespaces.

An overview of Linux namespaces and how they are used in containers.

[https://www.youtube.com/watch?v=kl8roLaLy-g](https://www.youtube.com/watch?v=kl8roLaLy-g)

Some videos about Network Namespaces and how they are used in containers.

[https://www.youtube.com/watch?v=j_UUnlVC2Ss&list=TLPQMTQxMDIwMjD4ry4yOmhx2w&index=2](https://www.youtube.com/watch?v=j_UUnlVC2Ss&list=TLPQMTQxMDIwMjD4ry4yOmhx2w&index=2)


### Google Kubernetes Engine (GKE)
Secured and fully managed Kubernetes service with revolutionary autopilot mode of operation.

#### An introduction to Kubernetes

[Kubernetes](https://kubernetes.io) is an open-source container-orchestration system for automating computer application deployment, scaling, and management. It was originally designed by Google and is now maintained by the Cloud Native Computing Foundation.

[https://www.youtube.com/watch?v=pQ87vVMZK-A](https://www.youtube.com/watch?v=pQ87vVMZK-A)

[https://www.youtube.com/watch?v=Krpb44XR0bk](https://www.youtube.com/watch?v=Krpb44XR0bk)


#### Kubectl

The Kubernetes command-line tool, [kubectl](https://kubernetes.io/docs/reference/kubectl/kubectl/), allows you to run commands against Kubernetes clusters. You can use kubectl to deploy applications, inspect and manage cluster resources, and view logs. For a complete list of kubectl operations, see [Overview of kubectl](https://kubernetes.io/docs/reference/kubectl/overview/).

[https://www.youtube.com/watch?v=azuwXALfyRg](https://www.youtube.com/watch?v=azuwXALfyRg)


##### Kustomize

Kustomize introduces a template-free way to customize application configuration that simplifies the use of off-the-shelf applications. Now, built into kubectl as apply -k.

[https://www.youtube.com/watch?v=uvH84BviDS4](https://www.youtube.com/watch?v=uvH84BviDS4)

https://kustomize.io/

#### How to create a GKE cluster

This video will teach you how to create a Google Kubernetes Engine (GKE) cluster using Terraform.

[https://www.youtube.com/watch?v=Vcv6GapxUCI](https://www.youtube.com/watch?v=Vcv6GapxUCI)

Here are some tutorials for using Terraform to manage Kubernetes on GCP.
[HashCorp Terraform Kubernetes Tutorials](https://learn.hashicorp.com/tutorials/terraform/gke?in=terraform/kubernetes)

#### Building small containers

A video to show you how you can build small containers to make your Kubernetes deployments faster and more secure.

[https://www.youtube.com/watch?v=wGz_cbtCiEA](https://www.youtube.com/watch?v=wGz_cbtCiEA)


#### Organizing with Kubernetes namespaces

This video shows how to work with Namespaces and how they can help you manage your Kubernetes resources.

[https://www.youtube.com/watch?v=xpnZX3if9Tc](https://www.youtube.com/watch?v=xpnZX3if9Tc)


#### Upgrading with zero down time

[https://www.youtube.com/watch?v=ajbC1yTW2x0](https://www.youtube.com/watch?v=ajbC1yTW2x0)


#### Mapping external services

[https://www.youtube.com/watch?v=fvpq4jqtuZ8](https://www.youtube.com/watch?v=fvpq4jqtuZ8)


#### Terminating with Grace

[https://www.youtube.com/watch?v=Z_l_kE1MDTc](https://www.youtube.com/watch?v=Z_l_kE1MDTc)


#### Health check

[https://www.youtube.com/watch?v=mxEvAPQRwhw](https://www.youtube.com/watch?v=mxEvAPQRwhw)


#### Google GKE Documentation

[https://cloud.google.com/kubernetes-engine/docs](https://cloud.google.com/kubernetes-engine/docs)


#### Kubernetes URLs

[https://github.com/ramitsurana/awesome-kubernetes](https://github.com/ramitsurana/awesome-kubernetes)


#### Resource Limits

[https://www.youtube.com/watch?v=xjpHggHKm78&list=PLIivdWyY5sqL3xfXz5xJvwzFW_tlQB_GB&index=4](https://www.youtube.com/watch?v=xjpHggHKm78&list=PLIivdWyY5sqL3xfXz5xJvwzFW_tlQB_GB&index=4)


#### RBAC

[https://www.youtube.com/watch?v=4HMRFcg6nEY](https://www.youtube.com/watch?v=4HMRFcg6nEY)


#### Deployment & Service

[https://www.youtube.com/watch?v=qmDzcu5uY1I](https://www.youtube.com/watch?v=qmDzcu5uY1I)

https://kubernetes.io/docs/concepts/services-networking/connect-applications-service/

#### Configmaps & Secrets

[https://www.youtube.com/watch?v=FAnQTgr04mU](https://www.youtube.com/watch?v=FAnQTgr04mU)


#### Stateful Sets

[https://www.youtube.com/watch?v=pPQKAR1pA9U](https://www.youtube.com/watch?v=pPQKAR1pA9U)


#### DaemonSet

A DaemonSet ensures that all (or some) Nodes run a copy of a Pod. As nodes are added to the cluster, Pods are added to them. As nodes are removed from the cluster, those Pods are garbage collected. Deleting a DaemonSet will clean up the Pods it created.

[https://kubernetes.io/docs/concepts/workloads/controllers/daemonset/](https://kubernetes.io/docs/concepts/workloads/controllers/daemonset/)


#### CRD

CRD stands for  Custom Resource Definition.

A resource is an endpoint in the [Kubernetes API](https://kubernetes.io/docs/reference/using-api/api-overview/) that stores a collection of [API objects](https://kubernetes.io/docs/concepts/overview/working-with-objects/kubernetes-objects/) of a certain kind; for example, the built-in pods resource contains a collection of Pod objects.

A custom resource is an extension of the Kubernetes API that is not necessarily available in a default Kubernetes installation. It represents a customization of a particular Kubernetes installation. However, many core Kubernetes functions are now built using custom resources, making Kubernetes more modular. Custom resources can appear and disappear in a running cluster through dynamic registration, and cluster admins can update custom resources independently of the cluster itself. Once a custom resource is installed, users can create and access its objects using [kubectl](https://kubernetes.io/docs/reference/kubectl/overview/), just as they do for built-in resources like Pods.

[https://kubernetes.io/docs/concepts/extend-kubernetes/api-extension/custom-resources/](https://kubernetes.io/docs/concepts/extend-kubernetes/api-extension/custom-resources/)

Kubebuilder is a framework for building Kubernetes APIs using custom resource definitions (CRDs).

https://book.kubebuilder.io/quick-start.html

https://github.com/kubernetes-sigs/kubebuilder


#### Operator Pattern

In [Kubernetes](https://opensource.com/resources/what-is-kubernetes), objects are analogous to a job or a completed task in the real world. You can use them to define common tasks, store them in a version control system, and apply them with kubectl apply. Kubernetes ensures that this triggers everything necessary to bring your declarative description to life by creating the dependent resources (like pods) to run your software. Kubernetes contains a number of built-in object types that can be created with this workflow, like Deployments and Services. With Operators, Kubernetes allows cluster maintainers or software providers to define their own Kubernetes object types, called custom resource definitions (CRDs). These objects can be handled by the Kubernetes API, just like built-in object types. Inside the Operator code, authors can define how to act on those custom objects. Operators are software extensions to Kubernetes that make use of [custom resources](https://kubernetes.io/docs/concepts/extend-kubernetes/api-extension/custom-resources/) to manage applications and their components. Operators follow Kubernetes principles, notably the [control loop](https://kubernetes.io/docs/concepts/architecture/controller).

Operators make it easy to manage complex stateful applications on top of Kubernetes. However writing an Operator today can be difficult because of challenges such as using low level APIs, writing boilerplate, and a lack of modularity which leads to duplication.

[https://kubernetes.io/docs/concepts/extend-kubernetes/operator/](https://kubernetes.io/docs/concepts/extend-kubernetes/operator/)

The Operator SDK is a framework that uses the controller-runtime library to make writing operators easier by providing:

* High level APIs and abstractions to write the operational logic more intuitively
* Tools for scaffolding and code generation to bootstrap a new project fast
* Extensions to cover common Operator use cases

https://github.com/operator-framework/operator-sdk
 
[https://opensource.com/article/20/3/kubernetes-operator-sdk](https://opensource.com/article/20/3/kubernetes-operator-sdk)

Shell-operator is a tool for running event-driven scripts in a Kubernetes cluster.

This operator is not an operator for a particular software product such as prometheus-operator or kafka-operator. Shell-operator provides an integration layer between Kubernetes cluster events and shell scripts by treating scripts as hooks triggered by events. Think of it as an operator-sdk but for scripts.

https://github.com/flant/shell-operator

Kubernetes Universal Declarative Operator (KUDO) provides a declarative approach to building production-grade Kubernetes operators. To quote the official documentation: "Operators are software extensions to Kubernetes that make use of custom resources to manage applications and their components". While Kubernetes already comes with a lot of built-in automation to run simple workloads, complex scenarios often need a human operator. 

https://d2iq.com/products/kudo

https://cert-manager.io/docs/installation/kubernetes/

https://krew.sigs.k8s.io/docs/user-guide/setup/install/

##### Operator Hub

[https://operatorhub.io/](https://operatorhub.io/)


##### Operator Sprawl

[https://thenewstack.io/the-runaway-problem-of-kubernetes-operators-and-dependency-lifecycles/](https://thenewstack.io/the-runaway-problem-of-kubernetes-operators-and-dependency-lifecycles/)


#### Kubernetes Networking

A video about kubernetes networking.

[https://www.youtube.com/watch?v=tq9ng_Nz9j8](https://www.youtube.com/watch?v=tq9ng_Nz9j8)

A video about kubernetes services networking.

[https://www.youtube.com/watch?v=NFApeJRXos4](https://www.youtube.com/watch?v=NFApeJRXos4)

A video about kubernetes ingress networking.

[https://www.youtube.com/watch?v=40VfZ_nIFWI](https://www.youtube.com/watch?v=40VfZ_nIFWI)

A video about how ingress works.

[https://www.youtube.com/watch?v=_BbxJGiMtL8](https://www.youtube.com/watch?v=_BbxJGiMtL8)


#### Kubernetes Storage

[https://www.youtube.com/watch?v=qktFhjJmFhg](https://www.youtube.com/watch?v=qktFhjJmFhg)


#### Persistent Volume Claim

[https://www.youtube.com/watch?v=0swOh5C3OVM](https://www.youtube.com/watch?v=0swOh5C3OVM)


#### Authentication and Authorization in Kubernetes

[https://www.youtube.com/watch?v=dAUJ3TBwDWo](https://www.youtube.com/watch?v=dAUJ3TBwDWo)


#### Ingress

[https://www.youtube.com/watch?v=80Ew_fsV4rM](https://www.youtube.com/watch?v=80Ew_fsV4rM)


#### GKE HA and Stateful Application, PVC

Kubernetes is a great tool to host your highly available applications but what happens when you have to work with stateful workloads? 

[https://www.youtube.com/watch?v=rRZtZX0PDFc](https://www.youtube.com/watch?v=rRZtZX0PDFc)


#### Kubernetes applications on Google Cloud Marketplace

The Kubernetes apps in Cloud Marketplace include container images and configuration files, such as a kubectl configuration or a[ Helm chart](https://helm.sh/docs/topics/charts/). When you deploy an app from Cloud Marketplace, the Kubernetes resources are created in your cluster, and you can manage the resources as a group.

[https://cloud.google.com/marketplace/docs/kubernetes-apps](https://cloud.google.com/marketplace/docs/kubernetes-apps)


#### GKE Operations

A video about using Cloud Logging on GKE.

[https://www.youtube.com/watch?v=IusP8jDfnt4](https://www.youtube.com/watch?v=IusP8jDfnt4)


#### Cloud Build & Cloud Code with Containers


##### Cloud Code

Using Cloud Code with Kubernetes.

[https://www.youtube.com/watch?v=KNd0mTxcQ_M](https://www.youtube.com/watch?v=KNd0mTxcQ_M)


##### Cloud Build

Cloud Build is a service that executes your builds on Google Cloud Platform infrastructure. Cloud Build can import source code from Google Cloud Storage, Cloud Source Repositories, GitHub, or Bitbucket, execute a build to your specifications, and produce artifacts such as Docker containers or Java archives.

A video about Cloud Build with Containers.

[https://www.youtube.com/watch?v=w7dMHiEyGAs](https://www.youtube.com/watch?v=w7dMHiEyGAs)

Cloud Build executes your build as a series of build steps, where each build step is run in a Docker container. A build step can do anything that can be done from a container irrespective of the environment. To perform your tasks, you can either [use the supported build steps](https://cloud.google.com/cloud-build/docs/configuring-builds/build-test-deploy-artifacts) provided by Cloud Build or [write your own build steps](https://cloud.google.com/cloud-build/docs/create-custom-build-steps).

[https://cloud.google.com/cloud-build/docs](https://cloud.google.com/cloud-build/docs)


##### Container Registry

Google Container Registry is a private container image registry that runs on Google Cloud's reliable, fast, and secure infrastructure. You can access Container Registry through secure HTTPS endpoints, which allow you to push, pull, and manage images from any system, VM instance, or your own hardware. Additionally, you can use the [Docker credential helper](https://cloud.google.com/container-registry/docs/advanced-authentication#docker_credential_helper) command-line tool to configure Docker to authenticate directly with Container Registry.

While Docker provides a central registry for storing public images, you might not want your images to be accessible to the world. To control access to your images, you must store your images in a private registry.

[Container Registry: Qwik Start](https://www.qwiklabs.com/focuses/1768?catalog_rank=%7B%22rank%22%3A7%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&parent=catalog&search_id=7467880)


#### Batch on GKE

Batch on GKE (Batch) is a cloud-native solution for scheduling and managing batch workloads. With Batch, you can leverage the on-demand and flexible nature of cloud. Batch is based on Kubernetes and containers so your jobs are portable.

[https://cloud.google.com/kubernetes-engine/docs/concepts/batch](https://cloud.google.com/kubernetes-engine/docs/concepts/batch)

A video about using Batch on GKE.

[https://www.youtube.com/watch?v=qLSLs-ko3ik](https://www.youtube.com/watch?v=qLSLs-ko3ik)


#### Prometheus

[https://www.youtube.com/watch?v=h4Sl21AKiDg](https://www.youtube.com/watch?v=h4Sl21AKiDg)

[https://www.youtube.com/watch?v=XToKHYXSUyc](https://www.youtube.com/watch?v=XToKHYXSUyc)


#### Grafana

[https://grafana.com/](https://grafana.com/)


#### Configuration as Data

[https://cloud.google.com/blog/products/containers-kubernetes/understanding-configuration-as-data-in-kubernetes](https://cloud.google.com/blog/products/containers-kubernetes/understanding-configuration-as-data-in-kubernetes)


#### Binary Authorizations

[https://cloud.google.com/binary-authorization/docs/overview](https://cloud.google.com/binary-authorization/docs/overview)


#### HPA: Horizontal Pod Autoscaling

[https://cloud.google.com/kubernetes-engine/docs/concepts/horizontalpodautoscaler](https://cloud.google.com/kubernetes-engine/docs/concepts/horizontalpodautoscaler)


#### Qwiklabs


##### GKE

Kubernetes is the most popular container orchestration system, and Google Kubernetes Engine was designed specifically to support managed Kubernetes deployments in Google Cloud. In this advanced-level quest, you will get hands-on practice configuring Docker images, containers, and deploying fully-fledged Kubernetes Engine applications. This quest will teach you the practical skills needed for integrating container orchestration into your own workflow. 

[Kubernetes in Google Cloud](https://www.qwiklabs.com/quests/29?catalog_rank=%7B%22rank%22%3A1%2C%22num_filters%22%3A1%2C%22has_search%22%3Atrue%7D&search_id=7467715)


##### GKE Solutions

Containerized applications have changed the game and are here to stay. With Kubernetes, you can orchestrate containers with ease, and integration with the Google Cloud Platform is seamless. In this advanced-level quest, you will be exposed to a wide range of Kubernetes use cases and will get hands-on practice architecting solutions over the course of 8 labs. From building Slackbots with NodeJS, to deploying game servers on clusters, to running the Cloud Vision API, Kubernetes Solutions will show you first-hand how agile and powerful this container orchestration system is.

[Kubernetes Solutions](https://www.qwiklabs.com/quests/45?catalog_rank=%7B%22rank%22%3A2%2C%22num_filters%22%3A1%2C%22has_search%22%3Atrue%7D&search_id=7467715)


##### GKE Deploy

Kubernetes is the most popular container orchestration system, and Google Kubernetes Engine was designed specifically to support managed Kubernetes deployments in Google Cloud. In this advanced-level quest, you will get hands-on practice configuring Docker images, containers, and deploying fully-fledged Kubernetes Engine applications. This quest will teach you the practical skills needed for integrating container orchestration into your own workflow. 

[Deploy to Kubernetes in Google Cloud](https://www.qwiklabs.com/quests/116?catalog_rank=%7B%22rank%22%3A3%2C%22num_filters%22%3A1%2C%22has_search%22%3Atrue%7D&search_id=7467715)


##### Security in GKE

The following hands-on labs focus on [security at scale](https://cloud.google.com/anthos/docs/concepts/anthos-overview#service_management) when deploying and managing production GKE environments -- specifically role-based access control, hardening, VPC networking, and binary authorization. 

[Secure Workloads in Google Kubernetes Engine](https://www.qwiklabs.com/quests/142?catalog_rank=%7B%22rank%22%3A4%2C%22num_filters%22%3A1%2C%22has_search%22%3Atrue%7D&search_id=7467715)

[Google Kubernetes Engine Best Practices: Security](https://www.qwiklabs.com/quests/64?catalog_rank=%7B%22rank%22%3A5%2C%22num_filters%22%3A1%2C%22has_search%22%3Atrue%7D&search_id=7467715)


##### Deploying Python Apps on GKE

Google Kubernetes Engine provides a managed environment for deploying, managing, and scaling your containerized applications using Google infrastructure. The environment Kubernetes Engine provides consists of multiple machines (specifically, Compute Engine instances) grouped together to form a cluster. Kubernetes provides the mechanisms through which you interact with your cluster. You use Kubernetes commands and resources to deploy and manage your applications, perform administration tasks and set policies, and monitor the health of your deployed workloads. In this lab, you deploy the Quiz application into Kubernetes Engine, leveraging Google Cloud resources, including Container Builder and Container Registry, and Kubernetes resources, such as Deployments, Pods, and Services.

[App Dev: Deploying the Application into Kubernetes Engine - Python](https://www.qwiklabs.com/focuses/1073?catalog_rank=%7B%22rank%22%3A30%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&parent=catalog&search_id=7467972)


##### Cloud Logging on GKE

Cloud Logging can be used aggregate logs from all Google Cloud resources, as well as any custom resources on other platforms, to allow for one centralized store for all logs and metrics. Logs are aggregated and then viewable within the provided Cloud Logging UI. They can also be [exported to Sinks](https://cloud.google.com/logging/docs/export/configure_export_v2) to support more specialized use cases. Currently, Cloud Logging supports exporting to the following sinks:



*   Cloud Storage
*   Pub/Sub
*   BigQuery

In this lab you will deploy a sample application to Kubernetes Engine that forwards log events to [Cloud Logging](https://cloud.google.com/logging/) using [Terraform](https://www.terraform.io/), a declarative [Infrastructure as Code](https://en.wikipedia.org/wiki/Infrastructure_as_Code) tool that enables configuration files to automate the deployment and evolution of infrastructure in the cloud. The configuration will also create a Cloud Storage bucket and a BigQuery dataset for exporting log data to. This lab was created by GKE Helmsman engineers to give you a better understanding of Cloud Logging. You can view this demo on Github [here](https://github.com/GoogleCloudPlatform/gke-binary-auth-demo.git). 

[Cloud Logging on Kubernetes Engine](https://www.qwiklabs.com/focuses/10910?catalog_rank=%7B%22rank%22%3A10%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&parent=catalog&search_id=7468028)


##### Migrating to GKE

Containers are quickly becoming an industry standard for deployment of software applications. The business and technological advantages of containerized workloads are driving many teams towards moving their applications to containers. This lab provides a basic walkthrough of migrating a stateless application from running on a VM to running on [Kubernetes Engine (GKE)](https://cloud.google.com/kubernetes-engine/). It demonstrates the lifecycle of an application transitioning from a typical VM/OS-based deployment to a specialized os for containers to a platform for containers better known as [GKE](https://cloud.google.com/kubernetes-engine/).

[Migrating to GKE Containers](https://www.qwiklabs.com/focuses/12768?catalog_rank=%7B%22rank%22%3A7%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&parent=catalog&search_id=7467835)


##### Java Application Development

In this advanced-level quest, you will learn the ins and outs of developing GCP applications in Java. The first labs will walk you through the basics of environment setup and application data storage with Cloud Datastore. Once you have a handle on the fundamentals, you will get hands-on practice deploying Java applications on Kubernetes and App Engine (the latter is the same framework that powers Snapchat!) With specialized bonus labs that teach user authentication and backend service development, this quest will give you practical experience so you can start developing robust Java applications straight away.

[Application Development - Java](https://www.qwiklabs.com/quests/42?catalog_rank=%7B%22rank%22%3A1%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&search_id=7467936)


##### Operations Suite on GKE

In this fundamental-level quest, you will learn the ins and outs of Google Cloud's operations suite running on Google Kubernetes Engine, an important service for generating insights into the health of your applications. It provides a wealth of information in application monitoring, report logging, and diagnoses. The labs in this quest will give you hands-on practice with and will teach you how to monitor virtual machines, generate logs and alerts, and create custom metrics for application data.

[Google Cloud's Operations Suite on GKE](https://www.qwiklabs.com/quests/133?catalog_rank=%7B%22rank%22%3A5%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&search_id=7468028)


##### Deploy Kubernetes Load Balancer with Terraform

In Terraform, a Provider is the logical abstraction of an upstream API. This lab will show you how to set up a Kubernetes cluster and deploy a Load Balancer type NGINX service on it.

A favorite lab.

[https://www.qwiklabs.com/focuses/1205?parent=catalog](https://www.qwiklabs.com/focuses/1205?parent=catalog)


### Service Mesh

Why use service mesh? How does istio work?

[https://www.youtube.com/watch?v=6zDrLvpfCK4](https://www.youtube.com/watch?v=6zDrLvpfCK4)

Enterprises are increasingly adopting microservices to enable new levels of IT agility, scale, and innovation — but a successful microservices implementation is notoriously complicated. As the number of services an organization uses grows, complexity and risk can increase rapidly. Moreover, microservices need to be exposed as APIs to enable seamless access for internal groups — or with external partners to increase operational efficiency and speed up development. This video shows how to build a secure and scalable [microservices architecture](https://medium.com/hashmapinc/the-what-why-and-how-of-a-microservices-architecture-4179579423a9) with Kubernetes, Istio, and Apigee API management platform.

[https://www.youtube.com/watch?v=IblDMVwSSk4](https://www.youtube.com/watch?v=IblDMVwSSk4)


#### Istio

Cloud platforms provide a wealth of benefits for the organizations that use them. However, there’s no denying that adopting the cloud can put strains on DevOps teams. Developers must use microservices to architect for portability, meanwhile operators are managing extremely large hybrid and multi-cloud deployments. Istio lets you connect, secure, control, and observe services.

At a high level, Istio helps reduce the complexity of these deployments, and eases the strain on your development teams. It is a completely open source service mesh that layers transparently onto existing distributed applications. It is also a platform, including APIs that let it integrate into any logging platform, or telemetry or policy system. Istio’s diverse feature set lets you successfully, and efficiently, run a distributed microservice architecture, and provides a uniform way to secure, connect, and monitor microservices.

Istio addresses the challenges developers and operators face as monolithic applications transition towards a distributed microservice architecture. To see how, it helps to take a more detailed look at Istio’s service mesh.

Istio makes it easy to create a network of deployed services with load balancing, service-to-service authentication, monitoring, and more, with few or no code changes in service code. You add Istio support to services by deploying a special sidecar proxy throughout your environment that intercepts all network communication between microservices, then configure and manage Istio using its control plane functionality, which includes:

* Automatic load balancing for HTTP, gRPC, WebSocket, and TCP traffic.
* Fine-grained control of traffic behavior with rich routing rules, retries, failovers, and fault injection.
* A pluggable policy layer and configuration API supporting access controls, rate limits and quotas.
* Automatic metrics, logs, and traces for all traffic within a cluster, including cluster ingress and egress.

Secure service-to-service communication in a cluster with strong identity-based authentication and authorization.

The term service mesh is used to describe the network of microservices that make up such applications and the interactions between them. As a service mesh grows in size and complexity, it can become harder to understand and manage. Its requirements can include discovery, load balancing, failure recovery, metrics, and monitoring. A service mesh also often has more complex operational requirements, like A/B testing, canary rollouts, rate limiting, access control, and end-to-end authentication.

Istio provides behavioral insights and operational control over the service mesh as a whole, offering a complete solution to satisfy the diverse requirements of microservice applications.


Your organization has moved to microservices, then to Kubernetes. But now you have lots of workloads, and many different points of entry into your application. You've heard about how a service mesh can help with traffic management, so you've installed Istio and have explored the samples. Now what? This talk goes deep with Istio traffic routing, highlighting the features that can help your organization reduce complexity, improve performance, and scale to your customers' needs. Using a microservices application running on Google Kubernetes Engine, we will walk through exactly how to manage traffic with Istio. Demos will include load balancing, rollouts, ingress and egress, content-based routing, traffic mirroring, and resilience features such as circuit breaking. 

[https://www.youtube.com/watch?v=7cINRP0BFY8](https://www.youtube.com/watch?v=7cINRP0BFY8)

Istio provides a powerful set of Kubernetes abstractions for traffic routing, security, and telemetry. But whether you're a first-time user, or running Istio in production, it's likely that you've encountered some roadblocks when installing and using Istio. This talk dives into the most common problems you may encounter with Istio's internals, and addresses how to fix them. Through a whirlwind set of demos running on Google Kubernetes Engine, we will cover scenarios like: why does my Istio install fail? Why is Pilot crashing? what if my sidecar proxies aren't routing properly? what if I can't see Istio metrics in Stackdriver? Why is my end-user JWT authentication failing? why won't IngressGateway accept incoming traffic? — and more! 

[https://www.youtube.com/watch?v=FbYBO7Pi2d8](https://www.youtube.com/watch?v=FbYBO7Pi2d8)


##### Istiod vs microservices

[https://blog.christianposta.com/microservices/istio-as-an-example-of-when-not-to-do-microservices/](https://blog.christianposta.com/microservices/istio-as-an-example-of-when-not-to-do-microservices/)


#### Envoy
Envoy is a L7 edge service Proxy used widely by service mesh controllers such as , Ambassador, Consul, Contour and istio.

[Watch a Video about Borg, Cloud Load Balancing, Kubernetes and Envoy into service mesh driven by Istio](https://www.youtube.com/watch?v=glATqKI-WR8).

There are many [Open source projects built on Envoy Proxy](https://www.envoyproxy.io/community).

[Events in the life of a request](https://www.envoyproxy.io/docs/envoy/latest/intro/life_of_a_request) passing through an Envoy proxy is complicated.
How a request flows through the components in a network depends on the network topology. Envoy can be used in a wide variety of networking topologies. Envoy originated as a service mesh sidecar proxy, factoring out load balancing, routing, observability, security and discovery services from applications. In the service mesh model, requests flow through Envoys as a gateway to the network. Requests arrive at an Envoy via either ingress or egress listeners.  

#### Apigee Envoy

Wanting to know how to use Envoy to protect your microservices? In this video, we give you a demo on how to enforce policies for any microservice within a service mesh via the Apigee adapter for Envoy. Watch to learn about this tool, and see if it’s the best choice for your specific use case! 

[https://www.youtube.com/watch?v=BNkfoZt-jvU](https://www.youtube.com/watch?v=BNkfoZt-jvU)


#### Ambassador Edge Stack and Consul Service Mesh

[https://www.youtube.com/watch?v=XW3AXQfAaQc](https://www.youtube.com/watch?v=XW3AXQfAaQc)


#### Linkerd

https://linkerd.io/

[https://www.youtube.com/watch?v=Bj7gGQUiDuk](https://www.youtube.com/watch?v=Bj7gGQUiDuk)

https://www.infracloud.io/blogs/service-mesh-comparison-istio-vs-linkerd/