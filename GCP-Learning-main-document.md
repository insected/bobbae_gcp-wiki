# GCP Learning main document
## A GCP Training


## Table of Contents

- [Preparation](https://github.com/bobbae/gcp/wiki/Preparation)
- [Introduction](https://github.com/bobbae/gcp/wiki/GCP-Introduction)
- [Compute Engine)(https://github.com/bobbae/gcp/wiki/GCP-Compute-Engine)


### App Engine


#### Introduction

App Engine is a fully managed, serverless platform for developing and hosting web applications at scale. You can choose from several popular languages, libraries, and frameworks to develop your apps, then let App Engine take care of provisioning servers and scaling your app instances based on demand.

[https://cloud.google.com/appengine/docs](https://cloud.google.com/appengine/docs)

Google App Engine makes it easy to focus on your code, not infrastructure.

[https://www.youtube.com/watch?v=2PRciDpqpko](https://www.youtube.com/watch?v=2PRciDpqpko)

App Engine's environments, the [Standard Environment](https://cloud.google.com/appengine/docs/about-the-standard-environment) and the [Flexible environment](https://cloud.google.com/appengine/docs/flexible/) , support a host of programming languages, including Java, Python, PHP, Node.js, Go, etc.. The two environments give users maximum flexibility in how their application behaves since each environment has certain strengths. Read [The App Engine Environments](https://cloud.google.com/appengine/docs/the-appengine-environments) for more information.

[https://cloud.google.com/appengine/docs/standard/python3](https://cloud.google.com/appengine/docs/standard/python3)

App Engine allows developers to focus on doing what they do best, writing code. The App Engine standard environment is based on container instances running on Google's infrastructure. Containers are preconfigured with one of several available runtimes (Java 8, Python 3.7, Go and PHP). Each runtime also includes libraries that support [App Engine Standard APIs](https://cloud.google.com/appengine/docs/about-the-standard-environment#index_of_features).  


#### AppEngine Standard

The App Engine standard environment makes it easy to build and deploy an application that runs reliably even under heavy load and with large amounts of data. It includes the following features:



*   Persistent storage with queries, sorting, and transactions.
*   Automatic scaling and load balancing.
*   Asynchronous task queues for performing work outside the scope of a request.
*   Scheduled tasks for triggering events at specified times or regular intervals.
*   Integration with other [Google cloud services and APIs](https://cloud.google.com/products/).

Applications run in a secure, sandboxed environment, allowing the App Engine standard environment to distribute requests across multiple servers, and scaling servers to meet traffic demands. Your application runs within its own secure, reliable environment that is independent of the hardware, operating system, or physical location of the server.


#### Language Support


##### Go

[https://cloud.google.com/appengine/docs/go](https://cloud.google.com/appengine/docs/go)

Here are some useful URL pointers regarding Go.

[https://github.com/avelino/awesome-go](https://github.com/avelino/awesome-go)

A Go language tutorial video.

[https://www.youtube.com/watch?v=YS4e4q9oBaU&list=PLk_epN-7EGrjdhjn5gCMJ1aLIhRTHDJcu&index=11&t=0s](https://www.youtube.com/watch?v=YS4e4q9oBaU&list=PLk_epN-7EGrjdhjn5gCMJ1aLIhRTHDJcu&index=11&t=0s)


##### Python

[https://cloud.google.com/appengine/docs/python](https://cloud.google.com/appengine/docs/python)

A Python tutorial video.

[https://www.youtube.com/watch?v=rfscVS0vtbw](https://www.youtube.com/watch?v=rfscVS0vtbw)


##### Node.js

A video tutorial on how to create a web application using node.js and express framework.

[https://www.youtube.com/watch?v=G8uL0lFFoN0](https://www.youtube.com/watch?v=G8uL0lFFoN0)


#### App Engine Flexible

Based on [Google Compute Engine](https://cloud.google.com/compute), the App Engine flexible environment automatically scales your app up and down while also balancing the load. In the standard environment, your application runs on a lightweight instance inside of a sandbox. This sandbox restricts what your application can do. For example, the sandbox only allows your app to use a limited set of binary libraries, and your app cannot write to disk. The standard environment also limits the CPU and memory options available to your application. Because of these restrictions, most App Engine standard applications tend to be stateless web applications that respond to HTTP requests quickly.

In contrast, the flexible environment runs your application in Docker containers on [Google Compute Engine virtual machines (VMs)](https://cloud.google.com/compute/docs/instances), which have fewer restrictions. For example, you can use any programming language of your choice, write to disk, use any library you'd like, and even run multiple processes. The flexible environment also allows you to choose any Compute Engine machine type for your instances so that your application has access to more memory and CPU.

[https://cloud.google.com/appengine/docs/flexible/go/flexible-for-standard-users](https://cloud.google.com/appengine/docs/flexible/go/flexible-for-standard-users)


#### Qwiklabs


##### App Engine with Python

[App Engine: Qwik Start - Python](https://www.qwiklabs.com/focuses/1014?catalog_rank=%7B%22rank%22%3A19%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&parent=catalog&search_id=7467964)


##### App Engine with Go

[App Engine: Qwik Start - Go](https://www.qwiklabs.com/focuses/2754?catalog_rank=%7B%22rank%22%3A14%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&parent=catalog&search_id=7467964)


##### App Engine with Java

[App Engine: Qwik Start - Java](https://www.qwiklabs.com/focuses/951?parent=catalog)


##### Baseline

In this introductory-level quest, you will learn the fundamentals of developing and deploying applications on the Google Cloud Platform. You will get hands-on experience with the Google App Engine framework by launching applications written in languages like Python, Ruby, and Java (just to name a few). You will see first-hand how straightforward and powerful GCP application frameworks are, and how easily they integrate with GCP database, data-loss prevention, and security services.

[Baseline: Deploy & Develop](https://www.qwiklabs.com/quests/37?catalog_rank=%7B%22rank%22%3A4%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&search_id=7467936)


##### Deploying

The Google Cloud Platform provides many different frameworks and options to fit your application’s needs. In this introductory-level quest, you will get plenty of hands-on practice deploying sample applications on Google App Engine. You will also dive into other web application frameworks like Firebase, Wordpress, and Node.js and see firsthand how they can be integrated with GCP.

[Deploying Applications](https://www.qwiklabs.com/quests/26?catalog_rank=%7B%22rank%22%3A3%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&search_id=7467936)


##### Python Flask on App Engine Flexible

In this lab, you will learn how to deploy a Python Flask web application to the App Engine Flexible environment. The example application allows a user to upload a photo of a person's face and learn how likely it is that the person is happy. The application uses Google Cloud APIs for Vision, Storage, and Datastore.

[Deploying a Python Flask Web Application to App Engine Flexible](https://www.qwiklabs.com/focuses/3339?catalog_rank=%7B%22rank%22%3A24%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&parent=catalog&search_id=7467972)


##### Node.js Express

[Deploy Node.js Express Application in App Engine](https://www.qwiklabs.com/focuses/3340?catalog_rank=%7B%22rank%22%3A21%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&parent=catalog&search_id=7467972)


### Cloud Functions

Cloud Functions has a simple and intuitive developer experience. Just write your code and let Google Cloud handle the operational infrastructure. Develop faster by writing and running small code snippets that respond to events. Connect to Google Cloud or third-party cloud services via triggers to streamline challenging orchestration problems.

[https://cloud.google.com/functions](https://cloud.google.com/functions)

[https://cloud.google.com/functions/docs/functions-framework](https://cloud.google.com/functions/docs/functions-framework)


#### Qwiklabs


##### Cloud Functions & Dialogflow

[Google Assistant](https://assistant.google.com/#?modal_active=none) is a personal voice assistant that offers a host of actions and integrations. From making appointments and setting reminders, to ordering coffee and playing music, the 1 million+ actions available suit a wide range of voice command tasks. Google Assistant is offered on Android and iOS, but it can even be integrated with other devices like smartwatches, Google Homes, and Android TVs. [Actions](https://developers.google.com/actions/extending-the-assistant) is the central platform for developing Google Assistant applications. The Actions platform integrates with human-computer interaction suites, which simplifies conversational app development. The most widely used suite is [Dialogflow](https://dialogflow.com/), which uses an underlying machine learning (ML) and natural language understanding (NLU) schema to build rich Assistant applications. The Actions platform also integrates with [Cloud Functions](https://cloud.google.com/functions/), which lets you run backend fulfillment code in response to events triggered by Dialogflow requests. In this lab you will get hands-on practice with the Actions platform, the Dialogflow suite, and Cloud Functions by building a "Silly Name Maker" application, which returns a user with a silly name after they have entered in a lucky number and favorite color. You will build a Dialogflow agent that intelligently parses user input for specific information. The agent will be supplemented with a webhook, which will trigger a Cloud Function that handles fulfillment logic and returns your user with their silly name.

[Google Assistant: Build an Application with Dialogflow and Cloud Functions](https://www.qwiklabs.com/focuses/3634?catalog_rank=%7B%22rank%22%3A19%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&parent=catalog&search_id=7510653)


### Cloud GPUs

Compute Engine provides graphics processing units (GPUs) that you can add to your virtual machine instances. You can use these GPUs to accelerate specific workloads on your instances such as machine learning and data processing. If you have graphics-intensive workloads, such as 3D visualization, 3D rendering, or virtual applications, you can create virtual workstations that use NVIDIA® GRID® technology. For information on GPUs for graphics-intensive applications, see [GPUs for graphics workloads](https://cloud.google.com/compute/docs/gpus#gpu-virtual-workstations).

[https://cloud.google.com/compute/docs/gpus](https://cloud.google.com/compute/docs/gpus)

A video about using GPUs to accelerate and scale as needed.

[https://www.youtube.com/watch?v=l3_uE4gdAWc](https://www.youtube.com/watch?v=l3_uE4gdAWc)


### Preemptible VM Instances

A preemptible VM is an instance that you can create and run at a much [lower price](https://cloud.google.com/compute/vm-instance-pricing) than normal instances. However, Compute Engine might stop (preempt) these instances if it requires access to those resources for other tasks. Preemptible instances are excess Compute Engine capacity, so their availability varies with usage.

[https://cloud.google.com/compute/docs/instances/preemptible](https://cloud.google.com/compute/docs/instances/preemptible)

A video about bringing cost down using preemptible VMs.

[https://www.youtube.com/watch?v=ljol9IipvWs](https://www.youtube.com/watch?v=ljol9IipvWs)


### Shielded VMs

Shielded VM offers verifiable integrity of your Compute Engine VM instances, so you can be confident your instances haven't been compromised by boot- or kernel-level [malware](https://en.wikipedia.org/wiki/Malware) or [rootkits](https://en.wikipedia.org/wiki/Rootkit). Shielded VM's verifiable integrity is achieved through the use of [Secure Boot](https://cloud.google.com/security/shielded-cloud/shielded-vm#secure-boot), [virtual trusted platform module (vTPM)](https://cloud.google.com/security/shielded-cloud/shielded-vm#vtpm)-enabled [Measured Boot](https://cloud.google.com/security/shielded-cloud/shielded-vm#measured-boot), and [integrity monitoring](https://cloud.google.com/security/shielded-cloud/shielded-vm#integrity-monitoring).

[https://cloud.google.com/security/shielded-cloud/shielded-vm](https://cloud.google.com/security/shielded-cloud/shielded-vm)

How do you secure sensitive data and workloads in the cloud, while still keeping it private? In this video, we address just that, and show you how to create a shielded VM in Google Cloud Console, and how to ensure encryption in-use for workloads with Google Cloud Confidential Computing. 

[https://www.youtube.com/watch?v=o3NXEgbvdmQ](https://www.youtube.com/watch?v=o3NXEgbvdmQ)


### Sole-tenant nodes

Sole-tenancy lets you have exclusive access to a sole-tenant node, which is a physical Compute Engine server that is dedicated to hosting only your project's VMs. Use sole-tenant nodes to keep your VMs physically separated from VMs in other projects, or to group your VMs together on the same host hardware.

[https://cloud.google.com/compute/docs/nodes](https://cloud.google.com/compute/docs/nodes)

Sole-tenant nodes? VMaaS and CloudSimple? N1 vs N2 vs E2 instances? BYO Microsoft or Linux licenses? Understand how the choices available with Google Cloud can maximize your savings while expanding your migration scenarios. 

[https://www.youtube.com/watch?v=ocHadXq14v8](https://www.youtube.com/watch?v=ocHadXq14v8)


### Bare Metal Solution

Enterprises want to embrace the pace of innovation and an operational business model of the modern-day cloud, but they don’t want to disrupt their existing IT landscape or upgrade all their legacy applications. This presents a conundrum, as most legacy applications were not designed to run in the cloud, and migrating them can be challenging, risky, and cost-prohibitive.  Bare Metal Solution addresses these challenges by providing all the infrastructure you need to run your specialized workload such as Oracle Database close to Google Cloud. Learn how Bare Metal Solutions enable enterprises to migrate all such workloads to GCP in a simple, cost effective and secure way.

[https://www.youtube.com/watch?v=EVWrwCUQlL8](https://www.youtube.com/watch?v=EVWrwCUQlL8)

Documentation on Bare Metal solutions.

[https://cloud.google.com/bare-metal/docs](https://cloud.google.com/bare-metal/docs)


#### Configuring Google Access for On-Premise

Private Google Access for on-premises hosts provides a way for on-premises systems to connect to [Google APIs and services](https://developers.google.com/apis-explorer/) by routing traffic through a [Cloud VPN](https://cloud.google.com/network-connectivity/docs/vpn) tunnel or a [Cloud Interconnect](https://cloud.google.com/network-connectivity/docs/interconnect) attachment (VLAN). Private Google Access for on-premises hosts is an alternative to connecting to Google APIs and services over the internet.

[https://cloud.google.com/vpc/docs/configure-private-google-access-hybrid](https://cloud.google.com/vpc/docs/configure-private-google-access-hybrid)

Before migrating a portion of your environment to the Cloud, it is important to plan ahead for IP address changes that could affect your workloads. In this episode, Stephanie covers private and public IPs on Google Cloud and how you can achieve remappable IP addresses for your Cloud resources. 

[https://www.youtube.com/watch?v=QUb86NiMZ8k](https://www.youtube.com/watch?v=QUb86NiMZ8k)


### Compute Options

Every Cloud based application has needs specific to its environment, and Google Cloud offers a diverse set of options to run your code on. What option is right for you? 

[https://www.youtube.com/watch?v=2tLXKCgqwLY](https://www.youtube.com/watch?v=2tLXKCgqwLY)

Tables comparing different hosting options.

[https://cloud.google.com/hosting-options#comparing_options](https://cloud.google.com/hosting-options#comparing_options)

Decision tree for compute options.

[https://cloud.google.com/blog/products/gcp/choosing-the-right-compute-option-in-gcp-a-decision-tree?m=1](https://cloud.google.com/blog/products/gcp/choosing-the-right-compute-option-in-gcp-a-decision-tree?m=1)


## Containers


### What is a container?

A container is a standard unit of software that packages up code and all its dependencies so the application runs quickly and reliably from one computing environment to another. A Docker container image is a lightweight, standalone, executable package of software that includes everything needed to run an application: code, runtime, system tools, system libraries and settings.

[https://www.docker.com/resources/what-container](https://www.docker.com/resources/what-container)


#### Containers vs. VMs

Comparison of containerizing vs using VMs.

[https://www.youtube.com/watch?v=TvnZTi_gaNc](https://www.youtube.com/watch?v=TvnZTi_gaNc)


#### Three ways to run containers in GCP

Find out the top three ways you can run your containers on Google Cloud! Google Kubernetes Engine for a container orchestration solution, Cloud Run for a fully serverless approach and Compute Engine to simply use Virtual Machines.

[https://www.youtube.com/watch?v=jh0fPT-AWwM](https://www.youtube.com/watch?v=jh0fPT-AWwM)


### Namespaces

An overview of Linux namespaces and how they are used in containers.

[https://www.youtube.com/watch?v=kl8roLaLy-g](https://www.youtube.com/watch?v=kl8roLaLy-g)

Some videos about Network Namespaces and how they are used in containers.

[https://www.youtube.com/watch?v=j_UUnlVC2Ss&list=TLPQMTQxMDIwMjD4ry4yOmhx2w&index=2](https://www.youtube.com/watch?v=j_UUnlVC2Ss&list=TLPQMTQxMDIwMjD4ry4yOmhx2w&index=2)


### Google Kubernetes Engine (GKE)


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


#### How to create a GKE cluster

This video will teach you how to create a Google Kubernetes Engine (GKE) cluster using Terraform.

[https://www.youtube.com/watch?v=Vcv6GapxUCI](https://www.youtube.com/watch?v=Vcv6GapxUCI)


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


#### Configmaps & Secrets

[https://www.youtube.com/watch?v=FAnQTgr04mU](https://www.youtube.com/watch?v=FAnQTgr04mU)


#### Stateful Sets

[https://www.youtube.com/watch?v=pPQKAR1pA9U](https://www.youtube.com/watch?v=pPQKAR1pA9U)


#### DaemonSet

A DaemonSet ensures that all (or some) Nodes run a copy of a Pod. As nodes are added to the cluster, Pods are added to them. As nodes are removed from the cluster, those Pods are garbage collected. Deleting a DaemonSet will clean up the Pods it created.

[https://kubernetes.io/docs/concepts/workloads/controllers/daemonset/](https://kubernetes.io/docs/concepts/workloads/controllers/daemonset/)


#### CRD (Custom Resource Definition)

A resource is an endpoint in the [Kubernetes API](https://kubernetes.io/docs/reference/using-api/api-overview/) that stores a collection of [API objects](https://kubernetes.io/docs/concepts/overview/working-with-objects/kubernetes-objects/) of a certain kind; for example, the built-in pods resource contains a collection of Pod objects.

A custom resource is an extension of the Kubernetes API that is not necessarily available in a default Kubernetes installation. It represents a customization of a particular Kubernetes installation. However, many core Kubernetes functions are now built using custom resources, making Kubernetes more modular. Custom resources can appear and disappear in a running cluster through dynamic registration, and cluster admins can update custom resources independently of the cluster itself. Once a custom resource is installed, users can create and access its objects using [kubectl](https://kubernetes.io/docs/reference/kubectl/overview/), just as they do for built-in resources like Pods.

[https://kubernetes.io/docs/concepts/extend-kubernetes/api-extension/custom-resources/](https://kubernetes.io/docs/concepts/extend-kubernetes/api-extension/custom-resources/)


#### Operator Pattern

In [Kubernetes](https://opensource.com/resources/what-is-kubernetes), objects are analogous to a job or a completed task in the real world. You can use them to define common tasks, store them in a version control system, and apply them with kubectl apply. Kubernetes ensures that this triggers everything necessary to bring your declarative description to life by creating the dependent resources (like pods) to run your software. Kubernetes contains a number of built-in object types that can be created with this workflow, like Deployments and Services. With Operators, Kubernetes allows cluster maintainers or software providers to define their own Kubernetes object types, called custom resource definitions (CRDs). These objects can be handled by the Kubernetes API, just like built-in object types. Inside the Operator code, authors can define how to act on those custom objects. Operators are software extensions to Kubernetes that make use of [custom resources](https://kubernetes.io/docs/concepts/extend-kubernetes/api-extension/custom-resources/) to manage applications and their components. Operators follow Kubernetes principles, notably the [control loop](https://kubernetes.io/docs/concepts/architecture/controller).

[https://kubernetes.io/docs/concepts/extend-kubernetes/operator/](https://kubernetes.io/docs/concepts/extend-kubernetes/operator/)

[https://opensource.com/article/20/3/kubernetes-operator-sdk](https://opensource.com/article/20/3/kubernetes-operator-sdk)


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

Your organization has moved to microservices, then to Kubernetes. But now you have lots of workloads, and many different points of entry into your application. You've heard about how a service mesh can help with traffic management, so you've installed Istio and have explored the samples. Now what? This talk goes deep with Istio traffic routing, highlighting the features that can help your organization reduce complexity, improve performance, and scale to your customers' needs. Using a microservices application running on Google Kubernetes Engine, we will walk through exactly how to manage traffic with Istio. Demos will include load balancing, rollouts, ingress and egress, content-based routing, traffic mirroring, and resilience features such as circuit breaking. 

[https://www.youtube.com/watch?v=7cINRP0BFY8](https://www.youtube.com/watch?v=7cINRP0BFY8)

Istio provides a powerful set of Kubernetes abstractions for traffic routing, security, and telemetry. But whether you're a first-time user, or running Istio in production, it's likely that you've encountered some roadblocks when installing and using Istio. This talk dives into the most common problems you may encounter with Istio's internals, and addresses how to fix them. Through a whirlwind set of demos running on Google Kubernetes Engine, we will cover scenarios like: why does my Istio install fail? Why is Pilot crashing? what if my sidecar proxies aren't routing properly? what if I can't see Istio metrics in Stackdriver? Why is my end-user JWT authentication failing? why won't IngressGateway accept incoming traffic? — and more! 

[https://www.youtube.com/watch?v=FbYBO7Pi2d8](https://www.youtube.com/watch?v=FbYBO7Pi2d8)


##### Istiod vs microservices

[https://blog.christianposta.com/microservices/istio-as-an-example-of-when-not-to-do-microservices/](https://blog.christianposta.com/microservices/istio-as-an-example-of-when-not-to-do-microservices/)


#### Envoy

What if you could deploy hybrid/multi-cloud services seamlessly without having to build or operate the requisite services management infrastructure? What building blocks are available today and what does the road ahead look like? We bring together folks from Google Cloud and Lyft to answer these questions. Google/Google Cloud have decades plus experience in delivering production-grade services like Borg, Cloud Load Balancing, Kubernetes Engine and more recently driving Istio, a fast-growing open source platform for managing (micro)services. Lyft developed and open sourced Envoy, a high performance proxy aiming to make the network transparent to applications, and transformed its own monolithic app into a sophisticated Envoy-based ""service mesh"".

[https://www.youtube.com/watch?v=glATqKI-WR8](https://www.youtube.com/watch?v=glATqKI-WR8)


#### Apigee Envoy

Wanting to know how to use Envoy to protect your microservices? In this video, we give you a demo on how to enforce policies for any microservice within a service mesh via the Apigee adapter for Envoy. Watch to learn about this tool, and see if it’s the best choice for your specific use case! 

[https://www.youtube.com/watch?v=BNkfoZt-jvU](https://www.youtube.com/watch?v=BNkfoZt-jvU)


#### Ambassador Edge Stack and Consul Service Mesh

[https://www.youtube.com/watch?v=XW3AXQfAaQc](https://www.youtube.com/watch?v=XW3AXQfAaQc)


#### Linkerd

[https://www.youtube.com/watch?v=Bj7gGQUiDuk](https://www.youtube.com/watch?v=Bj7gGQUiDuk)


## Storage


### Introduction

Cloud Storage allows world-wide storage and retrieval of any amount of data at any time. You can use Cloud Storage for a range of scenarios including serving website content, storing data for archival and disaster recovery, or distributing large data objects to users via direct download.

[https://cloud.google.com/storage/docs](https://cloud.google.com/storage/docs)

What is Cloud Storage?

[https://www.youtube.com/watch?v=VDBhvexAj8I](https://www.youtube.com/watch?v=VDBhvexAj8I)

Different ways to upload your data.

[https://www.youtube.com/watch?v=nmZxfuFIP08](https://www.youtube.com/watch?v=nmZxfuFIP08)


#### GFS, Colossus

[https://en.wikipedia.org/wiki/Google_File_System](https://en.wikipedia.org/wiki/Google_File_System)


### Storage options

Compute Engine offers several types of storage options for your instances. Each of the following storage options has unique price and performance characteristics:



*   [Zonal persistent disk](https://cloud.google.com/compute/docs/disks#pdspecs): Efficient, reliable block storage.
*   [Regional persistent disk](https://cloud.google.com/compute/docs/disks#repds): Regional block storage replicated in two zones.
*   [Local SSD](https://cloud.google.com/compute/docs/disks#localssds): High performance, transient, local block storage.
*   [Cloud Storage buckets](https://cloud.google.com/compute/docs/disks#gcsbuckets): Affordable object storage.
*   [Filestore](https://cloud.google.com/filestore/docs/mounting-fileshares): High performance file storage for Google Cloud users.

[https://cloud.google.com/products/storage](https://cloud.google.com/products/storage)


#### Disk Options

[https://cloud.google.com/compute/docs/disks](https://cloud.google.com/compute/docs/disks)


#### Storage products

Overview and comparison of various Storage services and products on GCP.

[https://cloud.google.com/products/storage](https://cloud.google.com/products/storage)

Companies have a wide range of options to choose from when storing data and selecting a database in the cloud. Listen to an overview of data storage options, discuss why you would choose one over the other.

[https://www.youtube.com/watch?v=HuhTkfautDA](https://www.youtube.com/watch?v=HuhTkfautDA)


### Cloud Storage

This video walks you through how to upload a file and share it on Google Cloud Storage. 

[https://www.youtube.com/watch?v=TfOO-fSzTNA](https://www.youtube.com/watch?v=TfOO-fSzTNA)

How do  different types of buckets impact your performance? 

[https://www.youtube.com/watch?v=nCTiVwnnEhQ](https://www.youtube.com/watch?v=nCTiVwnnEhQ)


#### Storage Classes

The storage class you set for an object affects the object's availability and [pricing model](https://cloud.google.com/storage/pricing).

[https://cloud.google.com/storage/docs/storage-classes](https://cloud.google.com/storage/docs/storage-classes)


### Persistent Disk

Reliable, high-performance block storage for virtual machine instances.

[https://www.youtube.com/watch?v=zovhVfou-DI](https://www.youtube.com/watch?v=zovhVfou-DI)


### Filestore

Filestore instances are fully managed [NFS](https://en.wikipedia.org/wiki/Network_File_System) file servers on Google Cloud (GCP) for use with applications running on Compute Engine virtual machines (VMs) instances or Google Kubernetes Engine clusters.

[https://www.youtube.com/watch?v=8rS8O2RiT80](https://www.youtube.com/watch?v=8rS8O2RiT80)

You can create and manage Filestore instances by using the Google Cloud Console or the gcloud command-line tool, and interact with the NFS file share on the instance by using standard operating system commands.

[https://cloud.google.com/filestore/docs](https://cloud.google.com/filestore/docs)


#### Backups

[https://cloud.google.com/blog/products/storage-data-transfer/introducing-filestore-backups](https://cloud.google.com/blog/products/storage-data-transfer/introducing-filestore-backups)


### Cloud Storage Connector

The [Cloud Storage](https://cloud.google.com/storage) connector is an [open source Java library](https://github.com/GoogleCloudDataproc/hadoop-connectors/tree/master/gcs) that lets you run [Apache Hadoop](https://hadoop.apache.org/) or [Apache Spark](https://spark.apache.org/) jobs directly on data in Cloud Storage, and offers a number of benefits over choosing the Hadoop Distributed File System (HDFS).

[https://cloud.google.com/dataproc/docs/concepts/connectors/cloud-storage](https://cloud.google.com/dataproc/docs/concepts/connectors/cloud-storage)


## Data Engineering


### Overview

[https://www.youtube.com/watch?v=tc2940Zwvyk](https://www.youtube.com/watch?v=tc2940Zwvyk)


### Database options

One of Google Cloud Platform's competitive advantages is the strong ecosystem of managed databases.  However, the wealth of options can be confusing to navigate as you look for the right technologies to grow your product.  This is a video about picking the right databases for your tech stack and how to make it all work in a unified way.

[https://www.youtube.com/watch?v=3aHBkfBRFEU](https://www.youtube.com/watch?v=3aHBkfBRFEU)

Choosing the right database for your workloads.

[https://www.youtube.com/watch?v=3YnLuEdGzU8](https://www.youtube.com/watch?v=3YnLuEdGzU8)

Compare different GCP Database services.

[https://cloud.google.com/products/databases](https://cloud.google.com/products/databases)


### Cloud SQL

Cloud SQL is a fully-managed database service that helps you set up, maintain, manage, and administer your relational databases on Google Cloud Platform.

You can use Cloud SQL with [MySQL](https://cloud.google.com/sql/docs/mysql), [PostgreSQL](https://cloud.google.com/sql/docs/postgres), or [SQL Server](https://cloud.google.com/sql/docs/sqlserver). 

[https://cloud.google.com/sql/docs](https://cloud.google.com/sql/docs)

[https://www.youtube.com/watch?v=OvR2KX8GVtU](https://www.youtube.com/watch?v=OvR2KX8GVtU)


### SQL


#### Tutorials

[https://www.youtube.com/watch?v=HXV3zeQKqGY](https://www.youtube.com/watch?v=HXV3zeQKqGY)

[https://www.freecodecamp.org/news/best-sql-database-tutorial/](https://www.freecodecamp.org/news/best-sql-database-tutorial/)


### Cloud Bigtable


#### Introduction

Cloud Bigtable is Google's NoSQL Big Data database service. It's the same database that powers many core Google services, including Search, Analytics, Maps, and Gmail.

[https://cloud.google.com/bigtable/docs](https://cloud.google.com/bigtable/docs)

Handle massive amounts of data workload with Cloud Bigtable.

[https://www.youtube.com/watch?v=MzT0c0l3RPc](https://www.youtube.com/watch?v=MzT0c0l3RPc)

Discuss the differences between Cassandra and Cloud Bigtable, why and how Spotify migrated some of their workloads, and how they built an auto-scaler for Cloud Bigtable.

[https://www.youtube.com/watch?v=Hfd3VZOYXNU](https://www.youtube.com/watch?v=Hfd3VZOYXNU)

Global Data Services with Bigtable.

[https://www.youtube.com/watch?v=dHr707_6woY](https://www.youtube.com/watch?v=dHr707_6woY)

Bigtable and Spanner.

[https://www.youtube.com/watch?v=_Qm0eopwjG0](https://www.youtube.com/watch?v=_Qm0eopwjG0)


#### HBase

This page lists differences between Bigtable and HBase. 

[https://cloud.google.com/bigtable/docs/hbase-differences](https://cloud.google.com/bigtable/docs/hbase-differences)


#### SSTable, LSM Tree, LevelDB

[https://www.igvita.com/2012/02/06/sstable-and-log-structured-storage-leveldb/](https://www.igvita.com/2012/02/06/sstable-and-log-structured-storage-leveldb/)


#### Qwiklabs


##### Hbase

One way to communicate with Cloud Bigtable is through the Cloud Bigtable HBase client for Java, which is a customized version of the [Apache HBase](https://hbase.apache.org/) client. The Cloud Bigtable HBase client for Java enables you to write Java applications that communicate with Cloud Bigtable through the open-source [HBase API](https://hbase.apache.org/apidocs/). The client is compatible with versions 1.0.x, 1.1.x, 1.2.x, and 1.3.x of the HBase API.

[Bigtable: Qwik Start - Hbase Shell](https://www.qwiklabs.com/focuses/580?catalog_rank=%7B%22rank%22%3A1%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&parent=catalog&search_id=7500925)


##### Bigtable

Cloud Bigtable is a sparsely populated table that can scale to billions of rows and thousands of columns, enabling you to store terabytes or even petabytes of data. A single value in each row is indexed; this value is known as the row key. Cloud Bigtable is ideal for storing very large amounts of single-keyed data with very low latency. It supports high read and write throughput at low latency, and it is an ideal data source for MapReduce operations.

Cloud Bigtable is exposed to applications through multiple client libraries, including a supported extension to the [Apache HBase library for Java](https://hbase.apache.org/). As a result, it integrates with the existing Apache ecosystem of open-source Big Data software.

[Intro to Bigtable](https://cloud.google.com/bigtable/docs) 


##### Cloud Bigtable Command line

In this lab you'll learn how to use the cbt command line to connect to a Cloud Bigtable instance, perform basic administrative tasks, and read and write data in a table.

[Bigtable: Qwik Start - Command Line](https://www.qwiklabs.com/focuses/579?catalog_rank=%7B%22rank%22%3A1%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&parent=catalog&search_id=7467646)


##### OpenTSDB

In this lab you will learn how to collect, record, and monitor [time-series data](https://en.wikipedia.org/wiki/Time_series) on Google Cloud using [OpenTSDB](http://opentsdb.net/) running on [Google Kubernetes Engine](https://cloud.google.com/kubernetes-engine/) and [Cloud Bigtable](https://cloud.google.com/bigtable/).

[Using OpenTSDB to Monitor Time-Series Data on Cloud Platform](https://www.qwiklabs.com/focuses/629?catalog_rank=%7B%22rank%22%3A3%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&parent=catalog&search_id=7467646)


##### Cryptocurrency Trading 

Currently, using an [econometric](https://www.investopedia.com/terms/e/econometrics.asp) approach—applying models to financial data to forecast future trends—doesn’t work for real-time financial predictions. And data that’s old, inaccurate or from a single source doesn’t translate into dependable data for financial institutions to use. But building pipelines with Google Cloud Platform (GCP) can solve some of these key challenges. In this lab, we’ll describe how to build a pipeline to predict financial trends in microseconds. We’ll walk through how to set up and configure a pipeline for ingesting real-time, time-series data from various financial exchanges and how to design a suitable data model, which facilitates querying and graphing at scale.

[Tracking Cryptocurrency Exchange Trades with Google Cloud Platform in Real-Time](https://www.qwiklabs.com/focuses/5570?catalog_rank=%7B%22rank%22%3A8%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&parent=catalog&search_id=7467646)


### Cloud Dataproc


#### Introduction

Dataproc is a managed [Apache Spark](https://spark.apache.org/) and [Apache Hadoop](https://hadoop.apache.org/) service that lets you take advantage of open source data tools for batch processing, querying, streaming, and machine learning. Dataproc automation helps you create clusters quickly, manage them easily, and save money by turning clusters off when you don't need them. With less time and money spent on administration, you can focus on your jobs and your data.

[https://cloud.google.com/dataproc/docs](https://cloud.google.com/dataproc/docs)

Enterprises are migrating their existing on-premises Apache Hadoop and Spark clusters over to Dataproc to manage costs and unlock the power of elastic scale. With Dataproc, enterprises get a fully managed, purpose-built cluster that can autoscale to support any data or analytics processing job. 

[https://cloud.google.com/dataproc/docs/tutorials](https://cloud.google.com/dataproc/docs/tutorials)

See how to use Cloud Dataproc to manage Apache Spark and Hadoop in an easy, cost-effective way. Try the Dataproc: Qwik Start lab here:[ http://bit.ly/2KZaZJM](https://www.youtube.com/redirect?q=http%3A%2F%2Fbit.ly%2F2KZaZJM&v=h1LvACJWjKc&redir_token=QUFFLUhqbXk5SU9PTlVJMDY1SHdmOV8zbF92U29rUGFvQXxBQ3Jtc0tsQU1ZZENDa1U4cnVLX3NCeS1wXzFNOEdYVDFueGcybmI5NTBuWWMtUkp2bWd0YUtQTUlfQTdqWGRNZFBNdzhVeGZnb0diUDRSR1RoNk5RTFlWX3FnZ3JJQlA1cHJiWE1HUkhNTmFtM1pDR1ZaSmh6dw%3D%3D&event=video_description)

[https://www.youtube.com/watch?v=h1LvACJWjKc](https://www.youtube.com/watch?v=h1LvACJWjKc)

Run Spark and Hadoop faster with Dataproc.

[https://www.youtube.com/watch?v=h1LvACJWjKc](https://www.youtube.com/watch?v=h1LvACJWjKc)


#### Big Data analytics with Dataproc

[https://programmaticponderings.com/2018/12/11/big-data-analytics-with-java-and-python-using-cloud-dataproc-googles-fully-managed-spark-and-hadoop-service/](https://programmaticponderings.com/2018/12/11/big-data-analytics-with-java-and-python-using-cloud-dataproc-googles-fully-managed-spark-and-hadoop-service/)


#### Migrating Hadoop to GCP

[https://www.youtube.com/watch?v=YK_-yS9y_0k](https://www.youtube.com/watch?v=YK_-yS9y_0k)


#### Basic introduction to Apache Hadoop

[https://www.youtube.com/watch?v=OoEpfb6yga8](https://www.youtube.com/watch?v=OoEpfb6yga8)


#### Apache Spark Tutorial

[https://www.youtube.com/watch?v=IQfG0faDrzE4](https://www.youtube.com/watch?v=IQfG0faDrzE4)  


##### A Scala tutorial for Java programmers

[https://docs.scala-lang.org/tutorials/scala-for-java-programmers.html](https://docs.scala-lang.org/tutorials/scala-for-java-programmers.html)


#### Some online courses to learn Hadoop and Spark.

[https://medium.com/swlh/5-free-online-courses-to-learn-big-data-hadoop-and-spark-in-2019-a553e6ccfe30](https://medium.com/swlh/5-free-online-courses-to-learn-big-data-hadoop-and-spark-in-2019-a553e6ccfe30)


#### Using Apache Hive on Cloud Dataproc

[https://cloud.google.com/solutions/using-apache-hive-on-cloud-dataproc](https://cloud.google.com/solutions/using-apache-hive-on-cloud-dataproc)


#### Spark by Example

[https://sparkbyexamples.com/](https://sparkbyexamples.com/)


##### Main Spark github source tree

[https://github.com/apache/spark](https://github.com/apache/spark)


##### Spark examples source code

[https://github.com/apache/spark/tree/master/examples/src/main](https://github.com/apache/spark/tree/master/examples/src/main)


#### Hadoop Data Storage

Dataproc integrates with Apache Hadoop and the Hadoop Distributed File System (HDFS). 

[https://cloud.google.com/dataproc/docs/concepts/dataproc-hdfs](https://cloud.google.com/dataproc/docs/concepts/dataproc-hdfs)


#### Hive

[Apache Hive](https://hive.apache.org/) is a data warehouse software project built on top of Apache Hadoop for providing data query and analysis. 

[https://www.youtube.com/watch?v=cMziv1iYt28](https://www.youtube.com/watch?v=cMziv1iYt28)


#### Pig vs SQL


##### Hadoop Pig 

[Apache Pig](http://pig.apache.org/) is a platform for analyzing large data sets that consists of a high-level language for expressing data analysis programs, coupled with infrastructure for evaluating these programs.

[https://www.youtube.com/watch?v=Hve24pRW_Ps](https://www.youtube.com/watch?v=Hve24pRW_Ps) \


Hive vs. Pig vs. SQL.

[https://www.whizlabs.com/blog/hive-vs-pig-vs-sql/](https://www.whizlabs.com/blog/hive-vs-pig-vs-sql/)


#### Pig Latin SQL Challenge

Doing ETL in SQL or [Pig Latin](https://pig.apache.org/docs/latest/basic.html) to give more detailed feel for why one might prefer one or the other in solving actual common problems:

[http://www.olric.org/2019/09/pig-latin-sql-challenge-or-window.html?m=1](http://www.olric.org/2019/09/pig-latin-sql-challenge-or-window.html?m=1)


##### Sawzall

A perspective on Sawzall DSL (domain specific language) over Google map/reduce and Pig DSL over Hadoop map/reduce.

[http://glinden.blogspot.com/2007/04/yahoo-pig-and-google-sawzall.html?m=1](http://glinden.blogspot.com/2007/04/yahoo-pig-and-google-sawzall.html?m=1)

And finally a perspective on replacing Sawzell within Google.

[http://www.unofficialgoogledatascience.com/2015/12/replacing-sawzall-case-study-in-domain.html?m=1](http://www.unofficialgoogledatascience.com/2015/12/replacing-sawzall-case-study-in-domain.html?m=1)


#### Qwiklabs


##### Spark Scala Jobs on Dataproc

[Write Spark Scala Jobs (From Spark to DataProc)](https://cloud.google.com/dataproc/docs/tutorials/spark-scala)


##### Moving from Hadoop to GCP

[Hadoop to GCP](https://cloud.google.com/blog/products/data-analytics/goodbye-hadoop-building-a-streaming-data-processing-pipeline-on-google-cloud) 


### Cloud Pub/Sub


#### What is Cloud Pub/Sub

Cloud Pub/Sub is a fully-managed real-time messaging service that allows you to send and receive messages between independent applications.

[https://cloud.google.com/pubsub/docs](https://cloud.google.com/pubsub/docs)

This video walks you through how to create a Google Cloud Pub/Sub topic. Pub/Sub allows you to create global real-time messaging and subscribe to topics you want to follow to stay up to date.

[https://www.youtube.com/watch?v=pU1zA-DMlWk](https://www.youtube.com/watch?v=pU1zA-DMlWk)


#### Example

Cloud IoT Core to push airline data to PubSub, Dataflow, and BigQuery.

[https://www.youtube.com/watch?v=-y3s6XY70Os](https://www.youtube.com/watch?v=-y3s6XY70Os)


#### A list of task queues

[https://taskqueues.com/](https://taskqueues.com/)


#### Kafka

[Apache Kafka](https://kafka.apache.org/) is an open-source distributed event streaming platform used by thousands of companies for high-performance data pipelines, streaming analytics, data integration, and mission-critical applications.

[https://kafka.apache.org/](https://kafka.apache.org/)

Kafka is open source. You can see its implementation: 

[https://github.com/apache/kafka](https://github.com/apache/kafka)

Review some  examples:

[https://github.com/apache/kafka/tree/trunk/examples/src/main/java/kafka/examples](https://github.com/apache/kafka/tree/trunk/examples/src/main/java/kafka/examples)

Using Kafka and Confluent allows customers to integrate legacy systems and Google services like BigQuery and Dataflow in real time. 

[https://www.youtube.com/watch?v=LjF8IqKKbWc](https://www.youtube.com/watch?v=LjF8IqKKbWc)


#### Qwiklabs


##### Cloud Pub/Sub

[Google Cloud Pub/Sub: Qwik Start - Python](https://www.qwiklabs.com/focuses/2775?catalog_rank=%7B%22rank%22%3A4%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&parent=catalog&search_id=7524031)


##### Kafka

Organizations around the world rely on Apache Kafka to integrate existing systems in real time and build a new class of event streaming applications that unlock new business opportunities. Google and Confluent are in a partnership to deliver the best event streaming service based on Apache Kafka and to build event driven applications and big data pipelines on Google Cloud Platform. In this Quest, you will first learn how to deploy and create a streaming data pipeline with Apache Kafka. You will then perform hand-on labs on the different functionalities of the Confluent Platform such as deploying and running Apache Kafka on GKE, building a Cloud Run Streaming Application with Apache Kafka on Anthos or developing a Streaming Microservices Application.

[Getting Started with Apache Kafka and Confluent Platform on Google Cloud](https://www.qwiklabs.com/quests/145?catalog_rank=%7B%22rank%22%3A1%2C%22num_filters%22%3A1%2C%22has_search%22%3Atrue%7D&search_id=7467576)


### BigQuery


#### Introduction

BigQuery is Google Cloud's fully managed, petabyte-scale, and cost-effective analytics data warehouse that lets you run analytics over vast amounts of data in near real time. With BigQuery, there's no infrastructure to set up or manage, letting you focus on finding meaningful insights using standard SQL and taking advantage of flexible pricing models across on-demand and flat-rate options.

[https://www.google.com/amp/s/cloudblog.withgoogle.com/products/data-analytics/new-blog-series-bigquery-explained-overview/amp/](https://www.google.com/amp/s/cloudblog.withgoogle.com/products/data-analytics/new-blog-series-bigquery-explained-overview/amp/)

[https://cloud.google.com/bigquery/docs](https://cloud.google.com/bigquery/docs)

BigQuery is designed to ingest and store large amounts of data, and make that data accessible for fast, large-scale analytics - to help analysts and developers alike. 

[https://www.youtube.com/watch?v=d3MDxC_iuaw](https://www.youtube.com/watch?v=d3MDxC_iuaw)

How to load CSV data in batch, and analyze your own data in BigQuery.

[https://www.youtube.com/watch?v=Abzj-Vyhi74](https://www.youtube.com/watch?v=Abzj-Vyhi74)


#### BigQuery 101

[https://www.youtube.com/watch?v=kKBnFsNWwYM](https://www.youtube.com/watch?v=kKBnFsNWwYM)


##### Data warehousing with BigQuery

[https://cloud.google.com/solutions/bigquery-data-warehouse](https://cloud.google.com/solutions/bigquery-data-warehouse)


##### BigQuery Explained

[https://cloud.google.com/blog/topics/developers-practitioners/bigquery-explained-blog-series](https://cloud.google.com/blog/topics/developers-practitioners/bigquery-explained-blog-series)

[https://www.youtube.com/watch?v=ZVgt1-LfWW4](https://www.youtube.com/watch?v=ZVgt1-LfWW4)

Most experienced data analysts and programmers already have the skills to get started. BigQuery is fully managed and lets you search through terabytes of data in seconds. It’s also cost effective: you can store gigabytes, terabytes, or even petabytes of data.

[https://www.youtube.com/watch?v=qqbYrQGSibQ](https://www.youtube.com/watch?v=qqbYrQGSibQ)


#### BigQuery under the hood

[https://cloud.google.com/blog/products/gcp/bigquery-under-the-hood](https://cloud.google.com/blog/products/gcp/bigquery-under-the-hood)


##### Loading Data into BigQuery

[https://cloud.google.com/bigquery/docs/loading-data](https://cloud.google.com/bigquery/docs/loading-data)


##### Anatomy of a BigQuery query

[https://cloud.google.com/blog/products/gcp/anatomy-of-a-bigquery-query](https://cloud.google.com/blog/products/gcp/anatomy-of-a-bigquery-query)


##### In memory query execution

[https://cloud.google.com/blog/products/gcp/in-memory-query-execution-in-google-bigquery](https://cloud.google.com/blog/products/gcp/in-memory-query-execution-in-google-bigquery)


##### Query plan and timeline

[https://cloud.google.com/bigquery/query-plan-explanation](https://cloud.google.com/bigquery/query-plan-explanation)


##### Managing input data and data sources

[https://cloud.google.com/bigquery/docs/best-practices-performance-input](https://cloud.google.com/bigquery/docs/best-practices-performance-input)


##### Optimizing communication between slots

[https://cloud.google.com/bigquery/docs/best-practices-performance-communication](https://cloud.google.com/bigquery/docs/best-practices-performance-communication)


##### Optimizing query computation

[https://cloud.google.com/bigquery/docs/best-practices-performance-compute](https://cloud.google.com/bigquery/docs/best-practices-performance-compute)


##### Managing materialization and outputs

[https://cloud.google.com/bigquery/docs/best-practices-performance-output](https://cloud.google.com/bigquery/docs/best-practices-performance-output)


##### Anti patterns

[https://cloud.google.com/bigquery/docs/best-practices-performance-patterns](https://cloud.google.com/bigquery/docs/best-practices-performance-patterns)


##### Dremel

Dremel is a scalable, interactive ad-hoc query system for analysis of read-only nested data. BigQuery is based on Dremel.

[https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/36632.pdf](https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/36632.pdf)


##### Building the world’s largest data warehouse

[https://www.youtube.com/watch?v=1gYUGv_omJA](https://www.youtube.com/watch?v=1gYUGv_omJA)


##### BigQuery nested and repeated fields

[https://www.youtube.com/watch?v=STo98QUKDS8](https://www.youtube.com/watch?v=STo98QUKDS8)


#### BigQuery tutorials

[https://cloud.google.com/bigquery/docs/tutorials](https://cloud.google.com/bigquery/docs/tutorials)


##### Learn writing java code to connect Dataproc map/reduce to BigQuery

[https://cloud.google.com/dataproc/docs/tutorials/bigquery-connector-mapreduce-example](https://cloud.google.com/dataproc/docs/tutorials/bigquery-connector-mapreduce-example)


##### BigQuery connector to Spark

[https://cloud.google.com/dataproc/docs/tutorials/bigquery-connector-spark-example](https://cloud.google.com/dataproc/docs/tutorials/bigquery-connector-spark-example)


#### Data Warehouse Topics


##### BigQuery, Snowflake, Redshift

[https://medium.com/2359media/redshift-vs-bigquery-vs-snowflake-a-comparison-of-the-most-popular-data-warehouse-for-data-driven-cb1c10ac8555](https://medium.com/2359media/redshift-vs-bigquery-vs-snowflake-a-comparison-of-the-most-popular-data-warehouse-for-data-driven-cb1c10ac8555)


##### Snowflake, Star, Galaxy

Star Schema in a data warehouse, in which the center of the star can have one fact table and a number of associated dimension tables. It is known as star schema as its structure resembles a star. The Star Schema data model is the simplest type of Data Warehouse schema. It is also known as Star Join Schema and is optimized for querying large data sets.

Snowflake Schema in a data warehouse is a logical arrangement of tables in a multidimensional database such that the [ER diagram](https://www.guru99.com/er-diagram-tutorial-dbms.html) resembles a snowflake shape. A Snowflake Schema is an extension of a Star Schema, and it adds additional dimensions. The dimension tables are normalized which splits data into additional tables.

A Galaxy Schema contains two fact table that share dimension tables between them. It is also called Fact Constellation Schema. The schema is viewed as a collection of stars hence the name Galaxy Schema.

[https://www.guru99.com/star-snowflake-data-warehousing.html](https://www.guru99.com/star-snowflake-data-warehousing.html)


##### Denormalization

[https://en.wikipedia.org/wiki/Denormalization](https://en.wikipedia.org/wiki/Denormalization)


#### Public Datasets

[https://cloud.google.com/bigquery/public-data](https://cloud.google.com/bigquery/public-data)


#### BigQuery Standard SQL

[https://cloud.google.com/bigquery/docs/reference/standard-sql/migrating-from-legacy-sql](https://cloud.google.com/bigquery/docs/reference/standard-sql/migrating-from-legacy-sql)


#### Qwiklabs


##### Data Analysts

BigQuery uses SQL and can take advantage of the pay-as-you-go model. BigQuery allows you to focus on analyzing data to find meaningful insights.

[BigQuery Basics for Data Analysts](https://www.qwiklabs.com/quests/69?catalog_rank=%7B%22rank%22%3A8%2C%22num_filters%22%3A1%2C%22has_search%22%3Atrue%7D&search_id=7467580)

GSP340

A favorite BigQuery challenge on Covid-19 public data sources

[https://www.qwiklabs.com/focuses/14341?parent=catalog](https://www.qwiklabs.com/focuses/14341?parent=catalog)


##### Data Warehousing

Looking to build or optimize your data warehouse? Learn best practices to Extract, Transform, and Load your data into Google Cloud with BigQuery. 

[Build and Optimize Data Warehouses with BigQuery](https://www.qwiklabs.com/quests/147?catalog_rank=%7B%22rank%22%3A1%2C%22num_filters%22%3A1%2C%22has_search%22%3Atrue%7D&search_id=7467580)


##### Marketing Analysts

Want to turn your marketing data into insights and build dashboards? Bring all of your data into one place for large-scale analysis and model building.

[BigQuery for Marketing Analysts](https://www.qwiklabs.com/quests/70?catalog_rank=%7B%22rank%22%3A2%2C%22num_filters%22%3A1%2C%22has_search%22%3Atrue%7D&search_id=7467580)


##### Machine Learning

Want to learn and practice machine learning and build models in minutes instead of hours using just SQL? BigQuery Machine Learning is a new feature in BigQuery where data analysts can create, train, evaluate, and predict machine learning models with minimal coding. In this series of labs you will experiment with different model types and learn what makes a good model.

[BigQuery for Machine Learning](https://www.qwiklabs.com/quests/71?catalog_rank=%7B%22rank%22%3A3%2C%22num_filters%22%3A1%2C%22has_search%22%3Atrue%7D&search_id=7467580)


##### Data Warehousing Optimization

In this series of interactive labs you will create and optimize your own data warehouse using a variety of large-scale BigQuery public datasets. 

[BigQuery for Data Warehousing](https://www.qwiklabs.com/quests/68?catalog_rank=%7B%22rank%22%3A4%2C%22num_filters%22%3A1%2C%22has_search%22%3Atrue%7D&search_id=7467580)


##### Insights from Data

Learn the best practices for querying and getting insights from your data warehouse with this interactive series of BigQuery labs. 

A favorite lab.

[Insights from Data with BigQuery](https://www.qwiklabs.com/quests/123?catalog_rank=%7B%22rank%22%3A5%2C%22num_filters%22%3A1%2C%22has_search%22%3Atrue%7D&search_id=7467580)


##### Create ML Models

Want to build ML models in minutes instead of hours using just SQL? BigQuery ML democratizes machine learning by letting data analysts create, train, evaluate, and predict with machine learning models using existing SQL tools and skills. 

[Create ML Models with BigQuery ML](https://www.qwiklabs.com/quests/146?catalog_rank=%7B%22rank%22%3A7%2C%22num_filters%22%3A1%2C%22has_search%22%3Atrue%7D&search_id=7467580)


##### March Madness

In this series of labs you will learn how to use BigQuery to analyze NCAA basketball data with SQL. Build a Machine Learning Model to predict the outcomes of NCAA March Madness basketball tournament games.

 \
[NCAA® March Madness®: Bracketology with Google Cloud](https://www.qwiklabs.com/quests/58?catalog_rank=%7B%22rank%22%3A9%2C%22num_filters%22%3A1%2C%22has_search%22%3Atrue%7D&search_id=7467580)


##### Scientific Data Processing

Big data, machine learning, and scientific data? It sounds like the perfect match. In this advanced-level quest, you will get hands-on practice with GCP services like Big Query, Dataproc, and TensorFlow by applying them to use cases that employ real-life, scientific data sets. By getting experience with tasks like earthquake data analysis and satellite image aggregation, Scientific Data Processing will expand your skill set in big data and machine learning so you can start tackling your own problems across a spectrum of scientific disciplines.

[Scientific Data Processing](https://www.qwiklabs.com/quests/28?catalog_rank=%7B%22rank%22%3A1%2C%22num_filters%22%3A1%2C%22has_search%22%3Atrue%7D&search_id=7467566)


##### Analyzing Natality Data Using AI Platform and BigQuery

A favorite lab.

This lab illustrates how you can carry out data exploration of large datasets, but continue to use familiar tools like Pandas and Jupyter. The trick is to do the first part of your aggregation in BigQuery, get back a Pandas DataFrame, then work with the smaller Pandas DataFrame locally. AI Platform provides a managed Jupyter experience, so you don't need to run notebook servers yourself.

[https://google.qwiklabs.com/focuses/604?parent=catalog](https://google.qwiklabs.com/focuses/604?parent=catalog)


##### Weather data in BigQuery

A favorite lab.

This lab uses two public datasets in BigQuery: weather data from NOAA and citizen complaints data from New York City.  Interestingly, you will find what types of municipal complaints are correlated with weather. For example, you will find (not surprisingly) that complaints about residential furnaces are most common when it is cold outside.

[https://google.qwiklabs.com/focuses/609?parent=catalog](https://google.qwiklabs.com/focuses/609?parent=catalog)


### Cloud Spanner


#### Introduction 

Cloud Spanner is a fully managed, mission-critical, relational database service that offers transactional consistency at global scale, schemas, SQL (ANSI 2011 with extensions), and automatic, synchronous replication for high availability.

[https://cloud.google.com/spanner/docs](https://cloud.google.com/spanner/docs)

Original paper on Spanner. 

[https://static.googleusercontent.com/media/research.google.com/en//archive/spanner-osdi2012.pdf](https://static.googleusercontent.com/media/research.google.com/en//archive/spanner-osdi2012.pdf)


#### External Consistency, Linearizability, Serializability

Cloud Spanner provides clients with the strictest concurrency-control guarantees for transactions, which is called external consistency. Under external consistency, the system behaves as if all transactions were executed sequentially, even though Cloud Spanner actually runs them across multiple servers (and possibly in multiple datacenters) for higher performance and availability. In addition if one transaction completes before another transaction starts to commit, the system guarantees that clients can never see a state that includes the effect of the second transaction but not the first. Intuitively, Cloud Spanner is semantically indistinguishable from a single-machine database. Even though it provides such strong guarantees, Cloud Spanner enables applications to achieve performance comparable to databases that provide weaker guarantees. 

Cloud Spanner provides external consistency, which is a stronger property than linearizability, because linearizability does not say anything about the behavior of transactions.

Linearizability is a property of concurrent objects that support atomic read and write operations. In a database, an "object" would typically be a single row or even a single cell. External consistency is a property of transaction-processing systems, where clients dynamically synthesize transactions that contain multiple read and write operations on arbitrary objects. Linearizability can be viewed as a special case of external consistency, where a transaction can only contain a single read or write operation on a single object.

Cloud Spanner provides external consistency, which is a stricter property than serializability. A transaction-processing system is serializable if it executes transactions in a manner that is indistinguishable from a system in which the transactions are executed serially. Cloud Spanner also guarantees that the serial order is consistent with the order in which the transactions can be observed to commit.

 In a system that provides serializability but not external consistency, even though the customer executed T1 and then T2 sequentially, the system would be permitted to reorder them, which could cause the debit to incur a penalty due to insufficient funds.


#### TrueTime

TrueTime is a highly available, distributed clock that is provided to applications on all Google servers. TrueTime enables applications to generate monotonically increasing timestamps: an application can compute a timestamp T that is guaranteed to be greater than any timestamp T' if T' finished being generated before T started being generated. This guarantee holds across all servers and all timestamps.

[https://cloud.google.com/spanner/docs/true-time-external-consistency](https://cloud.google.com/spanner/docs/true-time-external-consistency)


#### Cloud Spanner 101

[https://www.youtube.com/watch?v=IfsTINNCooY](https://www.youtube.com/watch?v=IfsTINNCooY)

Cloud Spanner is a fully managed relational database with unlimited scale, strong consistency, and up to 99.999% availability. Cloud Spanner can help you create time-sensitive, mission critical applications at scale. 

[https://www.youtube.com/watch?v=5bjYk6Hhd10](https://www.youtube.com/watch?v=5bjYk6Hhd10)

Build  an inventory ledger solution that streamlines the order-to-shipping process using Cloud Spanner, a scalable, globally consistent database service. The single source of truth enables seamless customer experiences across channels and real-time decisioning at scale. 

[https://www.youtube.com/watch?v=8kj_uA5vJfo](https://www.youtube.com/watch?v=8kj_uA5vJfo)


#### Tutorials

[https://cloud.google.com/spanner/docs/tutorials](https://cloud.google.com/spanner/docs/tutorials)


#### Perspectives

A Shift to Distributed SQL.

[https://medium.com/@garyorenstein/the-shift-to-distributed-sql-232c04dec1f7](https://medium.com/@garyorenstein/the-shift-to-distributed-sql-232c04dec1f7)

Databases, ETL, ELT and tools.

[https://cube.dev/blog/category/data-stack/](https://cube.dev/blog/category/data-stack/)


#### Qwiklabs


##### Quick Start

[Cloud Spanner: Qwik Start](https://www.qwiklabs.com/focuses/1774?catalog_rank=%7B%22rank%22%3A1%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&parent=catalog&search_id=7467628)


##### Java Client

In this lab, you will set up a Cloud Spanner instance, create a database and schema, then run sample queries on a dataset. Helpful Cloud Spanner information is provided along the way to help you get the most out of this powerful database service.

[Querying Cloud Spanner With a Java Client](https://www.qwiklabs.com/focuses/2189?catalog_rank=%7B%22rank%22%3A3%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&parent=catalog&search_id=7467628)


##### Leaderboard

In this lab, you will learn how to set up a Cloud Spanner instance. You will go through the steps of creating a database and schema that can be used for a gaming leaderboard. You'll start by creating a Players table for storing player information and a Scores table to store player scores.

[Cloud Spanner: Create a Gaming Leaderboard with C#](https://www.qwiklabs.com/focuses/1815?catalog_rank=%7B%22rank%22%3A4%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&parent=catalog&search_id=7467628)


##### Backend

In this lab, you develop a backend service for an online Quiz application to process user feedback and save scores.

[App Dev: Developing a Backend Service - Java](https://www.qwiklabs.com/focuses/1128?catalog_rank=%7B%22rank%22%3A9%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&parent=catalog&search_id=7467628)


##### Python

This lab concentrates on the backend service, putting together Pub/Sub, Natural Language, and Spanner services and APIs to collect and analyze feedback and scores from an online Quiz application.

[App Dev: Developing a Backend Service - Python](https://www.qwiklabs.com/focuses/1107?catalog_rank=%7B%22rank%22%3A10%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&parent=catalog&search_id=7467628)


### Cloud Data Fusion


#### Introduction 

Cloud Data Fusion is a fully managed, cloud-native, enterprise data integration service for quickly building and managing data pipelines. Cloud Data Fusion provides a graphical interface to increase time efficiency and reduce complexity. Now business users, developers, and data scientists can easily and reliably build scalable data integration solutions to cleanse, prepare, blend, transfer, and transform data— without having to wrestle with infrastructure.


#### CDAP

Cloud Data Fusion is powered by the open source project [CDAP](https://cdap.io/).

[https://cloud.google.com/data-fusion/docs](https://cloud.google.com/data-fusion/docs)


#### Qwiklab


##### Codeless Pipelines

This fundamental-level Quest offers hands-on practice with Cloud Data Fusion, a cloud-native, code-free, data integration platform. ETL Developers, Data Engineers and Analysts can greatly benefit from the pre-built transformations and connectors to build and deploy their pipelines without worrying about writing code. This Quest starts with a quickstart lab that familiarises learners with the Cloud Data Fusion UI. Learners then get to try running batch and realtime pipelines as well as using the built-in Wrangler plugin to perform some interesting transformations on data.

[Building Codeless Pipelines on Cloud Data Fusion](https://www.qwiklabs.com/quests/130?catalog_rank=%7B%22rank%22%3A4%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&search_id=7467888)


### Dataflow


#### Introduction

Dataflow is a managed service for executing a wide variety of data processing patterns. The documentation on this site shows you how to deploy your batch and streaming data processing pipelines using Dataflow, including directions for using service features.

[https://cloud.google.com/dataflow/docs](https://cloud.google.com/dataflow/docs)

Google Cloud Dataflow makes it easy to process and analyze real-time streaming data so that you can derive insights and react to new information in real-time. Learn how it is used in conjunction with other technologies, like PubSub, Kafka, BigQuery, Bigtable, or Datastore, to build end-to-end streaming architectures. Learn how these architectures enable diverse use cases such as real-time ingestion and ETL, real-time reporting & analytics, real-time alerting, or fraud detection.

[https://www.youtube.com/watch?v=7lJyq1hw_KI](https://www.youtube.com/watch?v=7lJyq1hw_KI)

Google Cloud customers are increasingly looking to leverage streaming data (customer interactions, sales transactions, machine logs) for building new innovative features, increasing sales, and protecting against risks. AI/ML (artificial intelligence/machine learning) technologies make it possible to amp up the detection of insights in large volumes of data: insights that otherwise would be impossible to gain with manual inspection. Learn how Dataflow together with TensorFlow Extended (TFX) and Cloud AI are enabling the extraction of label and classification information from video clips and natural text, predicting probabilities and detecting anomalies, fraud, and patterns in streams of business data.

[https://www.youtube.com/watch?v=cqDBnOaS6O4](https://www.youtube.com/watch?v=cqDBnOaS6O4)


#### Apache beam

The Apache Beam SDK is an open source programming model that enables you to develop both batch and streaming pipelines. You create your pipelines with an Apache Beam program and then run them on the Dataflow service. The [Apache Beam documentation](https://beam.apache.org/documentation/) provides in-depth conceptual information and reference material for the Apache Beam programming model, SDKs, and other runners.

[https://github.com/apache/beam](https://github.com/apache/beam)

[https://beam.apache.org/documentation/programming-guide/](https://beam.apache.org/documentation/programming-guide/)


#### Example Notebook

In this notebook, we set up your development environment and work through a simple example using the [DirectRunner](https://beam.apache.org/documentation/runners/direct/). You can explore other runners with the [Beam Capability Matrix](https://beam.apache.org/documentation/runners/capability-matrix/).

[https://colab.research.google.com/github/apache/beam/blob/master/examples/notebooks/get-started/try-apache-beam-py.ipynb](https://colab.research.google.com/github/apache/beam/blob/master/examples/notebooks/get-started/try-apache-beam-py.ipynb)


#### Word Count Example

[https://beam.apache.org/get-started/wordcount-example/](https://beam.apache.org/get-started/wordcount-example/)


#### Dataflow Templates 

These Dataflow templates are an effort to solve simple, but large, in-Cloud data tasks, including data import/export/backup/restore and bulk API operations, without a development environment. The technology under the hood which makes these operations possible is the [Google Cloud Dataflow](https://cloud.google.com/dataflow/) service combined with a set of [Apache Beam](https://beam.apache.org/) SDK templated pipelines.

[https://github.com/GoogleCloudPlatform/DataflowTemplates](https://github.com/GoogleCloudPlatform/DataflowTemplates)


#### Creating a pipeline

Using the Apache Beam interactive runner with JupyterLab notebooks lets you iteratively develop pipelines, inspect your pipeline graph, and parse individual PCollections in a read-eval-print-loop (REPL) workflow. These Apache Beam notebooks are made available through [AI Platform Notebooks](https://cloud.google.com/ai-platform/notebooks/docs), a managed service that hosts notebook virtual machines pre-installed with the latest data science and machine learning frameworks.

[https://cloud.google.com/dataflow/docs/guides/interactive-pipeline-development](https://cloud.google.com/dataflow/docs/guides/interactive-pipeline-development)


#### Using provided Dataflow templates

Google provides a set of [open-source](https://github.com/GoogleCloudPlatform/DataflowTemplates) Dataflow templates. 

[https://cloud.google.com/dataflow/docs/guides/templates/provided-templates](https://cloud.google.com/dataflow/docs/guides/templates/provided-templates)


#### Creating Dataflow templates

Dataflow [templates](https://cloud.google.com/dataflow/docs/templates/overview) use runtime parameters to accept values that are only available during pipeline execution. To customize the execution of a templated pipeline, you can pass these parameters to functions that run within the pipeline (such as a DoFn).

To create a template from your Apache Beam pipeline, you must modify your pipeline code to support runtime parameters.

[https://cloud.google.com/dataflow/docs/guides/templates/creating-templates](https://cloud.google.com/dataflow/docs/guides/templates/creating-templates)

[https://cloud.google.com/dataflow/docs/guides/templates/running-templates](https://cloud.google.com/dataflow/docs/guides/templates/running-templates)


#### Using Dataflow Flex templates

Dataflow Flex templates use docker containers.

[https://cloud.google.com/dataflow/docs/guides/templates/using-flex-templates#python](https://cloud.google.com/dataflow/docs/guides/templates/using-flex-templates#python)


#### Migrating from App  Engine Map/reduce to Dataflow

[https://cloud.google.com/dataflow/docs/guides/gae-mapreduce-migration](https://cloud.google.com/dataflow/docs/guides/gae-mapreduce-migration)


#### Dataflow Mobile Gaming Example

[https://beam.apache.org/get-started/mobile-gaming-example/](https://beam.apache.org/get-started/mobile-gaming-example/)


### Cloud Dataprep


#### Introduction

Cloud Dataprep by Trifacta is an intelligent data service for visually exploring, cleaning, and preparing structured and unstructured data for analysis, reporting, and machine learning. Because Cloud Dataprep is serverless and works at any scale, there is no infrastructure to deploy or manage. 

[https://cloud.google.com/dataprep](https://cloud.google.com/dataprep)

Use Cloud Dataprep to explore and transform raw data from disparate and/or large datasets into clean and structured data for further analysis and processing.

Access Cloud Dataprep at [https://clouddataprep.com](http://clouddataprep.com/)

Learn how to easily clean up your data without the hassle of writing complex ETL pipelines. 

[https://www.youtube.com/watch?v=DEh3pZIgJ9k](https://www.youtube.com/watch?v=DEh3pZIgJ9k)


#### Qwiklabs


##### Data Transformation Pipeline

The dataset you'll use is an [ecommerce dataset](https://www.en.advertisercommunity.com/t5/Articles/Introducing-the-Google-Analytics-Sample-Dataset-for-BigQuery/ba-p/1676331#) that has millions of Google Analytics session records for the [Google Merchandise Store](https://shop.googlemerchandisestore.com/) loaded into BigQuery. You have a copy of that dataset for this lab and will explore the available fields and rows for insights.

[Creating a Data Transformation Pipeline with Cloud Dataprep](https://www.qwiklabs.com/focuses/4415?parent=catalog)


### Cloud Composer


#### Introduction

Cloud Composer is a managed [Apache Airflow](https://airflow.apache.org/) service that helps you create, schedule, monitor and manage workflows. Cloud Composer automation helps you create Airflow environments quickly and use Airflow-native tools, such as the powerful Airflow web interface and command line tools, so you can focus on your workflows and not your infrastructure.

[https://cloud.google.com/composer/docs](https://cloud.google.com/composer/docs)

Cloud Composer is a managed workflow orchestration service built on Apache Airflow. 

[https://www.youtube.com/watch?v=bwZOAXnCMf8](https://www.youtube.com/watch?v=bwZOAXnCMf8)

Environments are a core concept in Cloud Composer. You can create one or more Cloud Composer environments inside of a project. Environments are self-contained Airflow deployments based on Google Kubernetes Engine. These environments work with Google Cloud services through connectors that are built into Airflow. You create Cloud Composer environments in [supported regions](https://cloud.google.com/about/locations), and the environments run within a Compute Engine zone. For simple use cases, you can create one environment in one region. For complex use cases, you can create multiple environments within a single region or across multiple regions. Airflow communicates with other Google Cloud products through the products' public APIs.


##### Data Pipelines with Cloud Composer

[https://www.youtube.com/watch?v=GeNFEtt-D4k](https://www.youtube.com/watch?v=GeNFEtt-D4k)


##### Cloud Composer best practices

[https://www.youtube.com/watch?v=RrKXZcKOz4A](https://www.youtube.com/watch?v=RrKXZcKOz4A)


#### Tutorials

[https://cloud.google.com/composer/docs/tutorials](https://cloud.google.com/composer/docs/tutorials)


##### Automating infrastructure using Airflow

Stop VM, take snapshots, start VMs, using python API and airflow.   Each step is put into an operator.  Collection of operators are put into a Plugin.  DAGs are composed of each step operator put into a pipeline. DAGs and Plugins are copied into Cloud Storage and run as Cloud Composer jobs.

[https://cloud.google.com/solutions/automating-infrastructure-using-cloud-composer](https://cloud.google.com/solutions/automating-infrastructure-using-cloud-composer)


#### Apache Airflow 

[Airflow](https://airflow.apache.org/) is a platform to programmatically author, schedule and monitor workflows.

Use Airflow to author workflows as Directed Acyclic Graphs (DAGs) of tasks. The Airflow scheduler executes your tasks on an array of workers while following the specified dependencies. Rich command line utilities make performing complex surgeries on DAGs a snap. The rich user interface makes it easy to visualize pipelines running in production, monitor progress, and troubleshoot issues when needed. Airflow is a micro-service architected framework. To deploy Airflow in a distributed setup, Cloud Composer provisions several Google Cloud components, which are collectively known as a Cloud Composer environment.


##### Concepts

[https://airflow.apache.org/docs/stable/concepts.html](https://airflow.apache.org/docs/stable/concepts.html)


##### Apache Airflow for Beginners.

[https://www.youtube.com/watch?v=YWtfU0MQZ_4](https://www.youtube.com/watch?v=YWtfU0MQZ_4)


##### Developing workflows with Apache Airflow

[http://michal.karzynski.pl/blog/2017/03/19/developing-workflows-with-apache-airflow/](http://michal.karzynski.pl/blog/2017/03/19/developing-workflows-with-apache-airflow/)


##### Operators

 An Operator is an atomic block of workflow logic, which performs a single action. Operators are written as Python classes (subclasses of BaseOperator), where the __init__ function can be used to configure settings for the task and a method named execute is called when the task instance is executed.

[https://github.com/apache/airflow/tree/master/airflow/operators](https://github.com/apache/airflow/tree/master/airflow/operators)


##### XCom

[https://airflow.apache.org/docs/stable/concepts.html#xcoms](https://airflow.apache.org/docs/stable/concepts.html#xcoms)


##### Task Orchestration tools: Comparison and Alternatives

A survey of pipeline & workflow tools.

[https://github.com/pditommaso/awesome-pipeline](https://github.com/pditommaso/awesome-pipeline)


##### Industrialization of a Machine Learning model using Apache Airflow and Apache BEAM.

[https://medium.com/swlh/industrialization-of-a-ml-model-using-airflow-and-apache-beam-5a5338f20184](https://medium.com/swlh/industrialization-of-a-ml-model-using-airflow-and-apache-beam-5a5338f20184)


##### Airflow vs. Luigi vs. Argo vs. MLFlow vs. KubeFlow

[https://www.datarevenue.com/en-blog/airflow-vs-luigi-vs-argo-vs-mlflow-vs-kubeflow](https://www.datarevenue.com/en-blog/airflow-vs-luigi-vs-argo-vs-mlflow-vs-kubeflow)


### Google Data Studio

Data Studio is a free tool that turns your data into informative, easy to read, easy to share, and fully customizable dashboards and reports. 

[https://support.google.com/datastudio#topic=6267740](https://support.google.com/datastudio#topic=6267740)

We all have a story to tell. Beyond the compelling words you share, you have insightful data you want your audience to interact with. But building custom interactive data visualizations, and publishing and maintaining them online can be challenging – and expensive. Join us to learn how Google Data Studio keeps you focused on what you do best – telling great data stories.

[https://www.youtube.com/watch?v=NhGLOVkyKjg](https://www.youtube.com/watch?v=NhGLOVkyKjg)


### Datalab 


#### Introduction

[https://www.youtube.com/watch?v=pdQHyTy3s7M](https://www.youtube.com/watch?v=pdQHyTy3s7M)

Cloud Datalab runs inside of a Google Compute Engine VM with an attached persistent disk that is used to store notebooks. Cloud Datalab VMs are connected to a special network in a project called datalab-network. The default configuration of this network limits incoming connections to SSH connections.

[https://cloud.google.com/datalab/docs/how-to/lifecycle](https://cloud.google.com/datalab/docs/how-to/lifecycle)


#### Datalab Quickstart

[https://cloud.google.com/datalab/docs/quickstart](https://cloud.google.com/datalab/docs/quickstart)


#### Working with Notebooks

Jupyter notebooks.

[https://www.youtube.com/watch?v=eEsfPL6SvJc](https://www.youtube.com/watch?v=eEsfPL6SvJc)

Working with Datalab notebooks.

[https://cloud.google.com/datalab/docs/how-to/working-with-notebooks](https://cloud.google.com/datalab/docs/how-to/working-with-notebooks)


### Looker 


#### Introduction

Looker gives you the tools to power a multitude of data experiences, from modern business intelligence and embedded analytics to workflow integrations and custom data apps. Regardless of where your data resides, Looker offers a unified surface to access the truest, most up-to-date version of your company’s data. And with data integrated into users’ daily workflows, organizations can extract value from their data at web scales.

[https://cloud.google.com/looker](https://cloud.google.com/looker)

Looker overview.

[https://www.youtube.com/watch?v=krXaBEi3f1s](https://www.youtube.com/watch?v=krXaBEi3f1s)

Database to Dashboard, technical demo.

[https://www.youtube.com/watch?v=HBgJWCBOOZg](https://www.youtube.com/watch?v=HBgJWCBOOZg)

The Data Modeling Layer.

[https://www.holistics.io/blog/the-data-modeling-layer/](https://www.holistics.io/blog/the-data-modeling-layer/)

How do you decide what to model in dbt vs LookML.

[https://blog.getdbt.com/-how-do-you-decide-what-to-model-in-dbt-vs-lookml--/](https://blog.getdbt.com/-how-do-you-decide-what-to-model-in-dbt-vs-lookml--/)

Dbt vs. Matillion vs. LookML.

[https://www.stephenlevin.co/data-modeling-layer-startup-analytics-dbt-vs-matillion-vs-lookml/](https://www.stephenlevin.co/data-modeling-layer-startup-analytics-dbt-vs-matillion-vs-lookml/)


#### Getting Started with Looker

Looker for data consumers.

[https://training.looker.com/looker-for-data-consumers](https://training.looker.com/looker-for-data-consumers)


#### Building Reports in Looker

Looker for data explorers.

[https://training.looker.com/looker-for-data-explorers](https://training.looker.com/looker-for-data-explorers)


#### LookML

Defining the language of your business with LookML.

[https://www.youtube.com/watch?v=XG4ytmgqSpU](https://www.youtube.com/watch?v=XG4ytmgqSpU)

Looker development foundations.

[https://training.looker.com/looker-development-foundations](https://training.looker.com/looker-development-foundations)

Introduction to LookML.

[https://docs.looker.com/data-modeling/learning-lookml/lookml-intro](https://docs.looker.com/data-modeling/learning-lookml/lookml-intro)

Training business users.

[https://training.looker.com/training-business-users](https://training.looker.com/training-business-users)


#### Looker vs Tableau

[https://looker.com/compare/looker-vs-tableau](https://looker.com/compare/looker-vs-tableau)


#### Looker, Building Explores:

[https://training.looker.com/building-explores-users-will-love](https://training.looker.com/building-explores-users-will-love)


#### Looker, Dashboards

[https://training.looker.com/designing-great-dashboards](https://training.looker.com/designing-great-dashboards)


#### Looker API Examples:

[https://training.looker.com/series/recorded-webinars/the-looker-api](https://training.looker.com/series/recorded-webinars/the-looker-api)


#### Recorded Training

[https://training.looker.com/series/recorded-webinars/custom-visualizations](https://training.looker.com/series/recorded-webinars/custom-visualizations)

[https://training.looker.com/series/recorded-webinars](https://training.looker.com/series/recorded-webinars)


### Data Catalog

Data Catalog is a fully managed and scalable metadata management service that empowers organizations to quickly discover, understand, and manage all of their data.

[https://cloud.google.com/data-catalog/docs](https://cloud.google.com/data-catalog/docs)

Data Catalog is a fully managed and scalable metadata management service that empowers organizations to quickly discover, understand, and manage all of their data.

[https://www.youtube.com/watch?v=eUKqXZDXj78](https://www.youtube.com/watch?v=eUKqXZDXj78)


### Cloud Life Sciences

Cloud Life Sciences is a suite of services and tools for managing, processing, and transforming life sciences data. It also enables advanced insights and operational workflows using highly scalable and compliant infrastructure. Cloud Life Sciences includes features such as the Cloud Life Sciences API and extract-transform-load (ETL) tools, and more.

[https://cloud.google.com/life-sciences/docs](https://cloud.google.com/life-sciences/docs)


### Firestore


#### Introduction

Firestore is a NoSQL document database built for automatic scaling, high performance, and ease of application development. While the Firestore interface has many of the same features as traditional databases, as a NoSQL database it differs from them in the way it describes relationships between data objects.

[https://cloud.google.com/firestore/docs](https://cloud.google.com/firestore/docs)

Cloud Firestore is a horizontally scaling document-model NoSQL database in the cloud.

[https://www.youtube.com/watch?v=v_hR4K4auoQ](https://www.youtube.com/watch?v=v_hR4K4auoQ)

Firestore can be used to build a serverless, scalable, mobile, syncing, analytical, IoT app. Firestore provides a powerful data back end for apps development from kilobyte to petabyte scale.

[https://www.youtube.com/watch?v=ah5tQ7yOh2s](https://www.youtube.com/watch?v=ah5tQ7yOh2s)

Cloud Firestore database service makes it easy for developers to scale new and existing applications, while adding real-time client data synchronization and offline mode capabilities.

[https://www.youtube.com/watch?v=9FRTk05PhRc](https://www.youtube.com/watch?v=9FRTk05PhRc)


#### Datastore

Firestore in Datastore mode is a NoSQL document database built for automatic scaling, high performance, and ease of application development.

Firestore is the newest version of Datastore and introduces [several improvements over Datastore](https://cloud.google.com/datastore/docs/firestore-or-datastore#in_native_mode). 

Existing Datastore users can access these improvements by creating a new Firestore in Datastore mode database instance. In the future, all existing Datastore databases will be [automatically upgraded to Firestore in Datastore mode](https://cloud.google.com/datastore/docs/upgrade-to-firestore).

While the Datastore mode interface has many of the same features as traditional databases, as a NoSQL database it differs from them in the way it describes relationships between data objects.

[https://cloud.google.com/datastore/docs](https://cloud.google.com/datastore/docs)

More explanations.

[https://www.youtube.com/watch?v=SYG-BgXoJFQ](https://www.youtube.com/watch?v=SYG-BgXoJFQ)


### Memorystore

Memorystore for Redis is a fully managed Redis service for the Google Cloud. Applications running on Google Cloud can achieve extreme performance by leveraging the highly scalable, available, secure Redis service without the burden of managing complex Redis deployments.

[https://cloud.google.com/memorystore/docs/redis](https://cloud.google.com/memorystore/docs/redis)

Cloud Memorystore for Redis provides a fully managed in-memory data store service built on scalable, more secure, and highly available infrastructure managed by Google.

[https://www.youtube.com/watch?v=sVpoAdbh2nU](https://www.youtube.com/watch?v=sVpoAdbh2nU)


### Firebase


#### Introduction

[Firebase](https://firebase.google.com/) is an app dev platform built on the [Google Cloud Platform](https://cloud.google.com/products) providing services and cross-platform SDKs. Firebase provides tools to develop high-quality apps, grow the  user base, and monetize the business while focusing on the users.

[https://firebase.google.com/docs/](https://firebase.google.com/docs/)

Youtube channel for firebase.

[https://www.youtube.com/playlist?list=PLOU2XLYxmsIJDw-9-88_LlOs0yR4b4Znv](https://www.youtube.com/playlist?list=PLOU2XLYxmsIJDw-9-88_LlOs0yR4b4Znv)

GCP & Firebase. Firebase projects are GCP Projects.

[https://www.youtube.com/watch?v=xbmYmgBEj4o](https://www.youtube.com/watch?v=xbmYmgBEj4o)

Cloud Functions, and Cloud Firestore. 

[https://www.youtube.com/watch?v=zR6CsTLTPsk](https://www.youtube.com/watch?v=zR6CsTLTPsk)

A list of URLs related to firebase.

[https://github.com/jthegedus/awesome-firebase](https://github.com/jthegedus/awesome-firebase)


#### Cloud Storage for Firebase

Developers use the Firebase SDKs for Cloud Storage to upload and download files directly from clients. If the network connection is poor, the client is able to retry the operation right where it left off, saving your users time and bandwidth.

[https://firebase.google.com/docs/storage/](https://firebase.google.com/docs/storage/)


#### Firebase Realtime Database

Store and sync data with our NoSQL cloud database. Data is synced across all clients in real time, and remains available when your app goes offline. The Firebase Realtime Database is a cloud-hosted database. Data is stored as JSON and synchronized in realtime to every connected client. When you build cross-platform apps with our iOS, Android, and JavaScript SDKs, all of your clients share one Realtime Database instance and automatically receive updates with the newest data.

[https://firebase.google.com/docs/database/](https://firebase.google.com/docs/database/)


#### Cloud Firestore or Realtime Database

Firebase offers two cloud-based, client-accessible database solutions that support real time data syncing:



*   Cloud Firestore is Firebase's newest database for mobile app development. It builds on the successes of the Realtime Database with a new, more intuitive data model. Cloud Firestore also features richer, faster queries and scales further than the Realtime Database.
*   Realtime Database is Firebase's original database. It's an efficient, low-latency solution for mobile apps that require synced states across clients in real time.

[https://firebase.google.com/docs/database/rtdb-vs-firestore](https://firebase.google.com/docs/database/rtdb-vs-firestore)


#### Firebase Authentication

Most apps need to know the identity of a user. Knowing a user's identity allows an app to securely save user data in the cloud and provide the same personalized experience across all of the user's devices. Firebase Authentication provides backend services, easy-to-use SDKs, and ready-made UI libraries to authenticate users to your app. It supports authentication using passwords, phone numbers, popular federated identity providers like Google, Facebook and Twitter, and more. Firebase Authentication integrates tightly with other Firebase services, and it leverages industry standards like OAuth 2.0 and OpenID Connect, so it can be easily integrated with your custom backend.

[https://firebase.google.com/docs/auth/](https://firebase.google.com/docs/auth/)


#### Cloud Functions for Firebase

Cloud Functions for Firebase is a serverless framework that lets you automatically run backend code in response to events triggered by Firebase features and HTTPS requests. Your JavaScript or TypeScript code is stored in Google's cloud and runs in a managed environment. There's no need to manage and scale your own servers.

[https://firebase.google.com/docs/functions/](https://firebase.google.com/docs/functions/)


#### Cloud Storage for Firebase

Cloud Storage for Firebase is a powerful, simple, and cost-effective object storage service built for Google scale. The Firebase SDKs for Cloud Storage add Google security to file uploads and downloads for your Firebase apps, regardless of network quality. You can use our SDKs to store images, audio, video, or other user-generated content. On the server, you can use [Google Cloud Storage](https://cloud.google.com/storage), to access the same files.

[https://firebase.google.com/docs/storage](https://firebase.google.com/docs/storage)


#### Firebase Test Lab

Firebase Test Lab is a cloud-based app-testing infrastructure. With one operation, you can test your Android or iOS app across a wide variety of devices and device configurations, and see the results—including logs, videos, and screenshots—in the Firebase console.

[https://firebase.google.com/docs/test-lab/](https://firebase.google.com/docs/test-lab/)


#### Qwiklabs


##### Build Apps

Firebase is a backend-as-service (Bass) platform for creating mobile and web applications. In this quest you will learn to build serverless web apps, import data into a serverless database, and build a Google Assistant application with Firebase and its Google Cloud integrations.

[Build Apps & Websites with Firebase](https://www.qwiklabs.com/quests/148?catalog_rank=%7B%22rank%22%3A6%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&search_id=7467888)


##### Hugo

In this lab you will create a pipeline for deploying websites based on Hugo, a static website builder. You will store the website content in Cloud Source Repositories and deploy the website with Firebase, then use Cloud Build to create a pipeline to automatically deploy new content that is committed to the repository.

[Deploy a Hugo Website with Cloud Build and Firebase Pipeline](https://www.qwiklabs.com/focuses/14353?catalog_rank=%7B%22rank%22%3A1%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&parent=catalog&search_id=7467907)


### Choosing Which Database to Use

Database choice and comparison charts and methods. \
[https://cloud.google.com/products/databases](https://cloud.google.com/products/databases)


## Data Science


### AI Building Blocks

AI Platform training with built-in algorithms.

[https://www.youtube.com/watch?v=IrPXm0DSCWI](https://www.youtube.com/watch?v=IrPXm0DSCWI)

What is Machine Learning?

[https://www.youtube.com/watch?v=HcqpanDadyQ&list=PLIivdWyY5sqJxnwJhe3etaK7utrBiPBQ2](https://www.youtube.com/watch?v=HcqpanDadyQ&list=PLIivdWyY5sqJxnwJhe3etaK7utrBiPBQ2)


#### AutoML

AutoML makes the power of machine learning available to you even if you have limited knowledge of machine learning. You can use AutoML to build on Google's machine learning capabilities to create your own custom machine learning models that are tailored to your business needs, and then integrate those models into your applications and web sites.

[https://cloud.google.com/automl/docs](https://cloud.google.com/automl/docs)


#### CloudML Engine

[https://www.youtube.com/watch?v=m0rqccviLNM](https://www.youtube.com/watch?v=m0rqccviLNM)


#### Cloud AutoML to custom model

[https://www.youtube.com/watch?v=OHIEZ-Scek8](https://www.youtube.com/watch?v=OHIEZ-Scek8)


#### AutoML NL for custom text classification

[https://www.youtube.com/watch?v=ieaqfU1BwJ8](https://www.youtube.com/watch?v=ieaqfU1BwJ8)


#### Vision AI

Cloud Vision includes several options that you can use to integrate machine learning vision models into your applications and web sites.

[https://cloud.google.com/vision/overview/docs](https://cloud.google.com/vision/overview/docs)

[https://www.youtube.com/watch?v=kgxfdTh9lz0](https://www.youtube.com/watch?v=kgxfdTh9lz0)

[https://www.youtube.com/watch?v=BN8aO0LULyw](https://www.youtube.com/watch?v=BN8aO0LULyw)

A favorite Qwiklab. Awwvision.

[https://www.qwiklabs.com/focuses/1241?parent=catalog](https://www.qwiklabs.com/focuses/1241?parent=catalog)


#### Video AI

Video Intelligence includes several options that you can use to integrate machine learning video intelligence models into your applications and web sites.

[https://cloud.google.com/video-intelligence/overview/docs](https://cloud.google.com/video-intelligence/overview/docs)

[https://www.youtube.com/watch?v=h1zU0Qor9J8](https://www.youtube.com/watch?v=h1zU0Qor9J8)


#### Cloud Natural Language API

The Cloud Natural Language API provides natural language understanding technologies to developers, including sentiment analysis, entity analysis, entity sentiment analysis, content classification, and syntax analysis. This API is part of the larger Cloud Machine Learning API family.

[https://cloud.google.com/natural-language/docs](https://cloud.google.com/natural-language/docs)

[https://www.youtube.com/watch?v=UFtXy0KRxVI](https://www.youtube.com/watch?v=UFtXy0KRxVI)

[https://www.youtube.com/watch?v=3iOtK0sRNMI](https://www.youtube.com/watch?v=3iOtK0sRNMI)

[https://www.youtube.com/watch?v=MNvT5JekDpg](https://www.youtube.com/watch?v=MNvT5JekDpg)


#### Cloud Translation

Cloud Translation can dynamically translate text between thousands of language pairs. Translation lets websites and programs programmatically integrate with the translation service.

[https://cloud.google.com/translate/docs](https://cloud.google.com/translate/docs)

[https://www.youtube.com/watch?v=YapTts_An9A](https://www.youtube.com/watch?v=YapTts_An9A)


#### Text-to-Speech

Text-to-Speech converts text or Speech Synthesis Markup Language (SSML) input into audio data of natural human speech.

[https://cloud.google.com/text-to-speech/docs](https://cloud.google.com/text-to-speech/docs)

[https://www.youtube.com/watch?v=OK1ZmlaFIV8](https://www.youtube.com/watch?v=OK1ZmlaFIV8)


#### Speech-to-Text

Text-to-Speech converts text or Speech Synthesis Markup Language (SSML) input into audio data of natural human speech.

[https://cloud.google.com/speech-to-text/docs](https://cloud.google.com/speech-to-text/docs)

[https://www.youtube.com/watch?v=naZ8oEKuR44](https://www.youtube.com/watch?v=naZ8oEKuR44)


### Dialogflow

Dialogflow is a natural language understanding platform that makes it easy to design and integrate a conversational user interface into your mobile app, web application, device, bot, interactive voice response system, and so on. Using Dialogflow, you can provide new and engaging ways for users to interact with your product.

[https://cloud.google.com/dialogflow/docs](https://cloud.google.com/dialogflow/docs)

[https://www.youtube.com/watch?v=YoytR7kzorg](https://www.youtube.com/watch?v=YoytR7kzorg)


### AutoML Tables

AutoML Tables enables your entire team to automatically build and deploy state-of-the-art machine learning models on structured data at massively increased speed and scale.

[https://cloud.google.com/automl-tables/docs](https://cloud.google.com/automl-tables/docs)

[https://www.youtube.com/watch?v=tWbiOuHae0c](https://www.youtube.com/watch?v=tWbiOuHae0c)


### Cloud Interference API

Time-series analysis is essential for day-to-day operation of many companies. Most popular use cases include analyzing foot traffic and conversion for retailers, detecting data anomalies, identifying correlations in real time over sensor data, or generating high-quality recommendations. With Cloud Inference API Alpha, you can gather insights in real time from your typed time-series datasets.

[https://cloud.google.com/inference/docs](https://cloud.google.com/inference/docs)


### Basic Bayes Theorem

Bayes' theorem, named after 18th-century British mathematician Thomas Bayes, is a mathematical formula for determining conditional probability. Conditional probability is the likelihood of an outcome occurring, based on a previous outcome occurring.

[https://www.youtube.com/watch?v=HZGCoVF3YvM](https://www.youtube.com/watch?v=HZGCoVF3YvM)

We can use probability to make predictions in machine learning. Perhaps the most widely used example is called the Naive Bayes algorithm. Not only is it straightforward to understand, but it also achieves surprisingly good results on a wide range of problems.

[https://machinelearningmastery.com/naive-bayes-classifier-scratch-python/](https://machinelearningmastery.com/naive-bayes-classifier-scratch-python/)


### Classification


#### Regression & Classification

[https://www.youtube.com/watch?v=TJveOYsK6MY](https://www.youtube.com/watch?v=TJveOYsK6MY)


#### Content Classification

Content Classification analyzes a document and returns a list of content categories that apply to the text found in the document. 

[https://cloud.google.com/natural-language/docs/classifying-text](https://cloud.google.com/natural-language/docs/classifying-text)

Using AutoML to classify text.

[https://www.youtube.com/watch?v=ieaqfU1BwJ8](https://www.youtube.com/watch?v=ieaqfU1BwJ8)


#### Classification, redaction, and de-identification

The Cloud Data Loss Prevention (DLP) helps you understand, manage, and protect sensitive data. With the Cloud DLP, you can easily classify and redact sensitive data contained in text-based content and images, including content stored in Google Cloud storage repositories.

[https://cloud.google.com/dlp/docs/classification-redaction](https://cloud.google.com/dlp/docs/classification-redaction)


### Scikit Learn

Whenever you perform classification, the first step is to understand the problem and identify potential features and labels. Features are those characteristics or attributes which affect the results of the label. For example, in the case of a loan distribution, bank manager's identify the customer's occupation, income, age, location, previous loan history, transaction history, and credit score. These characteristics are known as features which help the model classify customers.

[https://www.youtube.com/watch?v=rvVkVsG49uU](https://www.youtube.com/watch?v=rvVkVsG49uU)

[https://www.youtube.com/watch?v=MaKLWy5zXe8](https://www.youtube.com/watch?v=MaKLWy5zXe8)

The classification has two phases, a learning phase, and the evaluation phase. In the learning phase, the classifier trains its model on a given dataset and in the evaluation phase, it tests the classifier performance. Performance is evaluated on the basis of various parameters such as accuracy, error, precision, and recall.

[https://www.datacamp.com/community/tutorials/naive-bayes-scikit-learn](https://www.datacamp.com/community/tutorials/naive-bayes-scikit-learn)


### ML


#### Introduction

Machine learning is an application of artificial intelligence (AI) that provides systems the ability to automatically learn and improve from experience without being explicitly programmed. Machine learning focuses on the development of computer programs that can access data and use it to learn for themselves.

[https://www.youtube.com/watch?v=QR_LQQ-vvko](https://www.youtube.com/watch?v=QR_LQQ-vvko)

[https://www.youtube.com/watch?v=HcqpanDadyQ](https://www.youtube.com/watch?v=HcqpanDadyQ)


#### ML Solutions 101

AI Platform enables many parts of the machine learning (ML) workflow. This document provides an introductory description of the overall ML process and explains where each AI Platform service fits into the process.

[https://cloud.google.com/ai-platform/docs/ml-solutions-overview](https://cloud.google.com/ai-platform/docs/ml-solutions-overview)

7 steps of Machine learning.

[https://www.youtube.com/watch?v=nKW8Ndu7Mjw](https://www.youtube.com/watch?v=nKW8Ndu7Mjw)

Plain and Simple estimators.

[https://www.youtube.com/watch?v=G7oolm0jU8I](https://www.youtube.com/watch?v=G7oolm0jU8I)


#### ML Options

Decision pyramid to choose the right ML option.

[https://www.youtube.com/watch?v=pm_-pVPvZ-4](https://www.youtube.com/watch?v=pm_-pVPvZ-4)


#### TensorFlow

TensorFlow is an open source, powerful, portable machine learning library developed by Google that can work with very large datasets.

[https://www.tensorflow.org/learn](https://www.tensorflow.org/learn)


##### TensorFlow.js

Getting started with TensorFlow.js.

[https://www.youtube.com/watch?v=WYvgP9LfvTg](https://www.youtube.com/watch?v=WYvgP9LfvTg)


##### TensorFlow Hub

The TensorFlow Hub lets you search and discover hundreds of trained, ready-to-deploy machine learning models in one place.

[https://tfhub.dev/](https://tfhub.dev/)

[https://www.youtube.com/watch?v=SJ1LGUyw-Xg](https://www.youtube.com/watch?v=SJ1LGUyw-Xg)


##### TensorBoard

Visualizing your model with tensorboard.

[https://www.youtube.com/watch?v=qEQ-_EId-D0](https://www.youtube.com/watch?v=qEQ-_EId-D0)


##### TensorFlow Graph

Graphs are data structures that contain a set of [tf.Operation](https://www.tensorflow.org/api_docs/python/tf/Operation) objects, which represent units of computation; and [tf.Tensor](https://www.tensorflow.org/api_docs/python/tf/Tensor) objects, which represent the units of data that flow between operations. They are defined in a [tf.Graph](https://www.tensorflow.org/api_docs/python/tf/Graph) context. Since these graphs are data structures, they can be saved, run, and restored all without the original Python code.

[https://www.youtube.com/watch?v=qTYQEXsBb_E](https://www.youtube.com/watch?v=qTYQEXsBb_E)


##### TensorFlow Enterprise

TensorFlow Enterprise makes it easier to develop and deploy TensorFlow models on Google Cloud, by providing users with a set of products and services, which provide enterprise-grade support and cloud scale performance. Users can get the benefits of TensorFlow Enterprise by using the TensorFlow Enterprise Distribution on AI Platform Notebooks, AI Platform Deep Learning Containers and AI Platform Deep Learning VM Image.

[https://cloud.google.com/TensorFlow-enterprise/docs](https://cloud.google.com/tensorflow-enterprise/docs)


##### TensorFlow Resources

A list of URLs related to TensorFlow.

[https://github.com/jtoy/awesome-TensorFlow](https://github.com/jtoy/awesome-tensorflow)


##### Kubeflow

The Kubeflow project is dedicated to making deployments of machine learning (ML) workflows on Kubernetes simple, portable and scalable. Our goal is not to recreate other services, but to provide a straightforward way to deploy best-of-breed open-source systems for ML to diverse infrastructures. Anywhere you are running Kubernetes, you should be able to run Kubeflow.

[https://www.kubeflow.org/docs/about/kubeflow/](https://www.kubeflow.org/docs/about/kubeflow/)

[https://www.youtube.com/watch?v=cTZArDgbIWw&list=PLIivdWyY5sqLS4lN75RPDEyBgTro_YX7x](https://www.youtube.com/watch?v=cTZArDgbIWw&list=PLIivdWyY5sqLS4lN75RPDEyBgTro_YX7x)


### AI Platform and Accelerators


#### AI Platform

AI Platform makes it easy for machine learning developers, data scientists, and data engineers to take their ML projects from ideation to production and deployment, quickly and cost-effectively. From data engineering to "no lock- in" flexibility, AI Platform's integrated tool chain helps you build and run your own machine learning applications.

[https://cloud.google.com/ai-platform/docs](https://cloud.google.com/ai-platform/docs)


#### AI Platform Deep Learning VM Images

Deep Learning VM images are Debian 9- and Debian 10-based Compute Engine virtual machine images optimized for data science and machine learning tasks. All images come with key ML frameworks and tools pre-installed, and can be used out of the box on instances with GPUs to accelerate your data processing tasks.

[https://cloud.google.com/ai-platform/deep-learning-vm/docs](https://cloud.google.com/ai-platform/deep-learning-vm/docs)

[https://www.youtube.com/watch?v=kyNbYCHFCSw](https://www.youtube.com/watch?v=kyNbYCHFCSw)


#### AI Platform Notebooks

AI Platform Notebooks makes it easy to manage JupyterLab instances through a protected, publicly available notebook instance URL. A JupyterLab instance is a [Deep Learning virtual machine](https://cloud.google.com/ai-platform/deep-learning-vm/docs) instance with the latest machine learning and data science libraries pre-installed.

[https://cloud.google.com/ai-platform/notebooks/docs](https://cloud.google.com/ai-platform/notebooks/docs)

[https://www.youtube.com/watch?v=Eu57QKNHaiY](https://www.youtube.com/watch?v=Eu57QKNHaiY)


#### AI Platform Deep Learning Containers

[https://cloud.google.com/ai-platform/deep-learning-containers/docs](https://cloud.google.com/ai-platform/deep-learning-containers/docs)

[https://www.youtube.com/watch?v=h_BpDOdTX7Y](https://www.youtube.com/watch?v=h_BpDOdTX7Y)


#### AI Platform Pipelines

[https://cloud.google.com/ai-platform/pipelines/docs](https://cloud.google.com/ai-platform/pipelines/docs)

[https://www.youtube.com/watch?v=MUtsIaQuiRw](https://www.youtube.com/watch?v=MUtsIaQuiRw)


#### AI Hub

AI Hub offers a collection of assets for developers and data scientists building artificial intelligence (AI) systems. Train your machine learning (ML) model in a notebook or deploy it to a managed service. Find and deploy ML pipelines. Explore and reuse TensorFlow modules. Discover the best solution for serving and managing your trained model. Learn from in depth tutorials and examples.

[https://cloud.google.com/ai-hub/docs](https://cloud.google.com/ai-hub/docs)


#### AI Explanations

Intro to Explanations for AI Platform.

[https://www.youtube.com/watch?v=XXvFHqLv9p8](https://www.youtube.com/watch?v=XXvFHqLv9p8)


#### Document AI

Unlock insights from documents with machine learning. Tap into the opportunity offered by your unstructured data to increase operational efficiency, improve customer experience, and inform decision-making. Google Cloud’s Vision OCR (optical character recognition) and form parser technology uses [industry-leading](https://cloud.google.com/forrester-computer-vision) deep-learning neural network algorithms to perform text, character, and image recognition in over 200 languages with exceptional accuracy.

Using the same deep machine learning technology that powers Google Search and Assistant, Google Cloud’s natural language products enable you to derive valuable insights from your unstructured documents.

[https://cloud.google.com/solutions/document-ai](https://cloud.google.com/solutions/document-ai)

[https://www.youtube.com/watch?v=akp0zeI6_6c](https://www.youtube.com/watch?v=akp0zeI6_6c)


### Cloud GPUs

Compute Engine provides graphics processing units (GPUs) that you can add to your virtual machine instances. You can use these GPUs to accelerate specific workloads on your instances such as machine learning and data processing.

[https://cloud.google.com/compute/docs/gpus](https://cloud.google.com/compute/docs/gpus)

[https://www.youtube.com/watch?v=jUZhe1aTnFk](https://www.youtube.com/watch?v=jUZhe1aTnFk)


### Cloud TPU

Tensor Processing Units (TPUs) are Google’s custom-developed application-specific integrated circuits (ASICs) used to accelerate machine learning workloads. TPUs are designed from the ground up with the benefit of Google’s deep experience and leadership in machine learning.

[https://cloud.google.com/tpu/docs](https://cloud.google.com/tpu/docs)

[https://www.youtube.com/watch?v=2kSo7Az4ZOs](https://www.youtube.com/watch?v=2kSo7Az4ZOs)


### Keras


#### Introduction

Keras is an API designed for human beings, not machines. [Keras follows best practices for reducing cognitive load](https://blog.keras.io/user-experience-design-for-apis.html): it offers consistent & simple APIs, it minimizes the number of user actions required for common use cases, and it provides clear and actionable feedback upon user error. This makes Keras easy to learn and easy to use. As a Keras user, you are more productive, allowing you to try more ideas than your competition, faster -- which in turn [helps you win machine learning competitions](https://www.quora.com/Why-has-Keras-been-so-successful-lately-at-Kaggle-competitions). This ease of use does not come at the cost of reduced flexibility: because Keras integrates deeply with low-level TensorFlow functionality, it enables you to develop highly hackable workflows where any piece of functionality can be customized.

[https://keras.io/](https://keras.io/)


#### Getting started

[https://www.youtube.com/watch?v=J6Ok8p463C4](https://www.youtube.com/watch?v=J6Ok8p463C4)


#### TensorFlow Estimator

[https://www.youtube.com/watch?v=YCXFceVKHTk](https://www.youtube.com/watch?v=YCXFceVKHTk)


#### Notebook

[https://github.com/GoogleCloudPlatform/cloudml-samples/blob/master/notebooks/TensorFlow/getting-started-keras.ipynb](https://github.com/GoogleCloudPlatform/cloudml-samples/blob/master/notebooks/tensorflow/getting-started-keras.ipynb)


### Datalab


#### Introduction

 Cloud Datalab can be used to easily explore, visualize, analyze, and transform data using familiar languages, such as Python and SQL, interactively. Datalab comes with pre-installed Jupyter samples and tutorial notebooks.  Datalab can be used to  show you how to access, analyze, monitor and visualize data.  You can use notebooks with Python, TensorFlow ML, Google Analytics, BigQuery and Google Charts APIs.


##### Visualization of large datasets

[https://www.youtube.com/watch?v=pdQHyTy3s7M](https://www.youtube.com/watch?v=pdQHyTy3s7M)


##### Notebook in the cloud.

[https://www.youtube.com/watch?v=Eu57QKNHaiY](https://www.youtube.com/watch?v=Eu57QKNHaiY)


##### Jupyter

[https://www.youtube.com/watch?v=2eCHD6f_phE](https://www.youtube.com/watch?v=2eCHD6f_phE)


##### Datalab github open source

[https://github.com/googledatalab/datalab](https://github.com/googledatalab/datalab)


#### Quickstart

[https://cloud.google.com/datalab/docs/quickstart](https://cloud.google.com/datalab/docs/quickstart)


#### Videos

[https://cloud.google.com/datalab/docs#videos](https://cloud.google.com/datalab/docs#videos)


### Colab

A live Colab jupyter lab notebook can be run at:

[Getting started: Training and prediction with Keras in AI Platform](https://colab.research.google.com/github/GoogleCloudPlatform/cloudml-samples/blob/master/notebooks/tensorflow/getting-started-keras.ipynb)

_Please note that any ipynb file hosted on github can be pointed to_

https://colab.research.google.com/github/...path...to..the..file.ipynb and rendered live for interactive use and edits.


#### Neural Networks in Colab

[https://www.youtube.com/watch?v=_VTtrSDHPwU](https://www.youtube.com/watch?v=_VTtrSDHPwU)


### Qwiklabs


#### Data Science 101

In this first Quest, you are given the opportunity to practice all aspects of ingestion, preparation, processing, querying, exploring and visualizing data sets using Google Cloud tools and services.

[Data Science on Google Cloud](https://www.qwiklabs.com/quests/43?catalog_rank=%7B%22rank%22%3A1%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&search_id=7467654)


#### AI Platform

This lab will give you hands-on practice with [TensorFlow 2.x](http://tensorflow.org/) model training, both locally and on [AI Platform](https://cloud.google.com/ai-platform/docs/). After training, you will learn how to deploy your model to AI Platform for serving (prediction). You'll train your model to predict the income category of a person using the [United States Census Income Dataset](https://archive.ics.uci.edu/ml/datasets/Census+Income).

[AI Platform: Qwik Start](https://www.qwiklabs.com/focuses/581?catalog_rank=%7B%22rank%22%3A16%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&parent=catalog&search_id=7468017)


#### Machine learning

 In this second Quest, you run full-fledged machine learning jobs with state-of-the-art tools and real-world data sets, all using Google Cloud tools and services.

[Data Science on Google Cloud: Machine Learning](https://www.qwiklabs.com/quests/50?catalog_rank=%7B%22rank%22%3A2%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&search_id=7467654)


#### Business Transformation

What are cloud technology and data science, and what can they do for you and your business? In this course, you'll learn about core Google Cloud business drivers, how to determine whether business transformation is right for your team, and how to build short- and long-term projects with the power of the cloud. You'll also receive a supplementary student workbook that contains templates, guides, and resource links to help you create a custom briefing document to share with your leadership, technical teams, or partners.

[Business Transformation with Google Cloud](https://www.qwiklabs.com/courses/888?catalog_rank=%7B%22rank%22%3A3%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&search_id=7467654)


#### TensorFlow Hello World

In this lab you learn the basic ‘Hello World' of machine learning where, instead of programming explicit rules in a language such as Java or C++, you build a system that is trained on data to infer the rules that determine a relationship between numbers.

[Learning TensorFlow: the Hello World of Machine Learning](https://www.qwiklabs.com/focuses/7639?catalog_rank=%7B%22rank%22%3A14%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&parent=catalog&search_id=7468017)


#### ML with TensorFlow

In this lab, you learn how to use Google Cloud Machine Learning and TensorFlow 1.x to develop and evaluate prediction models using machine learning. 

[Machine Learning with TensorFlow](https://www.qwiklabs.com/focuses/3391?catalog_rank=%7B%22rank%22%3A8%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&parent=catalog&search_id=7468000)


#### Predict Housing Prices

In this lab, you will build an end to end machine learning solution using TensorFlow 1.x and AI Platform and leverage the cloud for distributed training and online prediction.

[Predict Housing Prices with TensorFlow and AI Platform](https://www.qwiklabs.com/focuses/3644?catalog_rank=%7B%22rank%22%3A9%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&parent=catalog&search_id=7468000)


#### TensorFlow on GCP

This quest takes you beyond the basics of using predefined models and teaches you how to build, train and deploy your own on GCP.

[Intermediate ML: TensorFlow on GCP](https://www.qwiklabs.com/quests/83?catalog_rank=%7B%22rank%22%3A1%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&search_id=7468000)


#### Data and Machine Learning

In this advanced-level quest, you will learn how to harness serious GCP computing power to run big data and machine learning jobs. The hands-on labs will give you use cases, and you will be tasked with implementing big data and machine learning practices utilized by Google’s very own Solutions Architecture team.

[Google Cloud Solutions II: Data and Machine Learning](https://www.qwiklabs.com/quests/38?catalog_rank=%7B%22rank%22%3A3%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&search_id=7468000)


#### TensorFlow for Poets

In this lab, you will learn how to install and run TensorFlow 1.x on a single machine, then train a simple classifier to classify images of flowers.

[TensorFlow for Poets](https://www.qwiklabs.com/focuses/1095?catalog_rank=%7B%22rank%22%3A10%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&parent=catalog&search_id=7468000)


#### Object Detection

A favorite lab.

This is a basic lab designed to familiarize you with TensorFlow applications. When you are finished, you should be able to:



*   Create a virtual machine (VM) using [Compute Engine](https://cloud.google.com/compute/).
*   Install the [Object Detection API](https://github.com/tensorflow/models/tree/master/research/object_detection) library.
*   Install and launch an object detection web application.
*   Test the web application with uploaded images.

[Creating an Object Detection Application Using TensorFlow](https://www.qwiklabs.com/focuses/1823?catalog_rank=%7B%22rank%22%3A11%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&parent=catalog&search_id=7468017)


#### Distributed TensorFlow

This lab shows you how to use a distributed configuration of [TensorFlow 1.x](https://www.tensorflow.org/) on multiple Compute Engine instances to train a [convolutional neural network](https://wikipedia.org/wiki/Convolutional_neural_network) model using the [MNIST dataset](http://yann.lecun.com/exdb/mnist/). The MNIST dataset enables handwritten digit recognition, and is widely used in machine learning as a training set for image recognition.

[Running Distributed TensorFlow on Compute Engine](https://www.qwiklabs.com/focuses/1826?catalog_rank=%7B%22rank%22%3A12%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&parent=catalog&search_id=7468017)


#### Baby Weight

In this lab you train, evaluate, and deploy a machine learning model to predict a baby's weight. You then send requests to the model to make online predictions.

[Predict Baby Weight with TensorFlow on AI Platform](https://www.qwiklabs.com/focuses/607?catalog_rank=%7B%22rank%22%3A13%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&parent=catalog&search_id=7468017)


#### BigQuery

Want to learn and practice machine learning and build models in minutes instead of hours using just SQL? BigQuery Machine Learning is a new feature in BigQuery where data analysts can create, train, evaluate, and predict machine learning models with minimal coding. In this series of labs you will experiment with different model types and learn what makes a good model.

[BigQuery for Machine Learning](https://www.qwiklabs.com/quests/71?catalog_rank=%7B%22rank%22%3A1%2C%22num_filters%22%3A1%2C%22has_search%22%3Atrue%7D&search_id=7467680)


#### ML API

It's no secret that machine learning is one of the fastest growing fields in tech, and Google Cloud has been instrumental in furthering its development. With a host of APIs, Google Cloud has a tool for just about any machine learning job. In this advanced-level quest, you will get hands-on practice with machine learning APIs by taking labs like Detect Labels, Faces, and Landmarks in Images with the Cloud Vision API. 

[Integrate with Machine Learning APIs](https://www.qwiklabs.com/quests/136?catalog_rank=%7B%22rank%22%3A2%2C%22num_filters%22%3A1%2C%22has_search%22%3Atrue%7D&search_id=7467680)


#### BigQuery ML

Want to build ML models in minutes instead of hours using just SQL? BigQuery ML democratizes machine learning by letting data analysts create, train, evaluate, and predict with machine learning models using existing SQL tools and skills. In this series of labs, you will experiment with different model types and learn what makes a good model.

[Create ML Models with BigQuery ML](https://www.qwiklabs.com/quests/146?catalog_rank=%7B%22rank%22%3A4%2C%22num_filters%22%3A1%2C%22has_search%22%3Atrue%7D&search_id=7467680)


#### Explainable AI

In this fundamental-level Quest, you will get hands-on practice with Explainable AI - a set of tools and frameworks to help you develop interpretable and inclusive machine learning models and deploy them with confidence. 

[Explore Machine Learning Models with Explainable AI](https://www.qwiklabs.com/quests/126?catalog_rank=%7B%22rank%22%3A6%2C%22num_filters%22%3A1%2C%22has_search%22%3Atrue%7D&search_id=7467680)


#### Genomics

Google Genomics helps the life science community organize the world’s genomic information and make it accessible and useful. Big genomic data is here today, with petabytes rapidly growing toward exabytes. [Google Genomics](https://cloud.google.com/genomics/) is an API that is part of Google Cloud Platform. Through this and other add-ons, you can apply the same technologies that power Google Search and Maps to securely store, process, explore, and share large, complex datasets.

In this lab you’ll learn how to run a pipeline that uses the Cloud Genomics Pipelines API to create an index file (BAI file) from a large binary file containing DNA sequences (BAM file).

[Google Genomics: Qwik Start](https://www.qwiklabs.com/focuses/589?catalog_rank=%7B%22rank%22%3A4%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&parent=catalog&search_id=7467654)


#### Geospatial

This lab demonstrates how to use Google Dataflow to process real-time streaming data from a real-time real world historical data set, storing the results in BigQuery and then using Google Data Studio to visualize real-time geospatial data. Cloud Dataflow is a fully-managed service for transforming and enriching data in stream (real time) and batch (historical) modes via Java and Python APIs with the Apache Beam SDK. Cloud Dataflow provides a serverless architecture that can be used to shard and process very large batch data sets, or high volume live streams of data, in parallel. BigQuery is a RESTful web service that enables interactive analysis of massively large datasets working in conjunction with Google Storage. The data set that is used provides historic information about internal flights in the United States retrieved from the US Bureau of Transport Statistics website. This data set can be used to demonstrate a wide range of data science concepts and techniques and will be used in all of the other labs in the [Data Science on Google Cloud](https://google.qwiklabs.com/quests/43) Quest.

[Visualize Real Time Geospatial Data with Google Data Studio](https://www.qwiklabs.com/focuses/1160?catalog_rank=%7B%22rank%22%3A5%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&parent=catalog&search_id=7467654)


#### Distributed Cloud ML

In this lab you will create and configure deep neural network models with Google Cloud ML, then use the Google Cloud ML Engine to make predictions using your trained models.

You will extend the basic Google Cloud ML machine learning framework developed in the previous lab in this quest, Machine Learning with TensorFlow, to explore a number of approaches to optimizing machine learning models. The base data set that is used for these labs provides historic information about internal flights in the United States and has been retrieved from the US Bureau of Transport Statistics website. This data set can be used to demonstrate a wide range of data science concepts and techniques and is used in all of the other labs in the Data Science on the Google Cloud and Data Science on Google Cloud: Machine Learning quests. The specific data files used in this lab provide separate training and evaluation data sets. The details about how these files can be produced is covered in a previous lab in this quest, Processing Time Windowed Data with Apache Beam and Cloud Dataflow (Java). Cloud Datalab is a powerful interactive tool created to explore, analyze, transform, and visualize data and build machine learning models on Google Cloud. It runs on Compute Engine and connects to multiple cloud services such as BigQuery, Cloud SQL, or simple text data stored on Cloud Storage,so you can focus on your data science tasks.

[Distributed Machine Learning with Google Cloud ML](https://www.qwiklabs.com/focuses/3389?catalog_rank=%7B%22rank%22%3A6%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&parent=catalog&search_id=7467654)


#### Ingesting Data 

In this lab you'll learn how to use a bash script to download selected data, which provides historical information about internal flights in the United States, from a large public data set available on the internet. The techniques used to ingest this data from the US Bureau of Transport Statistics website into the cloud can be applied generally to other data sets that provide comprehensive real world data that needs to be parsed and cleaned up before it can be used.

[Ingesting Data Into The Cloud](https://www.qwiklabs.com/focuses/1155?catalog_rank=%7B%22rank%22%3A7%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&parent=catalog&search_id=7467654)


#### Spark ML on Dataproc

In this lab you will learn how to implement logistic regression using a machine learning library for Apache Spark running on a Google Cloud Dataproc cluster to develop a model for data from a multivariable dataset. Google Cloud Dataproc is a fast, easy-to-use, fully-managed cloud service for running Apache Spark and Apache Hadoop clusters in a simple, cost-efficient way. Cloud Dataproc easily integrates with other Google Cloud services, giving you a powerful and complete platform for data processing, analytics and machine learning. Apache Spark is an analytics engine for large scale data processing. Logistic regression is available as a module in Apache Spark's machine learning library, MLlib. Spark MLlib, also called Spark ML, includes implementations for most standard machine learning algorithms such as k-means clustering, random forests, alternating least squares, k-means clustering, decision trees, support vector machines, etc. Spark can run on a Hadoop cluster, like Google Cloud Dataproc, in order to process very large datasets in parallel. The base data set that is used provides historical information about internal flights in the United States retrieved from the US Bureau of Transport Statistics website. This data set can be used to demonstrate a wide range of data science concepts and techniques and is used in all of the other labs in the Data Science on the Google Cloud and Data Science on Google Cloud: Machine Learning quests. In this lab the data is provided for you as a set of CSV formatted text files.

[Machine Learning with Spark on Google Cloud Dataproc](https://www.qwiklabs.com/focuses/3390?catalog_rank=%7B%22rank%22%3A8%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&parent=catalog&search_id=7467654)


#### Data Studio

This lab demonstrates how to use Google Data Studio to visualize data stored in Google Cloud SQL for MySQL.

[Visualizing Data with Google Data Studio](https://www.qwiklabs.com/focuses/1158?catalog_rank=%7B%22rank%22%3A9%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&parent=catalog&search_id=7467654)


#### Dataflow

In this lab you will learn how to deploy a Java application using Maven to process data with Cloud Dataflow. This lab uses a Java application that implements time-windowed aggregation to augment the raw data in order to produce a consistent training and test datasets that can be used to refine your machine learning models in later labs.

[Processing Time Windowed Data with Apache Beam and Cloud Dataflow (Java)](https://www.qwiklabs.com/focuses/3392?catalog_rank=%7B%22rank%22%3A10%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&parent=catalog&search_id=7467654)


#### Google Cloud ML

In this lab you will combine a number of the components developed in earlier labs in the Data Science on Google Cloud and Data Science on Google Cloud: Machine Learning quests to create a real-time flight delay prediction service using Google Cloud services.

[ML with Google Cloud ML](https://www.qwiklabs.com/focuses/3393?catalog_rank=%7B%22rank%22%3A8%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&parent=catalog&search_id=5293890).


#### Datalab

With Cloud Datalab you'll be able to analyze your data on BigQuery, Cloud Machine Learning Engine, Compute Engine, and Cloud Storage using Python, SQL, and JavaScript (for BigQuery user-defined functions).

[Google Cloud Datalab quick start](https://www.qwiklabs.com/focuses/999?catalog_rank=%7B%22rank%22%3A1%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&parent=catalog&search_id=5317075) 


#### Reinforcement Learning

Like many other areas of machine learning research, [reinforcement learning (RL)](https://en.wikipedia.org/wiki/Reinforcement_learning) is evolving at breakneck speed. Just as they have done in other research areas, researchers are leveraging deep learning to achieve state-of-the-art results.

[Reinforcement Learning](https://www.qwiklabs.com/focuses/10285?parent=catalog)


#### TensorFlow

TensorFlow is an open source software library for high performance numerical computation that's great for writing models that can train and run on platforms ranging from your laptop to a fleet of servers in the Cloud to an edge device. This quest takes you beyond the basics of using predefined models and teaches you how to build, train and deploy your own on GCP.

[Additional TensorFlow Quests](https://www.qwiklabs.com/quests/83)


#### Predict Visitor Purchases

[Predict Visitor Purchases with a Classification Model in BQML](https://www.qwiklabs.com/focuses/1794?catalog_rank=%7B%22rank%22%3A1%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&parent=catalog&search_id=7510934)


#### Kubeflow AI Platform Pipelines 

In this lab learn how to install and use Kubeflow Pipelines to orchestrate various Google Cloud Services in an end-to-end ML pipeline. Once Kubeflow Pipelines are installed you create an AI Platform Notebook and complete 2 example notebooks to demonstrate the services used and how to author a pipeline.

[Kubeflow Pipelines with AI Platform](https://www.qwiklabs.com/focuses/10948?catalog_rank=%7B%22rank%22%3A2%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&parent=catalog&search_id=7467701)


## Database Related topics


### SQL, NoSQL, NewSQL

[https://www.youtube.com/watch?v=ZS_kXvOeQ5Y](https://www.youtube.com/watch?v=ZS_kXvOeQ5Y)

[https://www.virtual-dba.com/differences-between-sql-nosql-and-newsql/](https://www.virtual-dba.com/differences-between-sql-nosql-and-newsql/)


### ACID, BASE, CAP

[https://medium.com/@pranabj.aec/acid-cap-and-base-cc73dee43f8c](https://medium.com/@pranabj.aec/acid-cap-and-base-cc73dee43f8c)


### Serializability, linearizability, and locality

[https://aphyr.com/posts/333-serializability-linearizability-and-locality](https://aphyr.com/posts/333-serializability-linearizability-and-locality)


### Distributed Consensus Protocols

[https://www.alibabacloud.com/blog/a-brief-analysis-of-consensus-protocol-from-logical-clock-to-raft_594675](https://www.alibabacloud.com/blog/a-brief-analysis-of-consensus-protocol-from-logical-clock-to-raft_594675)


### Database of Databases

[https://dbdb.io/browse](https://dbdb.io/browse)


## Migration


### Introduction

A video on Cloud Migration.

[https://www.youtube.com/watch?v=Bt_cWJrdfS8](https://www.youtube.com/watch?v=Bt_cWJrdfS8)

[https://cloud.google.com/solutions/migration-to-gcp-getting-started](https://cloud.google.com/solutions/migration-to-gcp-getting-started)


### BigQuery Data Transfer Service

The BigQuery Data Transfer Service automates data movement into BigQuery on a scheduled, managed basis. Your analytics team can lay the foundation for a BigQuery data warehouse without writing a single line of code.

[https://cloud.google.com/bigquery-transfer/docs/transfer-service-overview](https://cloud.google.com/bigquery-transfer/docs/transfer-service-overview)


### Migrate for Compute Engine

Google Cloud Migrate for Compute Engine (formerly Velostrata) migrates VMs from your on-premises data center, AWS, or Azure into Compute Engine.

[https://cloud.google.com/migrate/compute-engine/docs](https://cloud.google.com/migrate/compute-engine/docs)


#### Velostrata

Google Cloud Migrate for Compute Engine (formerly Velostrata) migrates VMs from your on-premises data center, AWS, or Azure into Compute Engine.

[https://cloud.google.com/blog/products/velostrata](https://cloud.google.com/blog/products/velostrata)


#### How to move thousands of VMs to GCP

[https://www.youtube.com/watch?v=WD454APAPV8](https://www.youtube.com/watch?v=WD454APAPV8)


### Cloud Storage Transfer Service

Storage Transfer Service allows you to quickly import online data into Cloud Storage. You can also set up a repeating schedule for transferring data, as well as transfer data within Cloud Storage, from one bucket to another.

[https://cloud.google.com/storage-transfer/docs](https://cloud.google.com/storage-transfer/docs)


### Migrate for Anthos

With Migrate for Anthos, you can migrate your VMs from [supported source platforms](https://cloud.google.com/migrate/anthos/docs/migration-prerequisites) to Google Kubernetes Engine or [Anthos](https://cloud.google.com/anthos).

[https://cloud.google.com/migrate/anthos/docs/getting-started](https://cloud.google.com/migrate/anthos/docs/getting-started)


#### Migrating enterprise workloads using Migrate for Anthos

[https://www.youtube.com/watch?v=8Q1kqWVbKQY](https://www.youtube.com/watch?v=8Q1kqWVbKQY)


### Transfer Appliance

Transfer Appliance is a hardware appliance you can use to securely migrate large volumes of data (from hundreds of terabytes up to 1 petabyte) to Google Cloud Platform without disrupting business operations.

[https://cloud.google.com/transfer-appliance/docs/2.0](https://cloud.google.com/transfer-appliance/docs/2.0)


### Cloud Data Transfer

There are many different ways to transfer data in GCP: Online Transfer, Transfer Service, Transfer Appliance, BigQuery Data Transfer Service and Offline Transfer Methods.

[https://cloud.google.com/products/data-transfer](https://cloud.google.com/products/data-transfer)


### Storage Transfer Service

Whether you're coming from an online or on-premises source, our online storage transfer solutions enable you to manage large-scale data transfers easily, securely, and efficiently. Storage Transfer Service and Transfer Service for on-premises data offer two highly performant pathways to Cloud Storage—both with the scalability and speed you need to simplify the data transfer process.

[https://cloud.google.com/storage-transfer-service](https://cloud.google.com/storage-transfer-service)


### Database Migration Service

[https://cloud.google.com/database-migration](https://cloud.google.com/database-migration)

[https://cloud.google.com/blog/products/databases/database-migration-service-now-available-for-cloud-sql-and-more](https://cloud.google.com/blog/products/databases/database-migration-service-now-available-for-cloud-sql-and-more)


### All Google Cloud Migration Guides

[https://cloud.google.com/blog/products/cloud-migration/guide-to-all-google-cloud-migration-guides](https://cloud.google.com/blog/products/cloud-migration/guide-to-all-google-cloud-migration-guides)


### Big Data Transfer over WAN

[https://asperasoft.com/fileadmin/media/Asperasoft.com/Product_Briefs/Google_AoD_AsperaPB.pdf](https://asperasoft.com/fileadmin/media/Asperasoft.com/Product_Briefs/Google_AoD_AsperaPB.pdf)


### Netapp

[https://cloud.google.com/netapp](https://cloud.google.com/netapp)


#### Trident

[https://github.com/NetApp/trident](https://github.com/NetApp/trident)


#### Cloud Volumes Service 

[https://cloud.netapp.com/cloud-volumes-service-for-gcp](https://cloud.netapp.com/cloud-volumes-service-for-gcp)


### AWS to GCP Data migration

[https://cloud.google.com/migrate/compute-engine/docs/4.2/how-to/migrate-aws-to-gcp/overview](https://cloud.google.com/migrate/compute-engine/docs/4.2/how-to/migrate-aws-to-gcp/overview)


## Networking


### Introduction

Google Cloud Platform includes software-defined networking, hybrid connectivity, network performance optimization, network security, service mesh deployment, NAT, load balancing, and routing.

[https://developers.google.com/learn/topics/networking](https://developers.google.com/learn/topics/networking)

[https://cloud.google.com/about/locations](https://cloud.google.com/about/locations)

[https://www.blog.google/products/google-cloud/expanding-our-global-infrastructure-new-regions-and-subsea-cables/](https://www.blog.google/products/google-cloud/expanding-our-global-infrastructure-new-regions-and-subsea-cables/)


#### Networking 101

[https://www.youtube.com/watch?v=0hN-dyOV10c](https://www.youtube.com/watch?v=0hN-dyOV10c)


#### Networking End to End

[https://www.youtube.com/playlist?list=PLIivdWyY5sqJ0oXcnZYqOnuNRsLF9H48u](https://www.youtube.com/playlist?list=PLIivdWyY5sqJ0oXcnZYqOnuNRsLF9H48u)


#### Two Tier vs. Three Tier Architecture

[https://www.wwt.com/article/comparing-two-tier-three-tier-data-center-networks](https://www.wwt.com/article/comparing-two-tier-three-tier-data-center-networks)


### Jupiter

Jupiter fabrics can deliver more than 1 Petabit/sec of total bisection bandwidth. To put this in perspective, such capacity would be enough for 100,000 servers to exchange information at 10Gb/s each, enough to read the entire scanned contents of the Library of Congress in less than 1/10th of a second.

[https://cloudplatform.googleblog.com/2015/06/A-Look-Inside-Googles-Data-Center-Networks.html](https://cloudplatform.googleblog.com/2015/06/A-Look-Inside-Googles-Data-Center-Networks.html?m=1)


### Network Options


#### Connectivity Options

[https://cloud.google.com/blog/products/networking/google-cloud-network-connectivity-options-explained](https://cloud.google.com/blog/products/networking/google-cloud-network-connectivity-options-explained)

For pricing, quotas, service level agreement (SLA), and release note information for all Network Connectivity products, see the [Network Connectivity resources page](https://cloud.google.com/network-connectivity/docs/resources).

For high-level architectural guides and tutorials that describe networking scenarios for Google Cloud, see the [Technical guides for networking](https://cloud.google.com/docs/tutorials#networking).


#### Choosing Network Products

[https://cloud.google.com/network-connectivity/docs/how-to/choose-product](https://cloud.google.com/network-connectivity/docs/how-to/choose-product)


#### Compare Dedicated Interconnect vs Partner Interconnect

[https://cloud.google.com/network-connectivity/docs/how-to/choose-product#compare-interconnect-solutions](https://cloud.google.com/network-connectivity/docs/how-to/choose-product#compare-interconnect-solutions)


#### Compare Direct Peering to Cloud Interconnect

[https://cloud.google.com/network-connectivity/docs/how-to/choose-product#dp-compare](https://cloud.google.com/network-connectivity/docs/how-to/choose-product#dp-compare)


#### Compare Cloud Interconnect with Carrier Peering

[https://cloud.google.com/network-connectivity/docs/how-to/choose-product#cp-compare](https://cloud.google.com/network-connectivity/docs/how-to/choose-product#cp-compare)


### Virtual Private Cloud (VPC)


#### Introduction

Google Cloud Virtual Private Cloud (VPC) provides networking functionality to Compute Engine virtual machine (VM) instances, Google Kubernetes Engine (GKE) containers, and the App Engine flexible environment. VPC provides networking for your cloud-based services that is global, scalable, and flexible.

[https://cloud.google.com/vpc/docs](https://cloud.google.com/vpc/docs)


#### Migrate from on-prem to cloud using VPC

[https://www.youtube.com/watch?v=cNb7xKyya5c](https://www.youtube.com/watch?v=cNb7xKyya5c)


#### VPC Deep Dive

[https://www.youtube.com/watch?v=wmP6SQe5J7g](https://www.youtube.com/watch?v=wmP6SQe5J7g)

Google Cloud Virtual Private Cloud (VPC) Network Peering allows private connectivity across two VPC networks regardless of whether or not they belong to the same project or the same organization.

VPC networks use Linux's [VIRTIO network module](http://dl.acm.org/citation.cfm?id=1400097.1400108) to model Ethernet card and router functionality, but higher levels of the networking stack, such as ARP lookups, are handled using standard networking software.

[https://cloud.google.com/vpc/docs/advanced-vpc](https://cloud.google.com/vpc/docs/advanced-vpc)


#### Shared VPC and VPC Peering

[Shared VPC](https://cloud.google.com/vpc/docs/shared-vpc) allows an  [organization](https://cloud.google.com/resource-manager/docs/cloud-platform-resource-hierarchy) to connect resources from multiple projects to a common [Virtual Private Cloud (VPC) network](https://cloud.google.com/vpc/docs/vpc), so that they can communicate with each other securely and efficiently using internal IPs from that network. When you use Shared VPC, you designate a project as a host project and attach one or more other service projects to it. The VPC networks in the host project are called Shared VPC networks. [Eligible resources](https://cloud.google.com/vpc/docs/shared-vpc#resources_that_can_be_attached_to_shared_vpc_networks_from_a_service_project) from service projects can use subnets in the Shared VPC network.

Shared VPC lets [organization administrators](https://cloud.google.com/resource-manager/docs/cloud-platform-resource-hierarchy#organizations) delegate administrative responsibilities, such as creating and managing instances, to [Service Project Admins](https://cloud.google.com/vpc/docs/shared-vpc#iam_in_shared_vpc) while maintaining centralized control over network resources like subnets, routes, and firewalls.

Google Cloud VPC Network Peering allows [internal IP address](https://cloud.google.com/vpc/docs/ip-addresses) connectivity across two Virtual Private Cloud (VPC) networks regardless of whether they belong to the same project or the same organization.

[VPC Network Peering](https://cloud.google.com/vpc/docs/vpc-peering) enables you to connect VPC networks so that workloads in different VPC networks can communicate internally. Traffic stays within Google's network and doesn't traverse the public internet.

[https://cloud.google.com/vpc/docs/vpc-peering](https://cloud.google.com/vpc/docs/vpc-peering)


##### VPC network Sharing and Peering

Shared VPC allows you to export subnets from a [VPC network](https://cloud.google.com/vpc/docs/vpc) in a host project to other service projects in the same [organization](https://cloud.google.com/resource-manager/docs/creating-managing-organization). Instances in the service projects can have network connections in the shared subnets of the host project. 

[https://cloud.google.com/vpc/docs/how-to#vpc-network-sharing-and-peering](https://cloud.google.com/vpc/docs/how-to#vpc-network-sharing-and-peering)


### Cloud Router


#### Introduction

Cloud Router enables you to dynamically exchange routes between your Virtual Private Cloud (VPC) and on-premises networks by using [Border Gateway Protocol (BGP)](https://www.wikipedia.org/wiki/Border_Gateway_Protocol). For example, if you use a Cloud VPN tunnel to connect your networks, you can use Cloud Router to establish a BGP session with your on-premises router over your Cloud VPN tunnel. Cloud Router automatically learns new subnets in your VPC network and announces them to your on-premises network.

[https://cloud.google.com/network-connectivity/docs/router](https://cloud.google.com/network-connectivity/docs/router)


#### BGP

[Cloud Router uses Border Gateway Protocol ](https://cloud.google.com/network-connectivity/docs/router/how-to/configuring-bgp)(BGP) to exchange routes between your Virtual Private Cloud (VPC) network and your on-premises network. On Cloud Router, you configure an interface and a BGP peer for your on-premises router. The interface and BGP peer configuration together form a BGP session.

[https://www.youtube.com/watch?v=_Z29ZzKeZHc](https://www.youtube.com/watch?v=_Z29ZzKeZHc)


#### Dynamic Routing

Dynamic routing with Cloud Router.

[https://www.youtube.com/watch?v=K_xb_j46YOk](https://www.youtube.com/watch?v=K_xb_j46YOk)

[https://medium.com/google-cloud/dynamic-routing-with-cloud-router-9ff5c362d833](https://medium.com/google-cloud/dynamic-routing-with-cloud-router-9ff5c362d833)


### Cloud VPN


#### Introduction

Cloud VPN securely extends your [peer](https://cloud.google.com/network-connectivity/docs/vpn/concepts/key-terms#peer-definition) network to Google's network through an IPsec VPN tunnel. Traffic is encrypted and travels between the two networks over the public internet. Cloud VPN is useful for low-volume data connections.

[https://cloud.google.com/network-connectivity/docs/vpn](https://cloud.google.com/network-connectivity/docs/vpn)


#### Types of Cloud VPN


##### Classic VPN

[ Classic VPN ](https://cloud.google.com/network-connectivity/docs/vpn/concepts/overview#classic-vpn)gateways have a single interface, a single external IP address, and support tunnels that use dynamic (BGP) or static routing (policy-based or route-based). They provide an SLA of 99.9% service availability.


##### HA VPN

[HA VPN](https://cloud.google.com/network-connectivity/docs/vpn/concepts/overview#ha-vpn) lets you easily set up redundant VPNs to isolate failures and provide continuous connectivity for workloads that are too important to fail. 

Use Case 1: Migrate an existing Classic VPN solution to HA VPN utilizing BGP as the routing protocol to an on-premises network (or any non Google Networks). Use Case 2: Migrate an existing Classic VPN utilizing policy based VPN to HA VPN utilizing BGP between two projects or VPCs within Google Cloud Platform.

[https://www.youtube.com/watch?v=lIEExVWf5bg](https://www.youtube.com/watch?v=lIEExVWf5bg)

If a Cloud VPN tunnel goes down, it restarts automatically. If an entire virtual VPN device fails, Cloud VPN automatically instantiates a new one with the same configuration. The new gateway and tunnel connect automatically.

VPN tunnels connected to HA VPN gateways must use dynamic (BGP) routing. Depending on the way that you configure route priorities for HA VPN tunnels, you can create an active/active or active/passive routing configuration. For both of these routing configurations, both VPN tunnels remain active.


##### Active/active vs. active/passive routing options for HA VPN

[https://cloud.google.com/network-connectivity/docs/vpn/concepts/overview#active](https://cloud.google.com/network-connectivity/docs/vpn/concepts/overview#active)


##### Comparison between HA VPN and Classic VPN

[https://cloud.google.com/network-connectivity/docs/vpn/concepts/overview#comparison_table](https://cloud.google.com/network-connectivity/docs/vpn/concepts/overview#comparison_table)


#### Cloud VPN Topologies

With Cloud VPN, your on-premises hosts communicate through one or more IPsec VPN tunnels to Compute Engine Virtual Machine (VM) instances in your project's VPC networks.

[https://cloud.google.com/network-connectivity/docs/vpn/concepts/topologies](https://cloud.google.com/network-connectivity/docs/vpn/concepts/topologies)


##### HA VPN to peer VPN Gateways

[https://cloud.google.com/network-connectivity/docs/vpn/concepts/topologies#to_peer_vpn_gateways](https://cloud.google.com/network-connectivity/docs/vpn/concepts/topologies#to_peer_vpn_gateways)


##### HA VPN to AWS peer Gateways

[https://cloud.google.com/network-connectivity/docs/vpn/concepts/topologies#to_aws_peer_gateways](https://cloud.google.com/network-connectivity/docs/vpn/concepts/topologies#to_aws_peer_gateways)


##### HA VPN between Google Cloud networks

[https://cloud.google.com/network-connectivity/docs/vpn/concepts/topologies#2-gcp-gateways](https://cloud.google.com/network-connectivity/docs/vpn/concepts/topologies#2-gcp-gateways)


### Cloud DNS


#### Introduction

Publish your domain names by using Google's infrastructure for production-quality, high-volume DNS services. Google's global network of anycast name servers provides reliable, low-latency, authoritative name lookups for your domains from anywhere in the world.

[https://cloud.google.com/dns/docs](https://cloud.google.com/dns/docs)


#### DNS & SSL

[https://www.youtube.com/watch?v=sTDVsMUegL8](https://www.youtube.com/watch?v=sTDVsMUegL8)


##### Cert Manager, Kubernetes, Let’s Encrypt

[https://www.youtube.com/watch?v=LH4nLtUpuBI](https://www.youtube.com/watch?v=LH4nLtUpuBI)


#### IP Addresses, Netmasks

[https://www.youtube.com/watch?v=EkNq4TrHP_U](https://www.youtube.com/watch?v=EkNq4TrHP_U)


### Identity, Security, AuthN, AuthZ

Access control for Google Cloud APIs encompasses authentication, authorization, and auditing. Authentication determines who you are, authorization determines what you can do, and auditing logs what you did.  For authorization, see [Identity and Access Management](https://cloud.google.com/iam/docs) (IAM). For auditing, see [Cloud Audit Logs](https://cloud.google.com/logging/docs/audit).

https://cloud.google.com/docs/authentication


#### PKI

A public key infrastructure (PKI) is a set of roles, policies, hardware, software and procedures needed to create, manage, distribute, use, store and revoke [digital certificates](https://en.wikipedia.org/wiki/Public_key_certificate) and manage [public-key encryption](https://en.wikipedia.org/wiki/Public-key_cryptography). The purpose of a PKI is to facilitate the secure electronic transfer of information for a range of network activities such as e-commerce, internet banking and confidential email. It is required for activities where simple passwords are an inadequate authentication method and more rigorous proof is required to confirm the identity of the parties involved in the communication and to validate the information being transferred.

[https://www.ssh.com/pki/](https://www.ssh.com/pki/)


#### OAthu, OpenID Connect, SAML

[https://www.okta.com/identity-101/whats-the-difference-between-oauth-openid-connect-and-saml/](https://www.okta.com/identity-101/whats-the-difference-between-oauth-openid-connect-and-saml/)


### Cloud CDN


#### Introduction

Cloud CDN (Content Delivery Network) uses Google's globally distributed edge points of presence to cache external HTTP(S) load balanced content close to your users. Caching content at the edges of Google's network provides faster delivery of content to your users while reducing serving costs.

[https://cloud.google.com/cdn/docs](https://cloud.google.com/cdn/docs)


#### Using CDN and Load Balancing

[https://www.youtube.com/watch?v=NedNhOg_TgA](https://www.youtube.com/watch?v=NedNhOg_TgA)


#### Setting up Cloud CDN with backend storage bucket

[https://cloud.google.com/cdn/docs/setting-up-cdn-with-bucket](https://cloud.google.com/cdn/docs/setting-up-cdn-with-bucket)


### Hybrid Connectivity

[https://cloud.google.com/hybrid-connectivity](https://cloud.google.com/hybrid-connectivity)


### Cloud Interconnect


#### Introduction

Cloud Interconnect extends your on-premises network to Google's network through a highly available, low latency connection. You can use Dedicated Interconnect to connect directly to Google or use Partner Interconnect to connect to Google through a supported service provider.

[https://cloud.google.com/network-connectivity/docs/interconnect](https://cloud.google.com/network-connectivity/docs/interconnect)

While migrating portions of your on-prem to the cloud, it’s important for your on-prem systems to communicate with your newly minted cloud resource.

[https://www.youtube.com/watch?v=cKaryf7qp9w](https://www.youtube.com/watch?v=cKaryf7qp9w)


#### Dedicated Interconnect

Dedicated Interconnect provides direct physical connections between your on-premises network and Google's network. Dedicated Interconnect enables you to transfer large amounts of data between networks, which can be more cost effective than purchasing additional bandwidth over the public Internet.

[https://cloud.google.com/network-connectivity/docs/interconnect](https://cloud.google.com/network-connectivity/docs/interconnect)

 After you create a VLAN attachment, you need to configure your on-premises router to establish a BGP session with your Cloud Router. Use the VLAN ID, interface IP address, and peering IP address provided by the [VLAN attachment](https://cloud.google.com/network-connectivity/docs/interconnect/how-to/dedicated/creating-vlan-attachments) to configure your on-premises router.

[https://cloud.google.com/network-connectivity/docs/interconnect/how-to/dedicated/configuring-onprem-routers](https://cloud.google.com/network-connectivity/docs/interconnect/how-to/dedicated/configuring-onprem-routers)


#### Partner Interconnect

Partner Interconnect provides connectivity between your on-premises network and your VPC network through a supported [service provider](https://cloud.google.com/network-connectivity/docs/interconnect/concepts/service-providers). A Partner Interconnect connection is useful if your data center is in a physical location that can't reach a Dedicated Interconnect colocation facility or if your data needs don't warrant an entire 10 Gbps connection.

[https://cloud.google.com/network-connectivity/docs/interconnect](https://cloud.google.com/network-connectivity/docs/interconnect)

An on-premises router in this context means a Layer 2 (L2) or Layer 3 (L3) device you configure to enable Partner Interconnect.

[https://cloud.google.com/network-connectivity/docs/interconnect/how-to/partner/configuring-onprem-routers](https://cloud.google.com/network-connectivity/docs/interconnect/how-to/partner/configuring-onprem-routers)


### Peering

[https://www.peeringdb.com/net/433](https://www.peeringdb.com/net/433)


#### Direct Peering

[https://cloud.google.com/network-connectivity/docs/direct-peering](https://cloud.google.com/network-connectivity/docs/direct-peering)

Direct Peering enables you to establish a direct [peering](https://www.wikipedia.org/wiki/Peering) connection between your business network and Google's edge network and exchange high-throughput cloud traffic.

Direct Peering exists outside of Google Cloud. Unless you need to access Google Workspace applications, the recommended methods of access to Google Cloud are [Dedicated Interconnect](https://cloud.google.com/network-connectivity/docs/interconnect/concepts/dedicated-overview) or [Partner Interconnect](https://cloud.google.com/network-connectivity/docs/interconnect/concepts/partner-overview).


#### Carrier Peering

Carrier Peering enables you to access Google applications, such as Google Workspace, by using a [service provider](https://cloud.google.com/network-connectivity/docs/carrier-peering#service-providers) to obtain enterprise-grade network services that connect your infrastructure to Google.

[https://cloud.google.com/network-connectivity/docs/carrier-peering](https://cloud.google.com/network-connectivity/docs/carrier-peering)


### Cloud Load Balancing


#### Introduction

Cloud Load Balancing allows you to put your resources behind a single IP address that is externally accessible or internal to your Virtual Private Cloud (VPC) network.

[https://cloud.google.com/load-balancing/docs](https://cloud.google.com/load-balancing/docs)

A Video about Cloud Load Balancing.

[https://www.youtube.com/watch?v=D4XZkCJyqis](https://www.youtube.com/watch?v=D4XZkCJyqis)

Google Cloud Load Balancing enables enterprises and cloud-natives to deliver highly available, scalable, low-latency cloud services with a global footprint. Use Google Global Load Balancing to deliver global reach and scale. Deploy your application backends in single or multiple regions wherever your users are, front-ending these with a single anycast VIP, and growing or shrinking your backend resources with intelligent Autoscaling. Scale private services using Internal Load Balancing (ILB) for clients in Google Cloud or on-prem across Interconnect/VPN. 

[https://www.youtube.com/watch?v=J5HJ1y6PeyE](https://www.youtube.com/watch?v=J5HJ1y6PeyE)


#### Types of Load Balancing

[https://cloud.google.com/load-balancing/docs/load-balancing-overview](https://cloud.google.com/load-balancing/docs/load-balancing-overview)

[https://cloud.google.com/blog/products/networking/google-cloud-networking-in-depth-cloud-load-balancing-deconstructed](https://cloud.google.com/blog/products/networking/google-cloud-networking-in-depth-cloud-load-balancing-deconstructed)


##### Maglev

[https://research.google/pubs/pub44824/](https://research.google/pubs/pub44824/)


##### Andromeda

[https://www.usenix.org/system/files/conference/nsdi18/nsdi18-dalton.pdf](https://www.usenix.org/system/files/conference/nsdi18/nsdi18-dalton.pdf)


#### Load Balancer Options

To decide which load balancer best suits your implementation of Google Cloud, consider the following aspects of Cloud Load Balancing:



*   Global versus regional load balancing
*   External versus internal load balancing
*   Traffic type

[https://cloud.google.com/load-balancing/docs/choosing-load-balancer](https://cloud.google.com/load-balancing/docs/choosing-load-balancer)


### Cloud NAT

Cloud NAT provides fully managed, software-defined network address translation support for Google Cloud.

[https://cloud.google.com/nat/docs](https://cloud.google.com/nat/docs)

Moving your internal services to the cloud can bring you a handful of new, useful features, but one of the biggest challenges is protecting your internal endpoints. 

[https://www.youtube.com/watch?v=bmaarG0IkH8](https://www.youtube.com/watch?v=bmaarG0IkH8)


### Cloud Armor

Google Cloud Armor helps protect your infrastructure and applications from distributed denial-of-service (DDoS) attacks by using Google's global infrastructure and security systems.

[https://cloud.google.com/armor/docs](https://cloud.google.com/armor/docs)

Setting up Cloud Armor.

[https://www.youtube.com/watch?v=g_c2KLpnWck](https://www.youtube.com/watch?v=g_c2KLpnWck)


### Network Intelligence Center

Network Intelligence Center provides a single console for managing Google Cloud network visibility, monitoring, and troubleshooting.

[https://cloud.google.com/network-intelligence-center/docs](https://cloud.google.com/network-intelligence-center/docs)

Getting started with topology in network intelligence center.

[https://www.youtube.com/watch?v=ID7szIL9eew](https://www.youtube.com/watch?v=ID7szIL9eew)


### Network Service Tiers

With Network Service Tiers, Google Cloud is the first major public cloud to offer a tiered cloud network. Select the right tier of network service for your requirements and budget.

[https://cloud.google.com/network-tiers](https://cloud.google.com/network-tiers)

Cost savings using different network tiers.

[https://www.youtube.com/watch?v=wsdgWGE-mwE](https://www.youtube.com/watch?v=wsdgWGE-mwE)


### Network Telemetry

VPC Flow Logs records a sample of network flows sent from and received by VM instances, including instances used as GKE nodes. These logs can be used for network monitoring, forensics, real-time security analysis, and expense optimization.

[https://cloud.google.com/vpc/docs/using-flow-logs](https://cloud.google.com/vpc/docs/using-flow-logs)

Network and security telemetry is fundamental to operate your deployments in public clouds with confidence, providing the required visibility on the behavior of your network and Access control firewalls. 

[https://www.youtube.com/watch?v=as9mXNEcaDo](https://www.youtube.com/watch?v=as9mXNEcaDo)


### Traffic Director

Traffic Director is Google Cloud's fully managed traffic control plane for service mesh. With Traffic Director, you can deploy global load balancing across clusters and virtual machine (VM) instances in multiple regions, offload health checking from service proxies, and configure sophisticated traffic control policies.

[https://cloud.google.com/traffic-director/docs](https://cloud.google.com/traffic-director/docs)

Traffic Director is toil-free, GCP-managed control plane with SLA for Service Meshes.

 In Istio environments, Traffic Director provides a GCP-managed Pilot for your service mesh. 

Traffic Director delivers traffic management and multi-region global load balancing for service meshes built using open proxies like Envoy and through the open xDSv2 APIs. It provides policy driven traffic routing, enabling you to control the flow of traffic between services. All of this makes load balancing, scaling, A/B testing, canary roll outs, and blue-green deployments easy  to set up. Traffic Director also provides centralized high fidelity health checking, and traffic driven autoscaling. Envoy-based Layer 7 Internal Load Balancing (L7 ILB), another flavor of Traffic Director, brings modern traffic management capabilities to traditional environments. With L7 ILB, Traffic Director controls a pool of GCP-managed Envoy proxies under the hood but presents this service as a traditional Layer 7 ILB middle proxy to front your legacy apps. 

Traffic Director supports VM-based, Kubernetes and GKE apps.

[https://www.youtube.com/watch?v=FUITCYMCEhU](https://www.youtube.com/watch?v=FUITCYMCEhU)


### Service Directory

Service Directory helps reduce the complexity of management and operations by providing a single place to publish, discover, and connect services. It is a managed service that enhances service inventory management at scale so you don’t have to. Service Directory provides real-time service information, whether you have a few service endpoints or thousands. 

[https://cloud.google.com/service-directory](https://cloud.google.com/service-directory)

[https://www.youtube.com/watch?v=H9UoE_cWIEY](https://www.youtube.com/watch?v=H9UoE_cWIEY)


### Qwiklabs


#### Networking

Networking is a principle theme of cloud computing. It’s the underlying structure of Google Cloud, and it’s what connects all your resources and services to one another. This fundamental-level quest will cover essential Google Cloud networking services and will give you hands-on practice with specialized tools for developing mature networks. From learning the ins-and-outs of VPCs, to creating enterprise-grade load balancers, Networking in the Google Cloud will give you the practical experience needed so you can start building robust networks right away.

[Networking in the Google Cloud](https://www.qwiklabs.com/quests/31?catalog_rank=%7B%22rank%22%3A4%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&search_id=7467791)


#### Secure Networks

[Build and Secure Networks in Google Cloud](https://www.qwiklabs.com/quests/128?catalog_rank=%7B%22rank%22%3A1%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&search_id=7467791)


#### Network Performance

This quest is composed of labs that cover real-life use cases and it will teach you best practices for overcoming common networking bottlenecks. From getting hands-on practice with testing and improving network performance, to integrating high-throughput VPNs and networking tiers, Network Performance and Optimization is an essential quest for GCP developers who are looking to double down on application speed and robustness. \


[Network Performance and Optimization](https://www.qwiklabs.com/quests/46?catalog_rank=%7B%22rank%22%3A2%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&search_id=7467791)


#### VPC Networking Fundamentals

Google Cloud Virtual Private Cloud (VPC) provides networking functionality to Compute Engine virtual machine (VM) instances, Kubernetes Engine containers and App Engine Flex. In other words, without a VPC network you cannot create VM instances, containers or App Engine applications. Therefore, each Google Cloud project has a default network to get you started.

You can think of a VPC network the same way you would think of a physical network, except that it is virtualized within Google Cloud. A VPC network is a global resource which consists of a list of regional virtual subnetworks (subnets) in data centers, all connected by a global wide area network (WAN). VPC networks are logically isolated from each other in Google Cloud.

[VPC Networking Fundamentals](https://www.qwiklabs.com/focuses/1229?catalog_rank=%7B%22rank%22%3A11%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&parent=catalog&search_id=7467802)


#### VPC Network Peering

VPC Network Peering allows you to build SaaS (Software-as-a-Service) ecosystems in Google Cloud, making services available privately across different VPC networks within and across organizations, allowing workloads to communicate in private space.

[VPC Network Peering](https://www.qwiklabs.com/focuses/964?catalog_rank=%7B%22rank%22%3A10%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&parent=catalog&search_id=7467800)


#### Performance Optimization

This quest is composed of labs that cover real-life use cases and it will teach you best practices for overcoming common networking bottlenecks. From getting hands-on practice with testing and improving network performance, to integrating high-throughput VPNs and networking tiers, Network Performance and Optimization is an essential quest for GCP developers who are looking to double down on application speed and robustness.

[Network Performance and Optimization](https://www.qwiklabs.com/quests/46?catalog_rank=%7B%22rank%22%3A3%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&search_id=7468028)


#### VPC Flow Logs

In this lab, you will learn how to configure a network to record traffic to and from an Apache web server using VPC Flow Logs. You will then export the logs to BigQuery for analysis. There are multiple use cases for VPC Flow Logs. For example, you might use VPC Flow Logs to determine where your applications are being accessed from to optimize network traffic expense, to create HTTP Load Balancers to balance traffic globally, or to denylist unwanted IP addresses with Cloud Armor.

[VPC Flow Logs - Analyzing Network Traffic](https://www.qwiklabs.com/focuses/1236?catalog_rank=%7B%22rank%22%3A12%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&parent=catalog&search_id=7467802)


#### Multiple VPC Networks

In this lab you create several VPC networks and VM instances and test connectivity across networks. Specifically, you create two custom mode networks (managementnet and privatenet) with firewall rules and VM instances. The mynetwork network with its firewall rules and two VM instances (mynet-eu-vm and mynet-us-vm) have already been created for you in this Qwiklabs project.

[Multiple VPC Networks](https://www.qwiklabs.com/focuses/1230?catalog_rank=%7B%22rank%22%3A13%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&parent=catalog&search_id=7467802)


#### Controlling Access

In this lab, you create two nginx web servers and control external HTTP access to the web servers using tagged firewall rules. Then, you explore IAM roles and service accounts.

[VPC Networks - Controlling Access](https://www.qwiklabs.com/focuses/1231?catalog_rank=%7B%22rank%22%3A15%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&parent=catalog&search_id=7467802)


#### Using VPC Network Peering

In this lab, you configure VPC Network Peering between two networks. Then, you verify private communication between two VMs in those networks. VPC Network Peering allows you to build SaaS (Software-as-a-Service) ecosystems on Google Cloud, making services available privately across different VPC networks within and across organizations, allowing workloads to communicate in private RFC 1918 space.

[Using VPC Network Peering](https://www.qwiklabs.com/focuses/1249?catalog_rank=%7B%22rank%22%3A16%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&parent=catalog&search_id=7467802)


#### HA-VPN

HA-VPN is IPSec VPN solution to enable secure connectivity between your on-premise network to your Google Cloud Platform (GCP) Virtual Private Cloud (VPC) network through an IPSec VPN connection with 99.99% service availability at GA. HA-VPN is a regional per VPC VPN solution. HA-VPN gateways have two interfaces, each with their own public IP address. When you create a HA-VPN gateway, two public IP addresses are automatically chosen from different address pools. When HA-VPN is configured with two tunnels, Cloud VPN offers a 99.99% service availability uptime.

[VPC Networking: Cloud HA-VPN](https://www.qwiklabs.com/focuses/6270?catalog_rank=%7B%22rank%22%3A18%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&parent=catalog&search_id=7467802)


#### Cloud Routers

In this lab, you configure Cloud Routers using the Console. The Cloud Routers will implement VPN gateways configured with BGP. BGP provides dynamic network discovery and eliminates the need to configure or maintain static routes. When successful you will be able to ping the internal IP of the VM in a newly discovered subnetwork via an auto-populated route.

[Dynamic VPN Gateways - Cloud Routers ](https://www.qwiklabs.com/focuses/1233?parent=catalog)


#### Service Directory

Service Directory provides real-time service information, whether you have a few service endpoints or thousands. This helps ensure that your applications only resolve the most updated information of their resources, increasing the reachability of your services. With Service Directory, you can easily understand all your services across multi-cloud environments. This includes workloads running in Compute Engine VMs, Google Kubernetes Engine (GKE), as well as external services running on-prem and third-party clouds. It improves application reachability by maintaining the endpoint information for all your services.

[Service Directory: Qwik Start](https://www.qwiklabs.com/focuses/12412?catalog_rank=%7B%22rank%22%3A19%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&parent=catalog&search_id=7468061)


## Serverless Computing


### Introduction

Google Cloud’s serverless platform lets you write code your way without worrying about the underlying infrastructure. Deploy functions or apps as source code or as containers. Build full stack serverless applications with Google Cloud’s storage, databases, machine learning, and more. Easily extend applications with event-driven computing from Google or third-party service integrations. You can even choose to move your serverless workloads to on-premises environments or to the cloud.

[https://www.youtube.com/watch?v=PBw9vD_BO5A](https://www.youtube.com/watch?v=PBw9vD_BO5A)


### Cloud Run

Cloud Run is a managed compute platform that enables you to run stateless containers that are invocable via web requests or Pub/Sub events. 

[http://cloud.run](http://cloud.run/)

Cloud Run is serverless: it abstracts away all infrastructure management, so you can focus on what matters most — building great applications. It is built from [Knative](https://cloud.google.com/knative/), letting you choose to run your containers either fully managed with Cloud Run, in your Google Kubernetes Engine cluster, or in workloads on-premises with Cloud Run for Anthos.

[https://cloud.google.com/run/docs](https://cloud.google.com/run/docs)


#### Quickstart: Build and Deploy

This interactive tutorial can be opened in Cloud Shell editor (theia) and followed step by step.

[https://cloud.google.com/run/docs/quickstarts/build-and-deploy](https://cloud.google.com/run/docs/quickstarts/build-and-deploy)


#### Use Cases

[https://cloud.google.com/run/#section-6](https://cloud.google.com/run/#section-6)

Learn how to deploy serverless containers in 3 environments using Cloud Run and Knative.

[https://www.youtube.com/watch?v=nhwYc4StHIc](https://www.youtube.com/watch?v=nhwYc4StHIc)

A video on migrating kubernetes apps to serverless with Cloud Run on Anthos.

[https://www.youtube.com/watch?v=0T5UliS9j8A](https://www.youtube.com/watch?v=0T5UliS9j8A)


### App Engine

App Engine is a fully managed, serverless platform for developing and hosting web applications at scale. You can choose from several popular languages, libraries, and frameworks to develop your apps, then let App Engine take care of provisioning servers and scaling your app instances based on demand.

[https://cloud.google.com/appengine/docs](https://cloud.google.com/appengine/docs)

Google App Engine makes it easy to focus on your code, while letting us manage your infrastructure.

[https://www.youtube.com/watch?v=2PRciDpqpko](https://www.youtube.com/watch?v=2PRciDpqpko)


### Cloud Functions

[Google Cloud Functions](https://cloud.google.com/functions/docs/concepts/overview) is a lightweight compute solution for developers to create single-purpose, stand-alone functions that respond to Cloud events without the need to manage a server or runtime environment.

[https://cloud.google.com/functions/docs](https://cloud.google.com/functions/docs)

A video tutorial of Cloud Functions that  will show you how to deploy a Cloud Function from a Google Cloud project.  You will learn how to test your function and see your log entries. 

[https://www.youtube.com/watch?v=vM-2O-uKBNQ](https://www.youtube.com/watch?v=vM-2O-uKBNQ)


#### Cloud Functions for .NET

[https://cloud.google.com/blog/products/application-development/introducing-net-google-cloud-functions](https://cloud.google.com/blog/products/application-development/introducing-net-google-cloud-functions)


### Knative

Knative (pronounced kay-nay-tiv) extends [Kubernetes](https://kubernetes.io/docs/concepts/overview/what-is-kubernetes/) to provide a set of middleware components that are essential to build modern, source-centric, and container-based applications that can run anywhere: on premises, in the cloud, or even in a third-party data center. Each of the components under the Knative project attempt to identify common patterns and codify the best practices that are shared by successful, real-world, Kubernetes-based frameworks and applications. Knative components focus on solving mundane but difficult tasks such as:



*   [Deploying a container](https://knative.dev/docs/serving/getting-started-knative-app)
*   [Routing and managing traffic with blue/green deployment](https://knative.dev/docs/serving/samples/blue-green-deployment)
*   [Scaling automatically and sizing workloads based on demand](https://knative.dev/docs/serving/autoscaling)
*   [Binding running services to eventing ecosystems](https://knative.dev/docs/eventing/getting-started)

Developers on Knative can use familiar idioms, languages, and frameworks to deploy functions, applications, or containers workloads.

Knative consists of the Serving and Eventing components:



*   [Eventing](https://knative.dev/docs/eventing) - Management and delivery of events
*   [Serving](https://knative.dev/docs/serving) - Request-driven compute that can scale to zero

[https://knative.dev/](https://knative.dev/)

Run managed serverless containers with Knative.

[https://www.youtube.com/watch?v=wPLjUF1hFCw](https://www.youtube.com/watch?v=wPLjUF1hFCw)


#### Cloud Run

[https://cloud.google.com/blog/products/serverless/knative-based-cloud-run-services-are-ga](https://cloud.google.com/blog/products/serverless/knative-based-cloud-run-services-are-ga)


### Workflows

You can use Workflows to create serverless workflows that link a series of serverless tasks together in an order you define. Combine the power of Google Cloud's APIs, serverless products like Cloud Functions and Cloud Run, and calls to external APIs to create flexible serverless applications. Workflows require no infrastructure management and scales seamlessly with demand, including scaling down to zero.

[https://cloud.google.com/workflows/docs](https://cloud.google.com/workflows/docs)

Build serverless workflows orchestrating various products and API calls within Google Cloud and beyond. 

[https://www.youtube.com/watch?v=Uz8G8fTwwXs](https://www.youtube.com/watch?v=Uz8G8fTwwXs)


### Serverless Predictions at Scale

Cloud Machine Learning Engine Prediction Service can serve TensorFlow models and scale.

[https://www.youtube.com/watch?v=_JCMN8-yhBM](https://www.youtube.com/watch?v=_JCMN8-yhBM)


### Qwiklabs


#### Deploy on Cloud Run

This is a Qwiklab to show you how to deploy a website using Cloud Run.

[Deploy Your Website on Cloud Run](https://www.qwiklabs.com/focuses/10445?parent=catalog)


#### Web Applications on Cloud Run

It is a part of the larger “Quest”.

[Websites and Web Applications](https://www.qwiklabs.com/quests/39?catalog_rank=%7B%22rank%22%3A5%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&search_id=7467936)


#### Monitoring Cloud Functions

You can [view your Cloud Functions](https://cloud.google.com/functions) with their execution times,execution counts, and memory usage in the Cloud Console using [Cloud Monitoring](https://cloud.google.com/monitoring), where you can set up custom alerting on these metrics.

[Monitoring and Logging for Cloud Functions](https://www.qwiklabs.com/focuses/1833?catalog_rank=%7B%22rank%22%3A16%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&parent=catalog&search_id=7468061)


#### Logging in Google Cloud

Learn how to monitor, troubleshoot, and improve your infrastructure and application performance. Guided by the principles of Site Reliability Engineering (SRE), this course features a combination of lectures, demos, hands-on labs, and real-world case studies. In this course, you'll gain experience with full-stack monitoring, real-time log management and analysis, debugging code in production, and profiling CPU and memory usage.

[Logging, Monitoring and Observability in Google Cloud](https://www.qwiklabs.com/courses/1514?catalog_rank=%7B%22rank%22%3A17%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&search_id=7468061)


#### Stackdriver Cloud Functions

In this lab you will learn how to use Cloud Functions to perform lightweight processing of Stackdriver Logging messages.

[Responding to Stackdriver Messages with Cloud Functions](https://www.qwiklabs.com/focuses/8500?catalog_rank=%7B%22rank%22%3A22%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&parent=catalog&search_id=7468090)


## Hybrid and Multi-cloud


### Anthos

Anthos is a modern application management platform that provides a consistent development and operations experience for cloud and on-premises environments. This page provides an overview of each layer of the Anthos infrastructure and shows how you can leverage its features.

[https://cloud.google.com/anthos/docs](https://cloud.google.com/anthos/docs)

Getting started with Anthos.

[https://www.youtube.com/watch?v=DM8p_cnc6ZY](https://www.youtube.com/watch?v=DM8p_cnc6ZY)

A sample deployment for Anthos. 

[https://www.youtube.com/watch?v=qgg1ceR6-es](https://www.youtube.com/watch?v=qgg1ceR6-es)

VM instances can exist on premises, managed by products such as VMWare vSphere, and in public clouds such as AWS or Azure, in addition to Google Cloud Compute Engine instances.


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


## Operations

AKA Stackdriver


### Introduction

Monitor, troubleshoot, and improve application performance on your Google Cloud environment.

[https://cloud.google.com/stackdriver/docs](https://cloud.google.com/stackdriver/docs)

Introduction to basic logging and monitoring with Stackdriver with a quick demo.

[https://www.youtube.com/watch?v=LVFr5qW4wO4](https://www.youtube.com/watch?v=LVFr5qW4wO4)


### Cloud Logging

Cloud Logging allows you to store, search, analyze, monitor, and alert on logging data and events from Google Cloud and Amazon Web Services. Using Cloud Logging includes access to the [BindPlane service](https://bluemedora.com/products/bindplane/bindplane-for-stackdriver/), which you can use to collect logging data from over 150 common application components, on-premises systems, and hybrid cloud systems.

[https://cloud.google.com/logging/docs](https://cloud.google.com/logging/docs)

GCP Essentials: Cloud Logging.

[https://www.youtube.com/watch?v=gyDp-Cl_MdA](https://www.youtube.com/watch?v=gyDp-Cl_MdA)


### Cloud Monitoring

Cloud Monitoring collects metrics, events, and metadata from Google Cloud, Amazon Web Services (AWS), hosted uptime probes, and application instrumentation. Using the [BindPlane service](https://bluemedora.com/products/bindplane/bindplane-for-stackdriver/), you can also collect this data from over 150 common application components, on-premise systems, and hybrid cloud systems. Google Cloud's operations suite ingests that data and generates insights via dashboards, charts, and alerts. BindPlane is included with your Google Cloud project at no additional cost.

[https://cloud.google.com/monitoring/docs](https://cloud.google.com/monitoring/docs)

Getting started with Cloud Monitoring.

[https://www.youtube.com/watch?v=wY8cmFY4ua8](https://www.youtube.com/watch?v=wY8cmFY4ua8)


#### Cloud Monitoring Agents

[https://cloud.google.com/monitoring/agent](https://cloud.google.com/monitoring/agent)


#### Dashboards

[https://cloud.google.com/monitoring/charts/dashboards](https://cloud.google.com/monitoring/charts/dashboards)


#### Metrics Explorer

[https://cloud.google.com/monitoring/charts/metrics-explorer](https://cloud.google.com/monitoring/charts/metrics-explorer)


### Cloud Trace

Cloud Trace is a distributed tracing system for Google Cloud that collects latency data from applications and displays it in near real-time in the [Google Cloud Console](https://console.cloud.google.com/).

[https://cloud.google.com/trace/docs](https://cloud.google.com/trace/docs)

Cloud Trace is a feature of the Google Cloud Platform that allows you to view the RPCs (remote procedure calls) invoked by your App Engine application and to view and analyze the time taken to complete each RPC and the overall latency of processing your applications requests.

[https://www.youtube.com/watch?v=NCFDqeo7AeY](https://www.youtube.com/watch?v=NCFDqeo7AeY)


### Cloud Debugger

Cloud Debugger is a feature of Google Cloud Platform that lets you inspect the state of an application, at any code location, without stopping or slowing down the running app. Cloud Debugger makes it easier to view the application state without adding logging statements.

[https://cloud.google.com/debugger/docs](https://cloud.google.com/debugger/docs)

Cloud Debugger makes it easier to view the application state at any point in the code without any modifications to your code.  

[https://www.youtube.com/watch?v=DCtLE6zPMdQ](https://www.youtube.com/watch?v=DCtLE6zPMdQ)


### Cloud Profiler

Cloud Profiler is a statistical, low-overhead profiler that continuously gathers CPU usage and memory-allocation information from your production applications. It attributes that information to the application's source code, helping you identify the parts of the application consuming the most resources, and otherwise illuminating the performance characteristics of the code.

[https://cloud.google.com/profiler/docs](https://cloud.google.com/profiler/docs)

Introduction to Stackdriver Profiler.

[https://www.youtube.com/watch?v=KXjPhadwr8k](https://www.youtube.com/watch?v=KXjPhadwr8k)


### Error Reporting

Error Reporting aggregates and displays errors produced in your running cloud services.

[https://cloud.google.com/error-reporting/docs](https://cloud.google.com/error-reporting/docs)

Error reporting can be useful in identifying and resolving bugs in your application. 

[https://www.youtube.com/watch?v=GANi9eRxhHs](https://www.youtube.com/watch?v=GANi9eRxhHs)


### Service Level Monitoring

Service monitoring and the SLO API help you manage your services like Google manages its own services. 

[https://cloud.google.com/stackdriver/docs/solutions/slo-monitoring](https://cloud.google.com/stackdriver/docs/solutions/slo-monitoring)

Basics of Service Level Monitoring.

[https://www.youtube.com/watch?v=u84TKyX8SfU](https://www.youtube.com/watch?v=u84TKyX8SfU)


### Qwiklabs


#### Operations Suite

In this fundamental-level quest, you will learn the ins and outs of Google Cloud's operations suite, an important service for generating insights into the health of your applications. It provides a wealth of information in application monitoring, report logging, and diagnoses. The labs in this quest will give you hands-on practice with and will teach you how to monitor virtual machines, generate logs and alerts, and create custom metrics for application data.

[Google Cloud's Operations Suite](https://www.qwiklabs.com/quests/35?catalog_rank=%7B%22rank%22%3A6%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&search_id=7468028)


#### Cloud Monitoring

In this fundamental-level quest, you will learn the ins and outs of Google Cloud's operations suite, an important service for generating insights into the health of your applications. It provides a wealth of information in application monitoring, report logging, and diagnoses. The labs in this quest will give you hands-on practice with and will teach you how to monitor virtual machines, generate logs and alerts, and create custom metrics for application data. 

[Monitor and Log with Google Cloud Operations Suite](https://www.qwiklabs.com/quests/143?catalog_rank=%7B%22rank%22%3A2%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&search_id=7468028)


#### Cloud Trace

When supporting a production system that services HTTP requests or provides an API, it is important to measure the latency of your endpoints to detect when a system's performance is not operating within specification. In monolithic systems this single latency measure may be useful to detect and diagnose deteriorating behavior. With modern microservice architectures, however, this becomes much more difficult because a single request may result in numerous additional requests to other systems before the request can be fully handled. Deteriorating performance in an underlying system may impact all other systems that rely on it. While latency can be measured at each service endpoint, it can be difficult to correlate slow behavior in the public endpoint with a particular sub-service that is misbehaving.

[Using Cloud Trace on Kubernetes Engine](https://www.qwiklabs.com/focuses/5159?catalog_rank=%7B%22rank%22%3A19%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&parent=catalog&search_id=7468017)


#### Cloud Logging

Cloud Logging is a fully managed service that performs at scale. It can ingest application and system log data from thousands of VMs and, even better, analyze all that log data in real time. In this fundamental-level Quest, you learn how to store, search, analyze, monitor, and alert on log data and events from Google Cloud. 

[Cloud Logging](https://www.qwiklabs.com/quests/81?catalog_rank=%7B%22rank%22%3A1%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&search_id=7468028)


#### Application Logs

In this hands-on lab, you learn how to use Cloud Logging to accumulate application logs in a single place, filter to reach the required log, understand how to create logs based metrics for advanced analysis, examine the audit logs use case, and export logs for compliance and/or advanced analysis needs.

[Fundamentals of Cloud Logging](https://www.qwiklabs.com/focuses/10911?catalog_rank=%7B%22rank%22%3A12%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&parent=catalog&search_id=7468061)


#### BigQuery Logging

In this lab you view the BigQuery logs inside Cloud Logging, setup a sink to export them back into BigQuery, and then use SQL to analyze the logs.

[Using BigQuery and Cloud Logging to Analyze BigQuery Usage](https://www.qwiklabs.com/focuses/6100?catalog_rank=%7B%22rank%22%3A15%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&parent=catalog&search_id=7468061)


## Security and Identity


### Introduction

[https://www.youtube.com/watch?v=UOdUC8DhprQ](https://www.youtube.com/watch?v=UOdUC8DhprQ)

[https://www.youtube.com/watch?v=kd33UVZhnAA](https://www.youtube.com/watch?v=kd33UVZhnAA)


#### Authentication Options

[https://cloud.google.com/blog/products/identity-security/identity-and-authentication-the-google-cloud-way](https://cloud.google.com/blog/products/identity-security/identity-and-authentication-the-google-cloud-way)


### IAM

Cloud IAM is Google Cloud Platform’s unified system for managing access to resources and assigning permissions for users and services to access those resources.  This video will take you through the basic terms and concepts you need to use Cloud IAM.

[https://www.youtube.com/watch?v=96HlT4f2AUU](https://www.youtube.com/watch?v=96HlT4f2AUU)

Cloud Identity and Access Management (IAM) lets administrators authorize who can take action on specific resources, giving you full control and visibility to manage Google Cloud resources centrally. For enterprises with complex organizational structures, hundreds of workgroups, and many projects, Cloud IAM provides a unified view into security policy across your entire organization, with built-in auditing to ease compliance processes. Cloud IAM provides a simple and consistent access control interface for all Google Cloud services. Learn one access control interface and apply that knowledge to all Google Cloud resources. Prior to Cloud IAM, you could only grant Owner, Editor, or Viewer roles to users. A wide range of services and resources now surface additional Cloud IAM roles out of the box. For example, the Pub/Sub service exposes Publisher and Subscriber roles in addition to the Owner, Editor, and Viewer roles. Create and manage Cloud IAM policies using the Google Cloud Console, the Cloud IAM methods, and the gcloud command line tool.

[https://cloud.google.com/iam](https://cloud.google.com/iam)


#### Roles

[https://cloud.google.com/iam/docs/understanding-roles](https://cloud.google.com/iam/docs/understanding-roles)


#### Service Accounts

[https://cloud.google.com/iam/docs/service-accounts](https://cloud.google.com/iam/docs/service-accounts)


### Cloud Identity API

Cloud Identity API is an API for provisioning and managing identity resources.

[https://cloud.google.com/identity/docs](https://cloud.google.com/identity/docs)


### Identity-Aware Proxy

Identity-Aware Proxy (IAP) lets you manage access to applications running in the App Engine standard environment, App Engine flexible environment, Compute Engine, and GKE. IAP establishes a central authorization layer for applications accessed by HTTPS, so you can adopt an application-level access control model instead of using network-level firewalls. When you turn on IAP, you must also use [signed headers](https://cloud.google.com/iap/docs/signed-headers-howto) or the App Engine standard environment [Users API](https://cloud.google.com/appengine/docs/standard#users) to secure your app.

[https://cloud.google.com/iap/docs](https://cloud.google.com/iap/docs)

Identity Aware Proxy enables you to configure secure controlled access to your applications so you can enforce "who can see what" access control at the application layer.  You don't need client software, remote access VPNs, firewalls, network configurations. 

[https://www.youtube.com/watch?v=XqMY-rPk3MY](https://www.youtube.com/watch?v=XqMY-rPk3MY)


### Context-Aware Access

Based on the [BeyondCorp](https://cloud.google.com/beyondcorp) security model, Context-Aware Access is an approach that utilizes a variety of Google Cloud offerings to enforce granular access control based on a user's identity and context of the request.

[https://cloud.google.com/context-aware-access/docs/overview](https://cloud.google.com/context-aware-access/docs/overview)

Envisioned in 2011, the BeyondCorp security model leverages identity and context to evaluate trust for access decisions rather than using the corporate network as the perimeter. 

[https://www.youtube.com/watch?v=Sq9gp8KBsY0](https://www.youtube.com/watch?v=Sq9gp8KBsY0)


### Identity Platform

Identity Platform provides back-end services, SDKs, and UI libraries that make it easier to authenticate users to your apps and services.

[https://cloud.google.com/identity-platform/docs](https://cloud.google.com/identity-platform/docs)

Manage the identities of customers, partners, and Things through Identity Platform.

[https://www.youtube.com/watch?v=O_O5Hb1bJyw](https://www.youtube.com/watch?v=O_O5Hb1bJyw)


### Managed Services for Microsoft Active Directory

Managed Service for Microsoft Active Directory is a highly available, hardened Google Cloud service running actual Microsoft AD that enables you to manage your cloud-based AD-dependent workloads, automate AD server maintenance and security configuration, and connect your on-premises AD domain to the cloud.

[https://cloud.google.com/managed-microsoft-ad/docs](https://cloud.google.com/managed-microsoft-ad/docs)


### Resource Manager

Google Cloud provides container resources such as organizations and projects that allow you to group and hierarchically organize other Google Cloud resources. This hierarchical organization helps you manage common aspects of your resources, such as access control and configuration settings. The Resource Manager API enables you to programmatically manage these container resources.

[https://cloud.google.com/ntresource-manager/docs](https://cloud.google.com/resource-manager/docs)

Setting up your Google Cloud Platform resources correctly can save you a lot of trouble down the road. 

[https://www.youtube.com/watch?v=MzclA_hdNLY](https://www.youtube.com/watch?v=MzclA_hdNLY)

Folders are a powerful tool for administering GCP resources in Cloud Resource Manager. Watch this demo video to learn how to get started using folders to help organize and control your cloud resources.

[https://www.youtube.com/watch?v=0oJZhlgDbg8](https://www.youtube.com/watch?v=0oJZhlgDbg8)


### Security Key enforcement

Service to enforce usage of security keys to prevent account takeovers.

[https://vecta.io/symbols/4/google-cloud-platform/44/security-key-enforcement](https://vecta.io/symbols/4/google-cloud-platform/44/security-key-enforcement)

Use 2-Step Verification to protect accounts from unauthorized access. 2-Step Verification puts an extra barrier between your business and cybercriminals who try to steal usernames and passwords to access business data. Turning on 2-Step Verification is the single most important action you can take to protect your business.

[https://support.google.com/cloudidentity/answer/175197/](https://support.google.com/cloudidentity/answer/175197/)

Security in the Cloud vs. on-prem. Sharing responsibility of security in the Cloud.

[https://www.youtube.com/watch?v=wDwQ1YMEyE8](https://www.youtube.com/watch?v=wDwQ1YMEyE8)


### Titan Security Keys

Titan Security Keys are built with a hardware chip that includes firmware engineered by Google to verify the key’s integrity. This helps to ensure that the keys haven’t been physically tampered with.

[https://cloud.google.com/titan-security-key](https://cloud.google.com/titan-security-key)


### Access Transparency

Access Transparency provides you with logs that capture the actions Google personnel take when accessing your content. You might be familiar with [Cloud Audit Logs](https://cloud.google.com/logging/docs/audit), which can help you answer questions about "who did what, where, and when?" in your Google Cloud projects. While Cloud Audit Logs provides these logs about the actions taken by members within your own organization, Access Transparency provides logs of the actions taken by Google personnel.

[https://cloud.google.com/logging/docs/audit/access-transparency-overview](https://cloud.google.com/logging/docs/audit/access-transparency-overview)

[https://www.youtube.com/watch?v=6BCuIBO0Mhg](https://www.youtube.com/watch?v=6BCuIBO0Mhg)


### Binary Authorization

Binary Authorization is a service on Google Cloud that provides software supply-chain security for applications that run in the cloud. Binary Authorization is a service on Google Cloud Platform (GCP) that provides software supply-chain security when deploying container-based applications. Binary Authorization extends Google Kubernetes Engine (GKE) and enforces security policies at deploy time. Binary Authorization works with container images from Container Registry or another container image registry. With Binary Authorization, you can automatically and digitally check each component of your software supply chain, ensuring the quality and integrity of your software before an application is deployed to your production environment.

[https://cloud.google.com/binary-authorization/docs](https://cloud.google.com/binary-authorization/docs)

Check out a demo of Binary Authorization, a Google Cloud Platform security feature. Binary Authorization is a deploy-time security control that ensures only trusted container images are deployed on Kubernetes Engine.

[https://www.youtube.com/watch?v=mi50OJq6wd0](https://www.youtube.com/watch?v=mi50OJq6wd0)


### Cloud Asset Inventory

Cloud Asset Inventory provides inventory services based on a time series database. This database keeps a five-week history of Google Cloud [asset](https://cloud.google.com/asset-inventory/docs/overview#assets) metadata.

[https://cloud.google.com/asset-inventory/docs/overview](https://cloud.google.com/asset-inventory/docs/overview)


### Cloud Data Loss Prevention

Welcome to Cloud Data Loss Prevention (DLP)! Cloud DLP provides access to a powerful sensitive data inspection, classification, and de-identification platform.

[https://cloud.google.com/dlp/docs](https://cloud.google.com/dlp/docs)

Learn how to automatically discover and redact sensitive data everywhere. Try the Data Loss Prevention: Qwik Start lab here:[ http://bit.ly/2QmSZsr](https://www.youtube.com/redirect?event=video_description&v=GArEb2e9jGk&q=http%3A%2F%2Fbit.ly%2F2QmSZsr&redir_token=QUFFLUhqbERxVzNuUE9wY3lHeHJDWGFuZkN4TkExNG9UUXxBQ3Jtc0trbGZ2dW5TYjJYd2FwQmFqZWlIek16QjdScG43R1hXekpkVU9sZTM5dFk1RjNJYkRRaFpEZ3lIdDhuRlVfQVltcVd2MF85aE1YUk9BMzAzOElNSW9qTndXejZURkxiY1hOdXRxTlEwTjJtVlRWTUY4cw%3D%3D)

[https://www.youtube.com/watch?v=GArEb2e9jGk](https://www.youtube.com/watch?v=GArEb2e9jGk)


### Cloud HSM

Cloud HSM is a cloud-hosted Hardware Security Module (HSM) service that allows you to host encryption keys and perform cryptographic operations in a cluster of [FIPS 140-2 Level 3](https://csrc.nist.gov/publications/detail/fips/140/2/final) certified HSMs. Google manages the HSM cluster for you, so you don't need to worry about clustering, scaling, or patching. Because Cloud HSM uses Cloud KMS as its front end, you can leverage all the conveniences and features that Cloud KMS provides.

[https://cloud.google.com/kms/docs/hsm](https://cloud.google.com/kms/docs/hsm)

[https://www.youtube.com/watch?v=DB6UfKFo3ds](https://www.youtube.com/watch?v=DB6UfKFo3ds)


### Security Command Center

Security Command Center is the canonical security and data risk database for Google Cloud. Security Command Center enables you to understand your security and data attack surface by providing asset inventory, discovery, search, and management.

[https://cloud.google.com/security-command-center/docs](https://cloud.google.com/security-command-center/docs)

[https://www.youtube.com/watch?v=k7ZEfAocMq4](https://www.youtube.com/watch?v=k7ZEfAocMq4)


### VPC Service Controls

With VPC Service Controls, administrators can define a security perimeter around resources of Google-managed services to control communication to and between those services.

[https://cloud.google.com/vpc-service-controls/docs](https://cloud.google.com/vpc-service-controls/docs)

VPC Service Controls enables you to establish security perimeters around sensitive data in Google Cloud Platform services such as Google Cloud Storage and BigQuery. 

[https://www.youtube.com/watch?v=EXwJFL24QzY](https://www.youtube.com/watch?v=EXwJFL24QzY)


### Incident Response and Management

The incident response problem space can be divided into three categories: people, process, and data management. Users have long had access to solid people-management solutions (on-call rotation schedulers, etc.) and Google’s SRE book outlines their Incident Management at Google (IMAG) process. In this presentation, attendees will learn the benefits of data management and how Google Cloud Platform (GCP) is providing technology to leverage the idea and accelerate users’ investigations. Attendees will see live demos of Stackdriver Incident Response and Management (IRM) Insights and the supporting GCP technology that makes the innovation possible.

[https://www.youtube.com/watch?v=VXqfbp_zE0c](https://www.youtube.com/watch?v=VXqfbp_zE0c)


### Phishing Protection

Phishing Protection is a phishing countermeasure platform that helps to detect phishing attacks against your users. The Phishing Protection Submission API also enables you to submit URLs suspected to be unsafe to [Safe Browsing](http://safebrowsing.google.com/). Any URLs that are confirmed to match the Safe Browsing Policies will be added to the Safe Browsing list, which is used by over three billion devices to show warnings when a user visits a known unsafe web resource. Common sources of these URLs are customer reports or internal phishing detection results.

[https://cloud.google.com/phishing-protection/docs](https://cloud.google.com/phishing-protection/docs)

A video to show you how security keys prevent phishing attacks by recognizing a domain name and using its hidden private key. 

[https://www.youtube.com/watch?v=c9EOETFnB74](https://www.youtube.com/watch?v=c9EOETFnB74)


### Cloud KMS

A cloud-hosted key management service that lets you manage symmetric and asymmetric cryptographic keys for your cloud services the same way you do on-premises. You can generate, use, rotate, and destroy AES256, RSA 2048, RSA 3072, RSA 4096, EC P256, and EC P384 cryptographic keys. Toggle between software- and hardware-protected encryption keys with the press of a button. Host encryption keys and perform cryptographic operations in FIPS 140-2 Level 3 certified HSMs. With this fully managed service, you can protect your most sensitive workloads without the need to worry about the operational overhead of managing an HSM cluster. Encrypt data in [BigQuery](https://cloud.google.com/bigquery) and [Compute Engine](https://cloud.google.com/compute) with encryption keys that are stored and managed in a third-party key management system that’s deployed outside Google’s infrastructure. External Key Manager allows you to maintain separation between your data at rest and your encryption keys while still leveraging the power of cloud for compute and analytics. Key Access Justifications works with [Cloud EKM](https://cloud.google.com/blog/products/identity-security/cloud-external-key-manager-now-in-beta) to greatly advance the control you have over your data. It’s the only product that gives you visibility into every request for an encryption key, a justification for that request, and a mechanism to approve or deny decryption in the context of that request. 

[https://cloud.google.com/security-key-management](https://cloud.google.com/security-key-management)

Learn about how Google automatically encrypts your data and how to take control of encryption by managing your own keys. 

[https://www.youtube.com/watch?v=38_dWxOHUN8](https://www.youtube.com/watch?v=38_dWxOHUN8)


### reCAPTCHA Enterprise

Google has been defending millions of sites with reCAPTCHA for almost a decade. reCAPTCHA Enterprise is an extension of that effort to help enterprises detect other types of fraudulent activity on their sites, like scraping, credential stuffing, and automated account creation. reCAPTCHA Enterprise offers enhanced detection with more granular scores, reason codes for risky events, and the ability to tune your site-specific model. reCAPTCHA Enterprise is a service that protects your site from spam and abuse. reCAPTCHA Enterprise builds on the existing reCAPTCHA API which uses advanced risk analysis techniques to tell humans and bots apart. reCAPTCHA Enterprise adds enhancements specifically designed to protect enterprise businesses, such as more granular scoring and returning reason codes with low scores to aid in analysis.

[https://cloud.google.com/recaptcha-enterprise/docs](https://cloud.google.com/recaptcha-enterprise/docs)

See how reCAPTCHA Enterprise can help protect your websites from fraud and abuse.

[https://www.youtube.com/watch?v=ic3Fj2B1LR4](https://www.youtube.com/watch?v=ic3Fj2B1LR4)


### Web Risk

Web Risk is a new enterprise security product that lets your client applications check URLs against Google's constantly updated lists of unsafe web resources.

[https://cloud.google.com/web-risk/docs](https://cloud.google.com/web-risk/docs)


### Identity & Security Topics

[https://cloud.google.com/blog/products/identity-security](https://cloud.google.com/blog/products/identity-security)


### Data Governance 


#### BigQuery Column-level security

[https://cloud.google.com/blog/products/data-analytics/data-governance-new-ways-to-securely-access-and-discover-data](https://cloud.google.com/blog/products/data-analytics/data-governance-new-ways-to-securely-access-and-discover-data)


### Qwiklabs


#### Cloud KMS

In this lab you'll learn how to use some advanced features of Google Cloud Security and Privacy APIs, including:



*   Setting up a secure Cloud Storage bucket
*   Managing keys and encrypted data using Key Management Storage
*   Viewing Cloud Storage audit logs

You'll take abridged data from the Enron Corpus, encrypt it and load it into Cloud Storage.

[Getting Started with Cloud KMS](https://www.qwiklabs.com/focuses/1713?catalog_rank=%7B%22rank%22%3A20%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&parent=catalog&search_id=7468061)


#### Security & Identity

Security is an uncompromising feature of Google Cloud services, and Google Cloud has developed specific tools for ensuring safety and identity across your projects. In this fundamental-level quest, you will get hands-on practice with Google Cloud’s Identity and Access Management (IAM) service, which is the go-to for managing user and virtual machine accounts.

[Security & Identity Fundamentals](https://www.qwiklabs.com/quests/40?catalog_rank=%7B%22rank%22%3A1%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&search_id=7482841)


#### IAM

In this fundamental-level quest, you will get hands-on practice with Google Cloud’s Identity and Access Management (IAM) service, which is the go-to for managing user and virtual machine accounts. You will get experience with network security by provisioning VPCs and VPNs, and learn what tools are available for security threat and data loss protections.

[Ensure Access & Identity in Google Cloud](https://www.qwiklabs.com/quests/150?catalog_rank=%7B%22rank%22%3A3%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&search_id=7482841)


## Infrastructure as Code


### Introduction

Provisioning compute resources has traditionally been hard to manage, not scalable, and prone to error, so what other techniques can you use to make sure you’re ready to meet demand? In this episode of Season of Scale, Stephanie Wong explains why you should adopt an Infrastructure as code (IaC) strategy, so you can automate the creation of your cloud resources, create templates, and store config files with the help of tools like Google Cloud Deployment Manager.

[https://cloud.google.com/solutions/infrastructure-as-code](https://cloud.google.com/solutions/infrastructure-as-code)


#### Google Cloud Deployment Manager

[https://www.youtube.com/watch?v=z-caqPtEw58](https://www.youtube.com/watch?v=z-caqPtEw58)


##### Cloud Deployment Quickstart

[https://cloud.google.com/deployment-manager/docs/quickstart](https://cloud.google.com/deployment-manager/docs/quickstart)


##### Deployments

[https://cloud.google.com/deployment-manager/docs/deployments](https://cloud.google.com/deployment-manager/docs/deployments)


##### Manifests

[https://cloud.google.com/deployment-manager/docs/deployments/viewing-manifest](https://cloud.google.com/deployment-manager/docs/deployments/viewing-manifest)


##### Cloud Deployment Manager Deploying Network Load Balanced Logbook 

[https://cloud.google.com/deployment-manager/docs/create-advanced-deployment](https://cloud.google.com/deployment-manager/docs/create-advanced-deployment)


##### Shard VPC with Cloud Deployment Manager

[https://cloud.google.com/solutions/shared-vpc-with-deployment-manager](https://cloud.google.com/solutions/shared-vpc-with-deployment-manager)


##### Solutions that use Cloud Deployment Manager

[https://cloud.google.com/docs/tutorials?sortBy=relevance#%22deployment%20manager%22](https://cloud.google.com/docs/tutorials?sortBy=relevance#%22deployment%20manager%22)


##### More examples

[https://github.com/GoogleCloudPlatform/deploymentmanager-samples/tree/master/examples/v2](https://github.com/GoogleCloudPlatform/deploymentmanager-samples/tree/master/examples/v2)


#### Cloud Foundation Toolkit

[https://cloud.google.com/foundation-toolkit/](https://cloud.google.com/foundation-toolkit/)


### Terraform 


#### Introduction

Terraform's infrastructure-as-code (IaC) approach supports [DevOps](https://cloud.google.com/devops) best practices for change management, letting you manage Terraform configuration files in source control to maintain an ideal provisioning state for testing and production environments.

[https://cloud.google.com/docs/terraform](https://cloud.google.com/docs/terraform)

Terraform is a tool from Hashicorp for building, changing, and versioning infrastructure safely and efficiently. Terraform can manage existing and popular service providers as well as custom in-house solutions.

[https://www.terraform.io/intro/index.html](https://www.terraform.io/intro/index.html)


#### Getting Started on GCP

[https://cloud.google.com/community/tutorials/getting-started-on-gcp-with-terraform](https://cloud.google.com/community/tutorials/getting-started-on-gcp-with-terraform)

Defining and managing your development, test, staging, and production environments using infra-as-code tools such as [Deployment Manager](https://cloud.google.com/deployment-manager) or [Terraform](https://www.terraform.io/) is a common practice. Ensuring that any changes you make to your environment config definitions are “safe” remains challenging, though.

[https://www.youtube.com/watch?v=3vfXQxWJazM](https://www.youtube.com/watch?v=3vfXQxWJazM)


##### Managing infrastructure as code with Terraform, Cloud Build, and GitOps

[https://cloud.google.com/solutions/managing-infrastructure-as-code](https://cloud.google.com/solutions/managing-infrastructure-as-code)


##### Hashicorp tutorials

[https://learn.hashicorp.com/collections/terraform/gcp-get-started#gcp](https://learn.hashicorp.com/collections/terraform/gcp-get-started#gcp)


##### Terraform Modules for GCP

[https://github.com/terraform-google-modules](https://github.com/terraform-google-modules)


##### Examples

[https://github.com/terraform-google-modules/docs-examples](https://github.com/terraform-google-modules/docs-examples)


#### Terraformer

Reverse of terraform.  

[https://github.com/GoogleCloudPlatform/terraformer](https://github.com/GoogleCloudPlatform/terraformer)


#### A list of URLs related to terraform

[https://github.com/shuaibiyy/awesome-terraform](https://github.com/shuaibiyy/awesome-terraform)


### Pulumi

[https://www.pulumi.com/docs/get-started/gcp/](https://www.pulumi.com/docs/get-started/gcp/)


### Ansible

An opinionated look at how ansible and terraform complement one another in a provisioner/configuration management separated view. A key takeaway is a simplified workflow for sysadmins/operators in cloud management that can be applied in multi-cloud/hybrid cloud scenarios.

[https://www.youtube.com/watch?v=utztQWTewWU](https://www.youtube.com/watch?v=utztQWTewWU)


### Qwiklabs


#### Terraform Quest

[https://www.qwiklabs.com/quests/44](https://www.qwiklabs.com/quests/44)


#### Terraform

In this Quest, the experienced user of Google Cloud will learn how to describe and launch cloud resources with Terraform, an open source tool that codifies APIs into declarative configuration files that can be shared amongst team members, treated as code, edited, reviewed, and versioned. In these nine hands-on labs, you will work with example templates and understand how to launch a range of configurations, from simple servers, through full load-balanced applications.

[Managing Cloud Infrastructure with Terraform](https://www.qwiklabs.com/quests/44?catalog_rank=%7B%22rank%22%3A1%2C%22num_filters%22%3A1%2C%22has_search%22%3Atrue%7D&search_id=7467726)


#### VM Migration

Google Cloud’s four step structured Cloud Migration Path Methodology provides a defined and repeatable path for users to follow when migrating and modernizing Virtual Machines. In this quest, you will get hands-on practice with Google’s current solution set for VM assessment, planning, migration, and modernization. You will start by analyzing your lab environment and building assessment reports with CloudPhysics and StratoZone, then build a landing zone within Google Cloud leveraging Terraform’s infrastructure-as-code templates, next you will manually transform a two-tier application into a cloud-native workload running on Kubernetes, and finally, transform a VM workload into Kubernetes with Migrate for Anthos and migrate a VM between cloud environments.

[VM Migration](https://www.qwiklabs.com/quests/87?catalog_rank=%7B%22rank%22%3A2%2C%22num_filters%22%3A1%2C%22has_search%22%3Atrue%7D&search_id=7467726)


## Google Maps Platform


### Introduction

Google Maps Platform includes Maps SDKs for Android and iOS, Maps Static API,

Maps JavaScript API, Street View Static API, Maps URLs and Maps Embed API. Routes APIs support Directions API, Distance Matrix API and Roads API.  Places SDK for Android and iOS add rich details for places. Places Library, Maps JavaScript API, Places API, Geocoding API, Geolocation API and Time Zone API provide rich location and time zone data.

[https://developers.google.com/maps/documentation/](https://developers.google.com/maps/documentation/)


### Solving business problems with Google Maps API

[https://www.youtube.com/watch?v=UzMEtXsMM08](https://www.youtube.com/watch?v=UzMEtXsMM08)


### Qwiklabs


#### Google Maps

In this quest you will use several tools available in Google Cloud to manipulate data and create a Google Map - map location details to find subway stations or a business; use geocoding and Apps Script to send an email of a map; visualize data on a customized map; and build a server-side proxy to create a map on a mobile device.

[Creating with Google Maps](https://www.qwiklabs.com/quests/103?catalog_rank=%7B%22rank%22%3A9%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&search_id=7467888)


## Google Workspace

AKA G-Suite


### Introduction

Similar to G Suite, all Google Workspace plans provide a custom email for your business and includes collaboration tools like Gmail, Calendar, Meet, Chat, Drive, Docs, Sheets, Slides, Forms, Sites, and more. 

[https://workspace.google.com/](https://workspace.google.com/)


### YouTube channel for Google Workspace

[https://www.youtube.com/channel/UCBmwzQnSoj9b6HzNmFrg_yw](https://www.youtube.com/channel/UCBmwzQnSoj9b6HzNmFrg_yw)


### Google Workspace Learning Center

[https://support.google.com/a/users#!/&topic=9296556](https://support.google.com/a/users#!/&topic=9296556)


### G Suite tutorial for beginners

[https://www.youtube.com/watch?v=wJ3S7kFFypU](https://www.youtube.com/watch?v=wJ3S7kFFypU)


### Introduction to G Suite Development tools

[https://www.youtube.com/watch?v=NqumcYgj5LI](https://www.youtube.com/watch?v=NqumcYgj5LI)


### G Suite REST APIs

[https://www.youtube.com/watch?v=ftxroBc7mi4](https://www.youtube.com/watch?v=ftxroBc7mi4)


### Qwiklabs


#### Essentials

G Suite is Google's Collaborative Applications platform, delivered from Google Cloud. In this introductory-level quest, you will get hands-on practice with G Suite’s core applications from a user perspective. Although there are many more applications and tool components to G Suite than are covered here, you will get experience with the primary apps: Gmail, Calendar, Sheets and a handful of others.

[G Suite Essentials](https://www.qwiklabs.com/quests/65?catalog_rank=%7B%22rank%22%3A1%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&search_id=7482904)


#### Integrations

This Quest of hands-on labs demonstrates the power of integrating Google Cloud services and tools with G Suite applications. With integration technologies like the Clasp Command Line environment, you will create and publish web apps and add-ons for G Suite products: Sheets, Docs, Forms, and Slides. In other labs you'll create direct connections to Google Cloud data sources using the BigQuery API, Sheets, and Slides to collect, analyze and present data.

[G Suite: Integrations](https://www.qwiklabs.com/quests/51?catalog_rank=%7B%22rank%22%3A2%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&search_id=7482904)


#### Certification Practice Lab

This practice lab helps you become familiar with the structure and types of questions used in the G Suite certification exam. The lab is helpful to anyone who is planning to take the exam.

[G Suite Certification: Practice Lab](https://www.qwiklabs.com/focuses/4051?catalog_rank=%7B%22rank%22%3A5%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&parent=catalog&search_id=7482904)


#### Gmail

Gmail is an email service developed by Google. Gmail stores your email safely in the cloud, allowing you to access it from any computer or device with a web browser. You can also quickly organize and find important email, as well as read and draft email without an internet connection.

[Gmail: Getting Started](https://www.qwiklabs.com/focuses/5825?catalog_rank=%7B%22rank%22%3A13%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&parent=catalog&search_id=7482915)


#### Shared Drives

Shared drives is a shared space where teams can easily store, search, and access their files anywhere, from any device. In Shared drive, files belong to the team. If members leave, the files stay exactly where they are so your team can continue to share information and get work done. In this lab you set up and use Shared drive.

[Shared Drives: Getting Started](https://www.qwiklabs.com/focuses/5829?catalog_rank=%7B%22rank%22%3A14%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&parent=catalog&search_id=7482915)


#### Meet

[Google Meet](https://apps.google.com/meet/) is a video conferencing application that lets you hold impromptu video meetings on the go, virtual training classes around the world, remote interviews, and much more. 

[Google Meet: Getting Started](https://www.qwiklabs.com/focuses/5831?catalog_rank=%7B%22rank%22%3A15%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&parent=catalog&search_id=7482915)


#### Google Drive

With Google Drive, you can store all your files in the cloud, including photos, Microsoft® Word® documents, Excel® spreadsheets, and more. You can also make changes to a Word file using Google Docs, or convert your Word files to Google Docs, Sheets, or Slides.

[Google Drive: Getting Started](https://www.qwiklabs.com/focuses/5827?catalog_rank=%7B%22rank%22%3A16%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&parent=catalog&search_id=7482915)


#### Sites

Google Sites is a website building platform for businesses and business teams. With Google Sites, you drag and drop content to easily build internal project hubs, team sites, public-facing websites, and more—all without designer, programmer, or IT help. In this lab, you explore how to use Google Sites to build and manage a website. You then share the site with people in your organization to collaborate on the content.

[Google Sites: Getting Started](https://www.qwiklabs.com/focuses/5830?catalog_rank=%7B%22rank%22%3A17%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&parent=catalog&search_id=7482915)


#### Sheets

Google Sheets is a cloud-based application that provides advanced, fast, online spreadsheets. Designed with collaboration and convenience in mind, you can analyze data with charts and filters, handle task lists, create project plans, and more with your team from any online device. All changes are saved automatically and in one place. Use Google Sheets to create, edit, and collaborate wherever you are.

[Google Sheets: Getting Started](https://www.qwiklabs.com/focuses/5828?catalog_rank=%7B%22rank%22%3A11%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&parent=catalog&search_id=7482915)


#### Calendar

Google Calendar is an online, integrated calendar designed for teams. You can quickly schedule meetings and events and get reminders about upcoming activities, so you always know what’s next. It’s easy to share your schedule with others and create multiple calendars that you and your team can use together.

[Google Calendar: Getting Started](https://www.qwiklabs.com/focuses/5826?catalog_rank=%7B%22rank%22%3A12%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&parent=catalog&search_id=7482915)

G Suite by Google Cloud is your go-to solution for productivity tools. Get more done with seamless collaboration tools, a simple management interface, and enterprise-level security and reliability. Easily add users, manage devices and configure security and settings so your data stays safe.


#### G Suite Administration

[G Suite Admin Getting Started - Personalization](https://www.qwiklabs.com/focuses/1724?catalog_rank=%7B%22rank%22%3A7%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&parent=catalog&search_id=7482904)


#### Hangouts Chat Bot

Hangouts Chat bots provide easy-to-use access points to your organization's data and services. Users can interact with bots conversationally within a chat experience.

[Hangouts Chat bot - Apps Script](https://www.qwiklabs.com/focuses/2165?catalog_rank=%7B%22rank%22%3A8%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&parent=catalog&search_id=7482904)


#### Big Data Analysis

This lab covers Google Cloud's [BigQuery](http://cloud.google.com/bigquery) API (as an Apps Script [advanced service](https://developers.google.com/apps-script/guides/services/advanced)) and the [built-in Apps Script services](https://developers.google.com/apps-script/guides/services) for [Google Sheets](http://gsuite.google.com/products/sheets) and [Google Slides](http://gsuite.google.com/products/slides).

[Big Data Analysis to a Slide Presentation](https://www.qwiklabs.com/focuses/3565?catalog_rank=%7B%22rank%22%3A9%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&parent=catalog&search_id=7482904)


#### Google Cloud Functions

In this lab, you build and deploy a few Cloud Functions connected to G Suite APIs and other Google Cloud Platform services.

[Empower Your Gmail Inbox with Google Cloud Functions](https://www.qwiklabs.com/focuses/5166?catalog_rank=%7B%22rank%22%3A10%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&parent=catalog&search_id=7482904)


## AppSheet


### Introduction

AppSheet Automation allows line-of-business employees to rapidly automate their critical business processes. The AI-powered solution anticipates your automation requirements, provides intelligent suggestions, and auto-constructs actions based on user intent.

[https://cloud.google.com/appsheet](https://cloud.google.com/appsheet)


### How to create a no-code App

[https://solutions.appsheet.com/how-to-create-an-app](https://solutions.appsheet.com/how-to-create-an-app)


### Sample Apps

[https://www.appsheet.com/SampleApps](https://www.appsheet.com/SampleApps)


### YouTube AppSheet Playlist

[https://www.youtube.com/watch?v=7Tzwu8mY-gI&list=PLZ81nepkT97KAehtQ_Y__bNJX3qZaStvt](https://www.youtube.com/watch?v=7Tzwu8mY-gI&list=PLZ81nepkT97KAehtQ_Y__bNJX3qZaStvt)


## Healthcare and Life Sciences


### Cloud Healthcare API

The Cloud Healthcare API provides industry-standard protocols and formats for ingesting, storing, analyzing, and integrating healthcare data with cloud-based applications.

The API supports the following applications:



*   Healthcare machine learning applications
*   Data-level integration of healthcare systems
*   Secure storage and retrieval of healthcare and life science data, including electronic protected health information (ePHI) and other forms of PII

For many applications, the Cloud Healthcare API can provide a cloud-based alternative to on-premises stacks implementing the following standards:



*   Digital Imaging and Communications in Medicine (DICOM)
*   Fast Healthcare Interoperability Resources (FHIR) DSTU2, STU3, and R4 standards
*   Health Level Seven Version 2.x (HL7v2)

The Cloud Healthcare API simplifies data integration with existing systems and allows developers to focus on differentiating features, such as UX and intelligence.

[https://cloud.google.com/healthcare/docs](https://cloud.google.com/healthcare/docs)

There is no shortage of opportunities for clinical decision support and cognitive assistance in healthcare. 

[https://www.youtube.com/watch?v=DH-JC9DfYdI](https://www.youtube.com/watch?v=DH-JC9DfYdI)


### Cloud Life Sciences

Cloud Life Sciences is a suite of services and tools for managing, processing, and transforming life sciences data. It also enables advanced insights and operational workflows using highly scalable and compliant infrastructure. Cloud Life Sciences includes features such as the Cloud Life Sciences API and extract-transform-load (ETL) tools, and more.

[https://cloud.google.com/life-sciences/docs](https://cloud.google.com/life-sciences/docs)


### Qwiklabs


#### ML Predictions

In this lab, you will create a prediction pipeline for FHIR resources using Cloud Healthcare API and AI Platform.

[Machine Learning Predictions with FHIR and Healthcare API](https://www.qwiklabs.com/focuses/6129?catalog_rank=%7B%22rank%22%3A18%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&parent=catalog&search_id=7468017)


## IoT


### Introduction

Learn how to create a Cloud IoT Core device registry and register a device. Try the Internet of Things: Qwik Start lab here:[ https://goo.gl/Wzgvaq](https://www.youtube.com/redirect?q=https%3A%2F%2Fgoo.gl%2FWzgvaq&redir_token=QUFFLUhqbU40UE5wbXFUUEtiSDRHT2hfY1dWbXIwdENXd3xBQ3Jtc0tueTJmREotMno2SHdtSi1xUVRJVGliZ21XNFRzd3VDWXppTWxxT1ZIcS0zc2NoZnBBZzJKWkx0akZybDRHTlg4cWF3T1RlWWN1OGQ5WWEtdVhCdjRVZ2FfME4zdXQ5ZFF0QnhHY0o3a2xfdmF6NUVwRQ%3D%3D&v=iRZzqpvARbc&event=video_description)

[https://www.youtube.com/watch?v=iRZzqpvARbc](https://www.youtube.com/watch?v=iRZzqpvARbc)


### IoT Core

Google Cloud Internet of Things (IoT) Core is a fully managed service for securely connecting and managing IoT devices, from a few to millions. Ingest data from connected devices and build rich applications that integrate with the other big data services of Google Cloud Platform.

[https://cloud.google.com/iot/docs](https://cloud.google.com/iot/docs)

Events of interest fire off continuously in the physical world, and data that is material to decision making can’t always wait for offline analysis. Internet-equipped sensors on any physical item imaginable make it possible to ingest data continuously into the cloud, directly from the source at massive scale. Learn why Cloud Platform is the best place to build IoT initiatives, taking advantage of Google’s heritage of web-scale processing, analytics, and machine intelligence.

[https://www.youtube.com/watch?v=51bq_Yhuof4](https://www.youtube.com/watch?v=51bq_Yhuof4)


### Qwiklabs


#### IoT in GCP

In this quest, you will learn about Google Cloud’s IoT Core service and its integration with other services like GCS, Dataprep, Stackdriver and Firestore. The labs in this quest use simulator code to mimic IOT devices and the learning here should empower you to implement the same streaming pipeline with real world IoT devices.

[IoT in the Google Cloud](https://www.qwiklabs.com/quests/49?catalog_rank=%7B%22rank%22%3A1%2C%22num_filters%22%3A1%2C%22has_search%22%3Atrue%7D&search_id=7467733)


#### Cloud Logging IoT

In this hands-on lab you will learn how to configure Cloud Functions to send IoT Core device application logs to Cloud Logging.

[Using Cloud Logging with IoT Core Devices](https://www.qwiklabs.com/focuses/2768?catalog_rank=%7B%22rank%22%3A18%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&parent=catalog&search_id=7468061)


## DevOps


### Introduction

Obtain a [competitive advantage](https://hbr.org/sponsored/2019/01/competitive-advantage-through-devops) through DevOps. [DevOps](https://cloud.google.com/devops/) is an organizational and cultural movement that aims to increase software delivery velocity, improve service reliability, and build shared ownership among software stakeholders. In this quest you will learn how to use Google Cloud to improve the speed, stability, availability, and security of your software delivery capability. [DevOps Research and Assessment](https://devops-research.com/) has joined Google Cloud. How does your team measure up? [Take this five multiple-choice question quiz](https://beta.devops-research.com/quickcheck.html) and find out! 

[DevOps Essentials](https://www.qwiklabs.com/quests/96?catalog_rank=%7B%22rank%22%3A3%2C%22num_filters%22%3A1%2C%22has_search%22%3Atrue%7D&search_id=7467726)


### Jenkins & GKE

Jenkins is one of the most popular CI systems in the world. It’s flexibility and ecosystem allow it to be used for almost any task.

[https://www.youtube.com/watch?v=IDoRWieTcMc](https://www.youtube.com/watch?v=IDoRWieTcMc)


### Spinnaker

Build a container based CI/CD pipeline leveraging Google Cloud Platform  tools along with open source tool Spinnaker for deployment. 

[https://www.youtube.com/watch?v=DQIu373gSKU](https://www.youtube.com/watch?v=DQIu373gSKU)


### Jib

Build optimized containers for your Java applications.

[https://www.youtube.com/watch?v=p36tv1YWIfU](https://www.youtube.com/watch?v=p36tv1YWIfU)


### Kubernetes CI/CD

This session demonstrates how using the best tools in the Kubernetes ecosystem, such as Jenkins X, Tekton, Docker, Helm, Skaffold, ChartMuseum, Knative, Prow and others can help you create a fully automated setup. 

[https://www.youtube.com/watch?v=jXPn36d5Tog](https://www.youtube.com/watch?v=jXPn36d5Tog)

Kubernetes had become the orchestrator of choice to deploy applications — but what about a developer’s day to day job? Building Kubernetes applications can require spending a lot of time on building containers, deploying them, and waiting to see changes. Developing applications on Kubernetes doesn’t have to be difficult, and this talk will show you how to leverage local development tools like Skaffold and Google Cloud Build to develop at 10x velocity. We’ll cover how Skaffold intelligently rebuilds and redeploys your application on every code change, all from the comfort of your favorite IDE. We’ll then go over how to use Skaffold and Google Cloud Build to easily deploy a robust CI/CD pipeline from GitHub to GKE, simplifying your local development experience from start to finish.

[https://www.youtube.com/watch?v=TYx0BTyFtmc](https://www.youtube.com/watch?v=TYx0BTyFtmc)


#### Security


##### StackRox

[https://www.stackrox.com/post/2020/11/stackrox-integrates-with-google-artifact-registry/](https://www.stackrox.com/post/2020/11/stackrox-integrates-with-google-artifact-registry/)


##### Binary Authorization Attestations with Voucher

[https://cloud.google.com/binary-authorization/docs/creating-attestations-voucher](https://cloud.google.com/binary-authorization/docs/creating-attestations-voucher)


### GitOps 

GitOps is a way to do application delivery. It works by using [Git](https://git-scm.com/) as a single source of truth for [declarative infrastructure and applications](https://en.wikipedia.org/wiki/Infrastructure_as_code), together with tools ensuring the _actual state_ of infrastructure and applications converges towards the _desired state_ declared in Git. With Git at the center of your delivery pipelines, developers can make pull requests to accelerate and simplify application deployments and operations tasks to your infrastructure or container-orchestration system (e.g. [Kubernetes](https://kubernetes.io/)).

[https://github.com/weaveworks/awesome-gitops](https://github.com/weaveworks/awesome-gitops)


#### Tutorial

This tutorial explains how to manage infrastructure as code with [Terraform](https://cloud.google.com/docs/terraform) and [Cloud Build](https://cloud.google.com/cloud-build) using the popular [GitOps](https://thenewstack.io/what-is-gitops-and-why-it-might-be-the-next-big-thing-for-devops/) methodology. The term GitOps was [first coined by Weaveworks](https://www.weave.works/blog/gitops-operations-by-pull-request), and its key concept is using a Git repository to store the environment state that you want. Terraform is a [HashiCorp](https://www.hashicorp.com/) open source tool that enables you to predictably create, change, and improve your cloud infrastructure by using code. In this tutorial, you use [Cloud Build](https://cloud.google.com/cloud-build), a Google Cloud continuous integration service, to automatically apply Terraform manifests to your environment.

[https://cloud.google.com/solutions/managing-infrastructure-as-code](https://cloud.google.com/solutions/managing-infrastructure-as-code)


#### Gitlab Gitops with Anthos

[https://www.youtube.com/watch?v=npc08ggdTOw](https://www.youtube.com/watch?v=npc08ggdTOw)


### ArgoCD

[https://www.youtube.com/watch?v=35Qimb_AZ8U](https://www.youtube.com/watch?v=35Qimb_AZ8U)


### Chaos Monkey

[https://netflix.github.io/chaosmonkey/](https://netflix.github.io/chaosmonkey/)


## Development, API & SDK


### Introduction

Google Cloud Application Programming Interfaces are the mechanism to interact with Google Cloud Services programmatically. 


### Cloud Endpoints

Endpoints is an API management system that helps you secure, monitor, analyze, and set quotas on your APIs using the same infrastructure Google uses for its own APIs. After you deploy your API to Endpoints, you can use the [Cloud Endpoints Portal](https://cloud.google.com/endpoints/docs/dev-portal-overview) to create a developer portal, a website that users of your API can access to view documentation and interact with your API.

[https://cloud.google.com/endpoints/docs](https://cloud.google.com/endpoints/docs)

Use Cloud Endpoints to deploy, test and  manage your API’s.

[https://www.youtube.com/watch?v=AgYImGHmvBA](https://www.youtube.com/watch?v=AgYImGHmvBA)


### Cloud API

Google Cloud APIs are a key part of Google Cloud Platform, allowing you to easily add the power of everything from storage access to machine-learning-based image analysis to your Cloud Platform applications.

[https://cloud.google.com/apis/docs/overview](https://cloud.google.com/apis/docs/overview)


### Artifact Registry

A universal package manager for all your build artifacts and dependencies. Fast, scalable, reliable and secure.

[https://cloud.google.com/artifacts/docs](https://cloud.google.com/artifacts/docs)

Container Registry has evolved into Artifact Registry - a platform that allows you to seamlessly manage container images, integrate with Cloud Build and third-party CI/CD systems. 

[https://www.youtube.com/watch?v=712Y0KpeHok](https://www.youtube.com/watch?v=712Y0KpeHok)


### Container Registry

Container Registry provides secure, private Docker image storage on Google Cloud Platform.

[https://cloud.google.com/container-registry/docs](https://cloud.google.com/container-registry/docs)


### Cloud Source Repositories

Cloud Source Repositories are fully featured, private [Git](https://git-scm.com/) repositories hosted on Google Cloud.

[https://cloud.google.com/source-repositories/docs](https://cloud.google.com/source-repositories/docs)


### Cloud Deployment Manager


#### Introduction

Google Cloud Deployment Manager is an infrastructure deployment service that automates the creation and management of Google Cloud resources. Write flexible template and configuration files and use them to create deployments that have a variety of Google Cloud services, such as Cloud Storage, Compute Engine, and Cloud SQL, configured to work together.

[https://cloud.google.com/deployment-manager/docs](https://cloud.google.com/deployment-manager/docs)


#### Tutorial

In this tutorial, you deploy an example logbook app that uses Node.js for its frontend and MySQL for its backend. 

[https://cloud.google.com/deployment-manager/docs/create-advanced-deployment](https://cloud.google.com/deployment-manager/docs/create-advanced-deployment)


### Codelabs

Google Developers Codelabs provide a guided, tutorial, hands-on coding experience. Most codelabs will step you through the process of building a small application, or adding a new feature to an existing application. They cover a wide range of topics such as Android Wear, Google Compute Engine, Project Tango, and Google APIs on iOS.

[https://codelabs.developers.google.com/](https://codelabs.developers.google.com/)


### Colab

Colaboratory, or "Colab" for short, allows you to write and execute Python in your browser.

Colab allows you to not only execute Jupyter Notebooks on the web, but also offers a free GPU, excellent collaboration features, built-in code snippets, and more.

[https://colab.research.google.com/](https://colab.research.google.com/)

A demo of Colab.

[https://www.youtube.com/watch?v=yEIc9z-Ad3k](https://www.youtube.com/watch?v=yEIc9z-Ad3k)


### Cloud Scheduler

Cloud Scheduler is a fully managed enterprise-grade cron job scheduler. It allows you to schedule virtually any job, including batch, big data jobs, cloud infrastructure operations, and more. You can automate everything, including retries in case of failure to reduce manual toil and intervention. Cloud Scheduler even acts as a single pane of glass, allowing you to manage all your automation tasks from one place.

[https://cloud.google.com/scheduler/docs/quickstart](https://cloud.google.com/scheduler/docs/quickstart)

Use Cloud Scheduler to run python scripts in the cloud periodically like cron jobs.

[https://www.youtube.com/watch?v=7Z1mgOxWTs8](https://www.youtube.com/watch?v=7Z1mgOxWTs8)


### Cloud Tasks

Cloud Tasks is a fully managed service that allows you to manage the execution, dispatch and delivery of a large number of distributed tasks. You can asynchronously perform work outside of a user request. Your tasks can be executed on App Engine or any arbitrary HTTP endpoint.

[https://cloud.google.com/tasks/docs](https://cloud.google.com/tasks/docs)

Understanding Cloud Tasks for Async Tasks.

Queues for background tasks.

[https://www.youtube.com/watch?v=Q_airdHCuV8](https://www.youtube.com/watch?v=Q_airdHCuV8)


### Cloud Code

Cloud Code provides IDE support for the full development cycle of Kubernetes and Cloud Run applications, from creating and customizing a new application from sample templates to running your finished application. Cloud Code also supports you along the way with run-ready samples, out-of-the-box configuration snippets, and a tailored debugging experience — making developing with Kubernetes and Cloud Run a whole lot easier!

[https://cloud.google.com/code/docs](https://cloud.google.com/code/docs)

Cloud Code provides an end-to-end workflow for developing, debugging, and deploying Cloud Run applications from within IDEs such as Visual Studio Code and IntelliJ. 

[https://www.youtube.com/watch?v=bOWsRGGO5xk](https://www.youtube.com/watch?v=bOWsRGGO5xk)

Using Cloud Code with Kubernetes.

[https://www.youtube.com/watch?v=KNd0mTxcQ_M](https://www.youtube.com/watch?v=KNd0mTxcQ_M)


### Cloud Build

Cloud Build is a service that executes your builds on Google Cloud Platform infrastructure. Cloud Build can import source code from Google Cloud Storage, Cloud Source Repositories, GitHub, or Bitbucket, execute a build to your specifications, and produce artifacts such as Docker containers or Java archives.

[https://cloud.google.com/cloud-build/docs](https://cloud.google.com/cloud-build/docs)

Google Cloud Build helps you create fast, consistent, and reliable workflows. 

[https://www.youtube.com/watch?v=w7dMHiEyGAs](https://www.youtube.com/watch?v=w7dMHiEyGAs)

A list of URLs related to Cloud Build.

[https://github.com/Timtech4u/awesome-cloudbuild](https://github.com/Timtech4u/awesome-cloudbuild)


### Qwiklabs


#### Exploring APIs

This quest will give you hands-on practice with a variety of GCP APIs, which you will learn through working with Google’s APIs Explorer, a tool that allows you to browse APIs and run their methods interactively. By learning how to transfer data between Cloud Storage buckets, deploy Compute Engine instances, configure Dataproc clusters and much more, Exploring APIs will show you how powerful APIs are and why they are used almost exclusively by proficient GCP users. Enroll in this quest today.

[Exploring APIs](https://www.qwiklabs.com/quests/54?catalog_rank=%7B%22rank%22%3A10%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&search_id=7467936)


#### App Engine API Explorer

[App Engine](https://cloud.google.com/appengine/) lets you deploy applications on a fully managed platform. You can scale your applications seamlessly without having to worry about managing the underlying infrastructure. With zero server management and zero configuration deployments, developers can focus only on building great applications without the management overhead.

In this lab you will deploy a simple hello world application to App Engine and make updates to its configuration using the App Engine Admin API through the APIs Explorer tool.

[APIs Explorer: App Engine](https://www.qwiklabs.com/focuses/3662?catalog_rank=%7B%22rank%22%3A16%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&parent=catalog&search_id=7467964)


## API Management, Apigee

Apigee is a Full-LifeCycle API Management tool.

[https://www.youtube.com/watch?v=-okdOGsitm8](https://www.youtube.com/watch?v=-okdOGsitm8)


### Apigee API Platform

With Apigee, you can build API proxies—RESTful, HTTP-based APIs that interact with your services. With easy-to-use APIs, developers can be more productive, increasing your speed to market.

[https://docs.apigee.com/](https://docs.apigee.com/)


### Apigee Developer Portal

Using the Drupal portal development tools, you can build a fully customizable developer portal. Drupal provides a rich set of functionality and all the CMS capabilities of Drupal with additional Apigee-developed Drupal modules. However, implementing a Drupal-based portal requires more time and effort.

[https://docs.apigee.com/api-platform/publish/developer-portal#integrated-portal](https://docs.apigee.com/api-platform/publish/developer-portal#integrated-portal)


### Apigee Sense

Apigee Sense protects your APIs from unwanted request traffic, including attacks from malicious clients. Apigee Sense analyzes API request traffic, identifying patterns that might represent unwanted requests.

[https://docs.apigee.com/sense/what-apigee-sense](https://docs.apigee.com/sense/what-apigee-sense)


### Apigee API Analytics

Edge API Analytics collects and calculates a wealth of information that flows through API proxies. You can visualize this data with graphs and charts in the Edge UI, or you can download the raw data for offline analysis using the Edge management APIs.

[https://docs.apigee.com/api-platform/analytics/analytics-services-overview](https://docs.apigee.com/api-platform/analytics/analytics-services-overview)


### Apigee API Monetization

As an API provider, you need an easy-to-use and flexible way to monetize your APIs so that you can generate revenue for the use of your APIs. Using monetization in Apigee Edge, you can create a variety of monetization plans that charge developers (or pay them through revenue sharing) for the use of your APIs.

[https://docs.apigee.com/api-platform/monetization/basics-monetization/](https://docs.apigee.com/api-platform/monetization/basics-monetization/)


### Apigee Hybrid

Apigee hybrid is a platform for developing and managing API proxies that features a hybrid deployment model. The hybrid model includes a management plane hosted by Apigee in the Cloud and a runtime plane that you install and manage on one of the [supported Kubernetes platforms](https://cloud.google.com/apigee/docs/hybrid/v1.3/install-before-begin#supported-platforms).

[https://docs.apigee.com/hybrid/what-is-hybrid](https://docs.apigee.com/hybrid/what-is-hybrid)


## Comparisons


### AWS vs. GCP 

Compare Google Cloud with AWS and highlight the similarities and differences between the two. 

[https://cloud.google.com/docs/compare/aws](https://cloud.google.com/docs/compare/aws) 


### DevOps vs. SRE

A video discussing differences and similarities between DevOps and SRE.

[https://www.youtube.com/watch?v=uTEL8Ff1Zvk](https://www.youtube.com/watch?v=uTEL8Ff1Zvk)

Some books on SRE from google.

[https://landing.google.com/sre/books/](https://landing.google.com/sre/books/)


## Accounts & Billing


### Concepts


#### Important Roles

[https://cloud.google.com/billing/docs/concepts#important_roles](https://cloud.google.com/billing/docs/concepts#important_roles)


#### Resource Hierarchy

[https://cloud.google.com/resource-manager/docs/cloud-platform-resource-hierarchy#resource-hierarchy-detail](https://cloud.google.com/resource-manager/docs/cloud-platform-resource-hierarchy#resource-hierarchy-detail)


#### Projects, Folders, Labels

[https://cloud.google.com/billing/docs/onboarding-checklist#projects-folders-labels](https://cloud.google.com/billing/docs/onboarding-checklist#projects-folders-labels)


#### Relationships between Resources

Relationships between organizations, projects, Cloud Billing accounts, and payments profiles

[https://cloud.google.com/billing/docs/concepts#relationships-between-resources](https://cloud.google.com/billing/docs/concepts#relationships-between-resources)


### Organizations

[https://cloud.google.com/resource-manager/docs/creating-managing-organization](https://cloud.google.com/resource-manager/docs/creating-managing-organization)


### Accounts

[https://cloud.google.com/billing/docs/how-to/manage-billing-account](https://cloud.google.com/billing/docs/how-to/manage-billing-account)


### Folders

[https://cloud.google.com/resource-manager/docs/creating-managing-folders](https://cloud.google.com/resource-manager/docs/creating-managing-folders)


### Billing Account & Payment Profile

[https://cloud.google.com/billing/docs/concepts#billing_account](https://cloud.google.com/billing/docs/concepts#billing_account)


### GCP Cloud Customer Onboarding Checklist

Google Cloud customers can be assisted in setting up their various Google Cloud resources to avoid common issues and enable best practices for access control and cost management. There are some design decisions and configuration options that help set you up for success in administering your cloud resources.

[https://cloud.google.com/billing/docs/onboarding-checklist](https://cloud.google.com/billing/docs/onboarding-checklist)


### Key Decisions

[https://cloud.google.com/billing/docs/onboarding-checklist#cloud-billing-accounts](https://cloud.google.com/billing/docs/onboarding-checklist#cloud-billing-accounts)


### Google Cloud Pricing Calculator

[https://cloud.google.com/products/calculator](https://cloud.google.com/products/calculator)

Managing GCP usage and cost trends is easier than you think. In this session, we'll show you how to quickly view your GCP costs, forecast your month-end bill, and provide an overview of some of the controls you can put in place to prevent budget overruns.

[https://www.youtube.com/watch?v=UocD6uY2-js](https://www.youtube.com/watch?v=UocD6uY2-js)


### Qwiklabs


#### Optimizing GCP Costs

Here you'll learn several ways to control and optimize your GCP costs, including setting up budgets and alerts, managing quota limits, and taking advantage of committed use discounts. In the hands-on labs, you’ll practice using various tools to control and optimize your GCP costs or to influence your technology teams to apply the cost optimization best practices.

[Optimizing Your GCP Costs](https://www.qwiklabs.com/quests/97?catalog_rank=%7B%22rank%22%3A4%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&search_id=7468028)


## Compliance

[GCP Compliance Offerings](https://cloud.google.com/security/compliance/offerings/#/)

[PCI Responsibility Matrix ](https://cloud.google.com/files/PCI_DSS_Shared_Responsibility_GCP_v32.pdf)

[GCP Security Controls](https://cloud.google.com/security/)

[Vault EaaS - Encryption As a Service](https://learn.hashicorp.com/tutorials/vault/eaas-transit)
