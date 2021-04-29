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

https://github.com/bobbae/gcp/wiki/Containers

## Namespaces

https://github.com/bobbae/gcp/wiki/Namespaces

# Kubernetes

Kubernetes is an open source container orchestration engine for automating deployment, scaling, and management of containerized applications. The open source project is hosted by the Cloud Native Computing Foundation (CNCF).

Kubernetes is a portable, extensible, open-source platform for managing containerized workloads and services, that facilitates both declarative configuration and automation. It has a large, rapidly growing ecosystem. Kubernetes services, support, and tools are widely available.

https://kubernetes.io/

[[https://d33wubrfki0l68.cloudfront.net/2475489eaf20163ec0f54ddc1d92aa8d4c87c96b/e7c81/images/docs/components-of-kubernetes.svg]]

## Kubernetes Control Plane

[[https://d33wubrfki0l68.cloudfront.net/d35c2b375b43b4fa374ae834f95224975418e33f/6b47b/images/blog/2018-06-05-11-ways-not-to-get-hacked/kubernetes-control-plane.png]]

https://kubernetes.io/docs/concepts/overview/components/

## API

https://kubernetes.io/docs/concepts/overview/kubernetes-api/

## Objects

A Kubernetes object is a "record of intent"--once you create the object, the Kubernetes system will constantly work to ensure that object exists. By creating an object, you're effectively telling the Kubernetes system what you want your cluster's workload to look like; this is your cluster's desired state.

https://kubernetes.io/docs/concepts/overview/working-with-objects/


## Google Kubernetes Engine (GKE)

https://github.com/bobbae/gcp/wiki/GKE

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

https://github.com/bobbae/gcp/wiki/Kubernetes-Origin

## Kubernetes Examples

https://github.com/bobbae/gcp/wiki/Kubernetes-Examples


## Kubernetes Details



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

https://github.com/bobbae/gcp/wiki/Kubernete-Networking




## Kubernetes Storage

https://github.com/bobbae/gcp/wiki/Kubernete-Storage

## Authentication and Authorization in Kubernetes

[https://www.youtube.com/watch?v=dAUJ3TBwDWo](https://www.youtube.com/watch?v=dAUJ3TBwDWo)

## Ingress

https://github.com/bobbae/gcp/wiki/Ingress




## Service Mesh

https://github.com/bobbae/gcp/wiki/Service-Mesh





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


## Scaling

https://github.com/bobbae/gcp/wiki/Kubernetes-scaling

## Qwiklabs

https://github.com/bobbae/gcp/wiki/Kubernetes-Qwiklabs