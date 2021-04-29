- [Containers](#containers)
  * [What is a container?](#what-is-a-container-)
  * [Containers vs. VMs](#containers-vs-vms)
    + [Comparison of containerizing vs using VMs](#comparison-of-containerizing-vs-using-vms)
  * [Three ways to run containers in GCP](#three-ways-to-run-containers-in-gcp)
  * [Namespaces](#namespaces)
    + [Linux namespaces](#linux-namespaces)
    + [Network namespaces and how they are used in containers](#network-namespaces-and-how-they-are-used-in-containers)
- [Kubernetes](#kubernetes)
  * [Kubernetes Control Plane](#kubernetes-control-plane)
  * [Google Kubernetes Engine (GKE)](#google-kubernetes-engine--gke-)
  * [An introduction to Kubernetes](#an-introduction-to-kubernetes)
  * [Kubectl](#kubectl)
    + [Kustomize](#kustomize)
  * [Kubernetes origin](#kubernetes-origin)
    + [Borg](#borg)
    + [Omega](#omega)
    + [Twine / Tupperware](#twine---tupperware)
    + [Swarm](#swarm)
    + [Mesos](#mesos)
  * [Kubernetes Examples](#kubernetes-examples)
      - [How to create a GKE cluster](#how-to-create-a-gke-cluster)
    + [Building small containers](#building-small-containers)
    + [Organizing with Kubernetes namespaces](#organizing-with-kubernetes-namespaces)
    + [Upgrading with zero down time](#upgrading-with-zero-down-time)
    + [Mapping external services](#mapping-external-services)
    + [Terminating with Grace](#terminating-with-grace)
    + [Health check](#health-check)
  * [Kubernetes Details](#kubernetes-details)
    + [Google GKE Documentation](#google-gke-documentation)
    + [Kubernetes URLs](#kubernetes-urls)
    + [Resource Limits](#resource-limits)
    + [Requests and limits](#requests-and-limits)
    + [RBAC](#rbac)
    + [Deployment & Service](#deployment---service)
    + [Configmaps & Secrets](#configmaps---secrets)
    + [Stateful Sets](#stateful-sets)
    + [DaemonSet](#daemonset)
    + [CRD](#crd)
    + [Operator Pattern](#operator-pattern)
    + [Operator Hub](#operator-hub)
    + [Operator Sprawl](#operator-sprawl)
  * [Kubernetes Networking](#kubernetes-networking)
    + [Basics](#basics)
    + [Services networking](#services-networking)
    + [ingress networking](#ingress-networking)
  * [CNI](#cni)
  * [Kubernetes Storage](#kubernetes-storage)
    + [Storage Classes](#storage-classes)
    + [ceph and Rook](#ceph-and-rook)
    + [Block Devices](#block-devices)
  * [PVC Persistent Volume Claim](#pvc-persistent-volume-claim)
  * [Authentication and Authorization in Kubernetes](#authentication-and-authorization-in-kubernetes)
  * [Ingress](#ingress)
  * [GKE HA and Stateful Application, PVC](#gke-ha-and-stateful-application--pvc)
  * [Kubernetes applications on Google Cloud Marketplace](#kubernetes-applications-on-google-cloud-marketplace)
  * [GKE Operations](#gke-operations)
  * [Cloud Build & Cloud Code with Containers](#cloud-build---cloud-code-with-containers)
    + [Cloud Code](#cloud-code)
    + [Cloud Build](#cloud-build)
    + [Container Registry](#container-registry)
    + [Batch on GKE](#batch-on-gke)
  * [K8s monitoring](#k8s-monitoring)
    + [Prometheus](#prometheus)
    + [Grafana](#grafana)
  * [Configuration as Data](#configuration-as-data)
  * [Binary Authorizations](#binary-authorizations)
  * [HPA: Horizontal Pod Autoscaling](#hpa--horizontal-pod-autoscaling)
  * [Qwiklabs](#qwiklabs)
    + [GKE](#gke)
    + [GKE Solutions](#gke-solutions)
        * [GKE Deploy](#gke-deploy)
    + [Security in GKE](#security-in-gke)
        * [Deploying Python Apps on GKE](#deploying-python-apps-on-gke)
    + [Cloud Logging on GKE](#cloud-logging-on-gke)
    + [Migrating to GKE](#migrating-to-gke)
        * [Java Application Development](#java-application-development)
    + [Operations Suite on GKE](#operations-suite-on-gke)
        * [Deploy Kubernetes Load Balancer with Terraform](#deploy-kubernetes-load-balancer-with-terraform)
  * [Service Mesh](#service-mesh)
    + [Istio](#istio)
    + [Istiod vs microservices](#istiod-vs-microservices)
  * [Envoy](#envoy)
  * [Apigee Envoy](#apigee-envoy)
  * [Ambassador Edge Stack and Consul Service Mesh](#ambassador-edge-stack-and-consul-service-mesh)
  * [Linkerd](#linkerd)
  * [Multi-cluster services](#multi-cluster-services)
    + [Configuring GKE MCS](#configuring-gke-mcs)
    + [Multi-cluster ingress](#multi-cluster-ingress)

<small><i><a href='http://ecotrust-canada.github.io/markdown-toc/'>Table of contents generated with markdown-toc</a></i></small>

# Containers


## What is a container?

A container is a standard unit of software that packages up code and all its dependencies so the application runs quickly and reliably from one computing environment to another. A Docker container image is a lightweight, standalone, executable package of software that includes everything needed to run an application: code, runtime, system tools, system libraries and settings.

[https://www.docker.com/resources/what-container](https://www.docker.com/resources/what-container)


## Containers vs. VMs

Virtual machines and containers differ in several ways, but the primary difference is that containers provide a way to virtualize an OS so that multiple workloads can run on a single OS instance. With VMs, the hardware is being virtualized to run multiple OS instances. Containers’ speed, agility, and portability make them yet another tool to help streamline software development.

 
### Comparison of containerizing vs using VMs

[https://www.youtube.com/watch?v=TvnZTi_gaNc](https://www.youtube.com/watch?v=TvnZTi_gaNc)


## Three ways to run containers in GCP

Find out the top three ways you can run your containers on Google Cloud! Google Kubernetes Engine for a container orchestration solution, Cloud Run for a fully serverless approach and Compute Engine to simply use Virtual Machines.

[https://www.youtube.com/watch?v=jh0fPT-AWwM](https://www.youtube.com/watch?v=jh0fPT-AWwM)


## Namespaces

Namespaces are a feature of the Linux kernel that partitions kernel resources such that one set of processes sees one set of resources while another set of processes sees a different set of resources. The feature works by having the same namespace for a set of resources and processes, but those namespaces refer to distinct resources. Resources may exist in multiple spaces. Examples of such resources are process IDs, hostnames, user IDs, file names, and some names associated with network access, and interprocess communication.



### Linux namespaces

Namespaces are a fundamental aspect of containers on Linux.

The term "namespace" is often used for a type of namespace (e.g. process ID) as well as for a particular space of names.

A Linux system starts out with a single namespace of each type, used by all processes. Processes can create additional namespaces and join different namespaces.

[https://www.youtube.com/watch?v=kl8roLaLy-g](https://www.youtube.com/watch?v=kl8roLaLy-g)

### Network namespaces and how they are used in containers

[https://www.youtube.com/watch?v=j_UUnlVC2Ss&list=TLPQMTQxMDIwMjD4ry4yOmhx2w&index=2](https://www.youtube.com/watch?v=j_UUnlVC2Ss&list=TLPQMTQxMDIwMjD4ry4yOmhx2w&index=2)



# Kubernetes

Kubernetes is an open source container orchestration engine for automating deployment, scaling, and management of containerized applications. The open source project is hosted by the Cloud Native Computing Foundation (CNCF).

https://kubernetes.io/

## Kubernetes Control Plane

[[https://d33wubrfki0l68.cloudfront.net/d35c2b375b43b4fa374ae834f95224975418e33f/6b47b/images/blog/2018-06-05-11-ways-not-to-get-hacked/kubernetes-control-plane.png]]

## Google Kubernetes Engine (GKE)
Secured and fully managed Kubernetes service with revolutionary autopilot mode of operation.

## An introduction to Kubernetes

[Kubernetes](https://kubernetes.io) is an open-source container-orchestration system for automating computer application deployment, scaling, and management. It was originally designed by Google and is now maintained by the Cloud Native Computing Foundation.

[https://www.youtube.com/watch?v=pQ87vVMZK-A](https://www.youtube.com/watch?v=pQ87vVMZK-A)

[https://www.youtube.com/watch?v=Krpb44XR0bk](https://www.youtube.com/watch?v=Krpb44XR0bk)


## Kubectl

The Kubernetes command-line tool, [kubectl](https://kubernetes.io/docs/reference/kubectl/kubectl/), allows you to run commands against Kubernetes clusters. You can use kubectl to deploy applications, inspect and manage cluster resources, and view logs. For a complete list of kubectl operations, see [Overview of kubectl](https://kubernetes.io/docs/reference/kubectl/overview/).

[https://www.youtube.com/watch?v=azuwXALfyRg](https://www.youtube.com/watch?v=azuwXALfyRg)


### Kustomize

Kustomize introduces a template-free way to customize application configuration that simplifies the use of off-the-shelf applications. Now, built into kubectl as apply -k.

[https://www.youtube.com/watch?v=uvH84BviDS4](https://www.youtube.com/watch?v=uvH84BviDS4)

https://kustomize.io/

## Kubernetes origin


### Borg

Borg is Google's main cluster management system that manages long running production services and non-production batch jobs on the same set of machines to maximize cluster utilization. Omega is a clean-slate rewrite of Borg using more principled architecture.

Google's Borg system is a cluster manager that runs hundreds of thousands of jobs, from many thousands of different applications, across a number of clusters each with up to tens of thousands of machines. It achieves high utilization by combining admission control, efficient task-packing, over-commitment, and machine sharing with process-level performance isolation. It supports high-availability applications with runtime features that minimize fault-recovery time, and scheduling policies that reduce the probability of correlated failures. Borg simplifies life for its users by offering a declarative job specification language, name service integration, real-time job monitoring, and tools to analyze and simulate system behavior.

[https://research.google/pubs/pub43438/](https://research.google/pubs/pub43438/)

### Omega

Omega is a Google's cluster management system based on shared state. In Omega, all system state lives in a consistent Paxos-based storage system that is accessed by a multitude of components which act as peers. A new parallel scheduler architecture is built around shared state, using lock-free optimistic concurrency and performance scalability.   Compared to monolithic schedulers or Two-level schedulers like Mesos and Hadoop-on-demand, the Omega addresses the entire cluster state in a scheduler.

https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/41684.pdf

Kubernetes is the latest open source container manager that draws on lessons from both previous systems.   





https://mwhittaker.github.io/papers/html/burns2016borg.html

All three systems use containers for security and performance isolation. Container technology has evolved greatly since the inception of Borg from chroot to jails to cgroups. Of course containers cannot prevent all forms of performance isolation. Today, containers also contain program images.

https://research.google/pubs/pub44843/

### Twine / Tupperware

Facebook's own hyperscale orchestration tool.

https://engineering.fb.com/2019/06/06/data-center-engineering/twine/

### Swarm
Docker Swarm is Docker’s native Container Orchestration Engine. 

https://github.com/docker/classicswarm

### Mesos

Mesos takes more of a distributed approach to managing datacenter and cloud resources. Mesos can have multiple masters which use Zookeeper to keep track of the cluster state amongst the masters and form a high-availability cluster.

http://mesos.apache.org/

## Kubernetes Examples

#### How to create a GKE cluster

This video will teach you how to create a Google Kubernetes Engine (GKE) cluster using Terraform.

[https://www.youtube.com/watch?v=Vcv6GapxUCI](https://www.youtube.com/watch?v=Vcv6GapxUCI)

Here are some tutorials for using Terraform to manage Kubernetes on GCP.
[HashCorp Terraform Kubernetes Tutorials](https://learn.hashicorp.com/tutorials/terraform/gke?in=terraform/kubernetes)

### Building small containers

A video to show you how you can build small containers to make your Kubernetes deployments faster and more secure.

[https://www.youtube.com/watch?v=wGz_cbtCiEA](https://www.youtube.com/watch?v=wGz_cbtCiEA)


### Organizing with Kubernetes namespaces

This video shows how to work with Namespaces and how they can help you manage your Kubernetes resources.

[https://www.youtube.com/watch?v=xpnZX3if9Tc](https://www.youtube.com/watch?v=xpnZX3if9Tc)


### Upgrading with zero down time

[https://www.youtube.com/watch?v=ajbC1yTW2x0](https://www.youtube.com/watch?v=ajbC1yTW2x0)


### Mapping external services

[https://www.youtube.com/watch?v=fvpq4jqtuZ8](https://www.youtube.com/watch?v=fvpq4jqtuZ8)


### Terminating with Grace

[https://www.youtube.com/watch?v=Z_l_kE1MDTc](https://www.youtube.com/watch?v=Z_l_kE1MDTc)


### Health check

[https://www.youtube.com/watch?v=mxEvAPQRwhw](https://www.youtube.com/watch?v=mxEvAPQRwhw)


## Kubernetes Details

### Google GKE Documentation

[https://cloud.google.com/kubernetes-engine/docs](https://cloud.google.com/kubernetes-engine/docs)


### Kubernetes URLs

[https://github.com/ramitsurana/awesome-kubernetes](https://github.com/ramitsurana/awesome-kubernetes)


### Resource Limits

When you specify a Pod, you can optionally specify how much of each resource a Container needs. The most common resources to specify are CPU and memory (RAM); there are others.

When you specify the resource request for Containers in a Pod, the scheduler uses this information to decide which node to place the Pod on. When you specify a resource limit for a Container, the kubelet enforces those limits so that the running container is not allowed to use more of that resource than the limit you set. The kubelet also reserves at least the request amount of that system resource specifically for that container to use.

### Requests and limits 

If the node where a Pod is running has enough of a resource available, it's possible (and allowed) for a container to use more resource than its request for that resource specifies. However, a container is not allowed to use more than its resource limit.

[https://www.youtube.com/watch?v=xjpHggHKm78&list=PLIivdWyY5sqL3xfXz5xJvwzFW_tlQB_GB&index=4](https://www.youtube.com/watch?v=xjpHggHKm78&list=PLIivdWyY5sqL3xfXz5xJvwzFW_tlQB_GB&index=4)


### RBAC

Role-based access control (RBAC) is a method of regulating access to computer or network resources based on the roles of individual users within your organization.

RBAC authorization uses the rbac.authorization.k8s.io API group to drive authorization decisions, allowing you to dynamically configure policies through the Kubernetes API.

[https://www.youtube.com/watch?v=4HMRFcg6nEY](https://www.youtube.com/watch?v=4HMRFcg6nEY)


### Deployment & Service

A Deployment provides declarative updates for Pods and ReplicaSets.

You describe a desired state in a Deployment, and the Deployment Controller changes the actual state to the desired state at a controlled rate. You can define Deployments to create new ReplicaSets, or to remove existing Deployments and adopt all their resources with new Deployments.

A Service is an abstract way to expose an application running on a set of Pods as a network service.
With Kubernetes you don't need to modify your application to use an unfamiliar service discovery mechanism. Kubernetes gives Pods their own IP addresses and a single DNS name for a set of Pods, and can load-balance across them


[https://www.youtube.com/watch?v=qmDzcu5uY1I](https://www.youtube.com/watch?v=qmDzcu5uY1I)

https://kubernetes.io/docs/concepts/services-networking/connect-applications-service/

### Configmaps & Secrets

A ConfigMap is an API object used to store non-confidential data in key-value pairs. Pods can consume ConfigMaps as environment variables, command-line arguments, or as configuration files in a volume.

A ConfigMap allows you to decouple environment-specific configuration from your container images, so that your applications are easily portable.

Kubernetes Secrets let you store and manage sensitive information, such as passwords, OAuth tokens, and ssh keys. Storing confidential information in a Secret is safer and more flexible than putting it verbatim in a Pod definition or in a container image. See Secrets design document for more information.

A Secret is an object that contains a small amount of sensitive data such as a password, a token, or a key. Such information might otherwise be put in a Pod specification or in an image. Users can create Secrets and the system also creates some Secrets.

[https://www.youtube.com/watch?v=FAnQTgr04mU](https://www.youtube.com/watch?v=FAnQTgr04mU)


### Stateful Sets

StatefulSet is the workload API object used to manage stateful applications.

Manages the deployment and scaling of a set of Pods, and provides guarantees about the ordering and uniqueness of these Pods.

[https://www.youtube.com/watch?v=pPQKAR1pA9U](https://www.youtube.com/watch?v=pPQKAR1pA9U)


### DaemonSet

A DaemonSet ensures that all (or some) Nodes run a copy of a Pod. As nodes are added to the cluster, Pods are added to them. As nodes are removed from the cluster, those Pods are garbage collected. Deleting a DaemonSet will clean up the Pods it created.

[https://kubernetes.io/docs/concepts/workloads/controllers/daemonset/](https://kubernetes.io/docs/concepts/workloads/controllers/daemonset/)


### CRD

CRD stands for  Custom Resource Definition.

A resource is an endpoint in the [Kubernetes API](https://kubernetes.io/docs/reference/using-api/api-overview/) that stores a collection of [API objects](https://kubernetes.io/docs/concepts/overview/working-with-objects/kubernetes-objects/) of a certain kind; for example, the built-in pods resource contains a collection of Pod objects.

A custom resource is an extension of the Kubernetes API that is not necessarily available in a default Kubernetes installation. It represents a customization of a particular Kubernetes installation. However, many core Kubernetes functions are now built using custom resources, making Kubernetes more modular. Custom resources can appear and disappear in a running cluster through dynamic registration, and cluster admins can update custom resources independently of the cluster itself. Once a custom resource is installed, users can create and access its objects using [kubectl](https://kubernetes.io/docs/reference/kubectl/overview/), just as they do for built-in resources like Pods.

[https://kubernetes.io/docs/concepts/extend-kubernetes/api-extension/custom-resources/](https://kubernetes.io/docs/concepts/extend-kubernetes/api-extension/custom-resources/)

Kubebuilder is a framework for building Kubernetes APIs using custom resource definitions (CRDs).

https://book.kubebuilder.io/quick-start.html

https://github.com/kubernetes-sigs/kubebuilder


### Operator Pattern

In Kubernetes, objects are analogous to a job or a completed task in the real world. You can use them to define common tasks, store them in a version control system, and apply them with kubectl apply. Kubernetes ensures that this triggers everything necessary to bring your declarative description to life by creating the dependent resources (like pods) to run your software. Kubernetes contains a number of built-in object types that can be created with this workflow, like Deployments and Services. With Operators, Kubernetes allows cluster maintainers or software providers to define their own Kubernetes object types, called custom resource definitions (CRDs). These objects can be handled by the Kubernetes API, just like built-in object types. Inside the Operator code, authors can define how to act on those custom objects. Operators are software extensions to Kubernetes that make use of [custom resources](https://kubernetes.io/docs/concepts/extend-kubernetes/api-extension/custom-resources/) to manage applications and their components. Operators follow Kubernetes principles, notably the [control loop](https://kubernetes.io/docs/concepts/architecture/controller).

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

### Operator Hub

[https://operatorhub.io/](https://operatorhub.io/)


### Operator Sprawl

[https://thenewstack.io/the-runaway-problem-of-kubernetes-operators-and-dependency-lifecycles/](https://thenewstack.io/the-runaway-problem-of-kubernetes-operators-and-dependency-lifecycles/)


## Kubernetes Networking

Networking is a central part of Kubernetes, but it can be challenging to understand exactly how it is expected to work. There are 4 distinct networking problems to address:

1. Highly-coupled container-to-container communications: this is solved by Pods and localhost communications.
2. Pod-to-Pod communications: this is the primary focus of this document.
3. Pod-to-Service communications: this is covered by services.
4. External-to-Service communications: this is covered by services.

https://www.stackrox.com/post/2020/01/kubernetes-networking-demystified/

### Basics

https://www.youtube.com/watch?v=InZVNuKY5GY


### Services networking

[https://www.youtube.com/watch?v=NFApeJRXos4](https://www.youtube.com/watch?v=NFApeJRXos4)

### ingress networking

[https://www.youtube.com/watch?v=40VfZ_nIFWI](https://www.youtube.com/watch?v=40VfZ_nIFWI)

[https://www.youtube.com/watch?v=_BbxJGiMtL8](https://www.youtube.com/watch?v=_BbxJGiMtL8)

https://www.youtube.com/watch?v=sHUSiM8jqbA

## CNI

CNI (Container Network Interface), a Cloud Native Computing Foundation project, consists of a specification and libraries for writing plugins to configure network interfaces in Linux containers, along with a number of supported plugins. CNI concerns itself only with network connectivity of containers and removing allocated resources when the container is deleted. Because of this focus, CNI has a wide range of support and the specification is simple to implement.

https://github.com/containernetworking/cni



## Kubernetes Storage

Kubernetes containers are stateless as a core principle, but data must still be managed, preserved, and made accessible to other services. Stateless means that the container is running in isolation without any knowledge of past transactions, which makes it easy to replace, delete, or distribute the container. However, it also means that data will be lost for certain lifecycle events like restart or deletion.


[https://www.youtube.com/watch?v=qktFhjJmFhg](https://www.youtube.com/watch?v=qktFhjJmFhg)

### Storage Classes

A StorageClass provides a way for administrators to describe the "classes" of storage they offer. Different classes might map to quality-of-service levels, or to backup policies, or to arbitrary policies determined by the cluster administrators. Kubernetes itself is unopinionated about what classes represent. This concept is sometimes called "profiles" in other storage systems.

https://kubernetes.io/docs/concepts/storage/storage-classes/

### ceph and Rook

Rook is a storage orchestration tool that provides a cloud-native, open source solution for a diverse set of storage providers. Rook uses the power of Kubernetes to turn a storage system into self-managing services that provide a seamless experience for saving Kubernetes application or deployment data.

Ceph is a highly scalable distributed-storage solution offering object, block, and file storage. Ceph clusters are designed to run on any hardware using the so-called CRUSH algorithm (Controlled Replication Under Scalable Hashing).

https://www.digitalocean.com/community/tutorials/how-to-set-up-a-ceph-cluster-within-kubernetes-using-rook

### Block Devices 

You may use Ceph Block Device images with Kubernetes v1.13 and later through ceph-csi, which dynamically provisions RBD images to back Kubernetes volumes and maps these RBD images as block devices (optionally mounting a file system contained within the image) on worker nodes running pods that reference an RBD-backed volume. Ceph stripes block device images as objects across the cluster, which means that large Ceph Block Device images have better performance than a standalone server.

https://docs.ceph.com/en/latest/rbd/rbd-kubernetes/

### Volumes

On-disk files in a container are ephemeral, which presents some problems for non-trivial applications when running in containers. One problem is the loss of files when a container crashes. The kubelet restarts the container but with a clean state. A second problem occurs when sharing files between containers running together in a Pod. 

Docker has a concept of volumes, though it is somewhat looser and less managed. A Docker volume is a directory on disk or in another container. Docker provides volume drivers, but the functionality is somewhat limited.

Kubernetes supports many types of volumes. A Pod can use any number of volume types simultaneously. Ephemeral volume types have a lifetime of a pod, but persistent volumes exist beyond the lifetime of a pod. When a pod ceases to exist, Kubernetes destroys ephemeral volumes; however, Kubernetes does not destroy persistent volumes. For any kind of volume in a given pod, data is preserved across container restarts.

At its core, a volume is a directory, possibly with some data in it, which is accessible to the containers in a pod. How that directory comes to be, the medium that backs it, and the contents of it are determined by the particular volume type used.


https://kubernetes.io/docs/concepts/storage/volumes/

### Snapshots

In Kubernetes, a VolumeSnapshot represents a snapshot of a volume on a storage system. This document assumes that you are already familiar with Kubernetes persistent volumes.


https://kubernetes.io/docs/concepts/storage/volume-snapshots/

### Dynamic Volume Provisioning

Dynamic volume provisioning allows storage volumes to be created on-demand. Without dynamic provisioning, cluster administrators have to manually make calls to their cloud or storage provider to create new storage volumes, and then create PersistentVolume objects to represent them in Kubernetes. The dynamic provisioning feature eliminates the need for cluster administrators to pre-provision storage. Instead, it automatically provisions storage when it is requested by users.


https://kubernetes.io/docs/concepts/storage/dynamic-provisioning/

### CSI

Container Storage Interface (CSI) defines a standard interface for container orchestration systems (like Kubernetes) to expose arbitrary storage systems to their container workloads.


https://kubernetes.io/docs/concepts/storage/volumes/#csi

### PVC Persistent Volume Claim

[https://www.youtube.com/watch?v=0swOh5C3OVM](https://www.youtube.com/watch?v=0swOh5C3OVM)


## Authentication and Authorization in Kubernetes

[https://www.youtube.com/watch?v=dAUJ3TBwDWo](https://www.youtube.com/watch?v=dAUJ3TBwDWo)

## Ingress

https://github.com/bobbae/gcp/wiki/Ingress

[https://www.youtube.com/watch?v=80Ew_fsV4rM](https://www.youtube.com/watch?v=80Ew_fsV4rM)


## GKE HA and Stateful Application, PVC

Kubernetes is a great tool to host your highly available applications but what happens when you have to work with stateful workloads? 

[https://www.youtube.com/watch?v=rRZtZX0PDFc](https://www.youtube.com/watch?v=rRZtZX0PDFc)


## Kubernetes applications on Google Cloud Marketplace

The Kubernetes apps in Cloud Marketplace include container images and configuration files, such as a kubectl configuration or a[ Helm chart](https://helm.sh/docs/topics/charts/). When you deploy an app from Cloud Marketplace, the Kubernetes resources are created in your cluster, and you can manage the resources as a group.

[https://cloud.google.com/marketplace/docs/kubernetes-apps](https://cloud.google.com/marketplace/docs/kubernetes-apps)


## GKE Operations

A video about using Cloud Logging on GKE.

[https://www.youtube.com/watch?v=IusP8jDfnt4](https://www.youtube.com/watch?v=IusP8jDfnt4)


## Cloud Build & Cloud Code with Containers


### Cloud Code

Using Cloud Code with Kubernetes.

[https://www.youtube.com/watch?v=KNd0mTxcQ_M](https://www.youtube.com/watch?v=KNd0mTxcQ_M)


### Cloud Build

Cloud Build is a service that executes your builds on Google Cloud Platform infrastructure. Cloud Build can import source code from Google Cloud Storage, Cloud Source Repositories, GitHub, or Bitbucket, execute a build to your specifications, and produce artifacts such as Docker containers or Java archives.

A video about Cloud Build with Containers.

[https://www.youtube.com/watch?v=w7dMHiEyGAs](https://www.youtube.com/watch?v=w7dMHiEyGAs)

Cloud Build executes your build as a series of build steps, where each build step is run in a Docker container. A build step can do anything that can be done from a container irrespective of the environment. To perform your tasks, you can either [use the supported build steps](https://cloud.google.com/cloud-build/docs/configuring-builds/build-test-deploy-artifacts) provided by Cloud Build or [write your own build steps](https://cloud.google.com/cloud-build/docs/create-custom-build-steps).

[https://cloud.google.com/cloud-build/docs](https://cloud.google.com/cloud-build/docs)


### Container Registry

Google Container Registry is a private container image registry that runs on Google Cloud's reliable, fast, and secure infrastructure. You can access Container Registry through secure HTTPS endpoints, which allow you to push, pull, and manage images from any system, VM instance, or your own hardware. Additionally, you can use the [Docker credential helper](https://cloud.google.com/container-registry/docs/advanced-authentication#docker_credential_helper) command-line tool to configure Docker to authenticate directly with Container Registry.

While Docker provides a central registry for storing public images, you might not want your images to be accessible to the world. To control access to your images, you must store your images in a private registry.

[Container Registry: Qwik Start](https://www.qwiklabs.com/focuses/1768?catalog_rank=%7B%22rank%22%3A7%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&parent=catalog&search_id=7467880)


### Batch on GKE

Batch on GKE (Batch) is a cloud-native solution for scheduling and managing batch workloads. With Batch, you can leverage the on-demand and flexible nature of cloud. Batch is based on Kubernetes and containers so your jobs are portable.

[https://cloud.google.com/kubernetes-engine/docs/concepts/batch](https://cloud.google.com/kubernetes-engine/docs/concepts/batch)

A video about using Batch on GKE.

[https://www.youtube.com/watch?v=qLSLs-ko3ik](https://www.youtube.com/watch?v=qLSLs-ko3ik)

## K8s monitoring

### Prometheus

[https://www.youtube.com/watch?v=h4Sl21AKiDg](https://www.youtube.com/watch?v=h4Sl21AKiDg)

[https://www.youtube.com/watch?v=XToKHYXSUyc](https://www.youtube.com/watch?v=XToKHYXSUyc)


### Grafana

[https://grafana.com/](https://grafana.com/)


## Configuration as Data

[https://cloud.google.com/blog/products/containers-kubernetes/understanding-configuration-as-data-in-kubernetes](https://cloud.google.com/blog/products/containers-kubernetes/understanding-configuration-as-data-in-kubernetes)


## Binary Authorizations

Binary Authorization is a service on Google Cloud that provides software supply-chain security for container-based applications. Binary Authorization extends Google Kubernetes Engine (GKE) and Anthos clusters on VMware with deploy time enforcement of security policies. On Anthos clusters on VMware, Binary Authorization extends this policy enforcement to hybrid-cloud architectures. Binary Authorization works with container images from Container Registry, Artifact Registry and other container image registries.

With Binary Authorization, you can automatically check each component of your software supply chain, ensuring the quality and integrity of your software before an application is deployed to your production environment.

[https://cloud.google.com/binary-authorization/docs/overview](https://cloud.google.com/binary-authorization/docs/overview)


## HPA: Horizontal Pod Autoscaling

HPA changes the shape of your Kubernetes workload by automatically increasing or decreasing the number of Pods in response to the workload's CPU or memory consumption, or in response to custom metrics reported from within Kubernetes or external metrics from sources outside of your cluster.

[https://cloud.google.com/kubernetes-engine/docs/concepts/horizontalpodautoscaler](https://cloud.google.com/kubernetes-engine/docs/concepts/horizontalpodautoscaler)

There are also Vertical Pod Autoscaling (VPA) and Cluster auto scaling.

https://github.com/bobbae/gcp/wiki/Kubernetes-scaling

## Qwiklabs


### GKE

Kubernetes is the most popular container orchestration system, and Google Kubernetes Engine was designed specifically to support managed Kubernetes deployments in Google Cloud. In this advanced-level quest, you will get hands-on practice configuring Docker images, containers, and deploying fully-fledged Kubernetes Engine applications. This quest will teach you the practical skills needed for integrating container orchestration into your own workflow. 

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


## Service Mesh

https://github.com/bobbae/gcp/wiki/Service-Mesh


[https://www.youtube.com/watch?v=6zDrLvpfCK4](https://www.youtube.com/watch?v=6zDrLvpfCK4)

Enterprises are increasingly adopting microservices to enable new levels of IT agility, scale, and innovation — but a successful microservices implementation is notoriously complicated. As the number of services an organization uses grows, complexity and risk can increase rapidly. Moreover, microservices need to be exposed as APIs to enable seamless access for internal groups — or with external partners to increase operational efficiency and speed up development. 

https://github.com/bobbae/gcp/wiki/Service-Mesh

This video shows how to build a secure and scalable [microservices architecture](https://medium.com/hashmapinc/the-what-why-and-how-of-a-microservices-architecture-4179579423a9) with Kubernetes, Istio, and Apigee API management platform.

[https://www.youtube.com/watch?v=IblDMVwSSk4](https://www.youtube.com/watch?v=IblDMVwSSk4)


### Istio

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


### Istiod vs microservices

[https://blog.christianposta.com/microservices/istio-as-an-example-of-when-not-to-do-microservices/](https://blog.christianposta.com/microservices/istio-as-an-example-of-when-not-to-do-microservices/)


## Envoy

Envoy is  a L7 edge service Proxy used widely by service mesh controllers such as Consul, Contour and istio. Envoy is also used by API gateway like Ambassador.

[Watch a Video about Borg, Cloud Load Balancing, Kubernetes and Envoy into service mesh driven by Istio](https://www.youtube.com/watch?v=glATqKI-WR8).

There are many [Open source projects built on Envoy Proxy](https://www.envoyproxy.io/community).

[Events in the life of a request](https://www.envoyproxy.io/docs/envoy/latest/intro/life_of_a_request) passing through an Envoy proxy is complicated.
How a request flows through the components in a network depends on the network topology. Envoy can be used in a wide variety of networking topologies. Envoy originated as a service mesh sidecar proxy, factoring out load balancing, routing, observability, security and discovery services from applications. In the service mesh model, requests flow through Envoys as a gateway to the network. Requests arrive at an Envoy via either ingress or egress listeners.  

https://github.com/bobbae/gcp/wiki/L7-Proxies

## Apigee Envoy

Wanting to know how to use Envoy to protect your microservices? In this video, we give you a demo on how to enforce policies for any microservice within a service mesh via the Apigee adapter for Envoy. Watch to learn about this tool, and see if it’s the best choice for your specific use case! 

[https://www.youtube.com/watch?v=BNkfoZt-jvU](https://www.youtube.com/watch?v=BNkfoZt-jvU)


## Ambassador Edge Stack and Consul Service Mesh

[Consul](https://www.consul.io/)  is a widely used service mesh. You can use Consul with [Ambassador Edge Stack](https://www.getambassador.io/docs/), as it natively supports Consul for service discovery and end-to-end TLS (including mTLS between services). This capability is particularly useful when deploying Ambassador Edge Stack in so-called hybrid clouds, where applications are deployed on VMs and Kubernetes. In this environment, Ambassador Edge Stack can securely route over TLS to any application regardless of where it is deployed.


[https://www.youtube.com/watch?v=XW3AXQfAaQc](https://www.youtube.com/watch?v=XW3AXQfAaQc)


## Linkerd

https://linkerd.io/

[https://www.youtube.com/watch?v=Bj7gGQUiDuk](https://www.youtube.com/watch?v=Bj7gGQUiDuk)

Linkerd and istio comparison. 

https://www.infracloud.io/blogs/service-mesh-comparison-istio-vs-linkerd/

## Multi-cluster services

Multi-cluster Services (MCS)  is a cross-cluster Service discovery and invocation mechanism for Google Kubernetes Engine (GKE) that leverages the existing Service object. Services enabled with this feature are discoverable and accessible across clusters with a virtual IP, matching the behavior of a ClusterIP Service accessible in a cluster. Just like your existing Services, MCS is compatible with community-driven and open APIs, ensuring your workloads remain portable.

https://cloud.google.com/kubernetes-engine/docs/concepts/multi-cluster-services

### Configuring GKE MCS

The Google Kubernetes Engine (GKE) MCS feature extends the reach of the Kubernetes Service beyond the cluster boundary and lets you discover and invoke Services across multiple GKE clusters. You can export a subset of existing Services or new Services.

https://cloud.google.com/kubernetes-engine/docs/how-to/multi-cluster-services

### Multi-cluster ingress

Multi-cluster Ingress (MCI) is a cloud-hosted multi-cluster Ingress controller for Anthos clusters. It's a Google-hosted service that supports deploying shared load balancing resources across clusters and across regions.

https://cloud.google.com/kubernetes-engine/docs/how-to/multi-cluster-ingress-setup


