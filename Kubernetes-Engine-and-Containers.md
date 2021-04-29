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

https://github.com/bobbae/gcp/wiki/Kubernetes-Details

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