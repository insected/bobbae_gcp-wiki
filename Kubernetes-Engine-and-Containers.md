- [Containers](#containers)
  * [Namespaces](#namespaces)
- [Kubernetes](#kubernetes)
  * [Kubernetes Control Plane](#kubernetes-control-plane)
  * [API](#api)
  * [Objects](#objects)
  * [Google Kubernetes Engine (GKE)](#google-kubernetes-engine--gke-)
  * [An introduction to Kubernetes](#an-introduction-to-kubernetes)
  * [Kubectl](#kubectl)
    + [Kustomize](#kustomize)
  * [Kubernetes origin](#kubernetes-origin)
  * [Kubernetes Examples](#kubernetes-examples)
  * [Kubernetes Details](#kubernetes-details)
  * [Kubernetes Networking](#kubernetes-networking)
  * [Kubernetes Storage](#kubernetes-storage)
  * [Authentication and Authorization in Kubernetes](#authentication-and-authorization-in-kubernetes)
  * [Ingress](#ingress)
  * [Service Mesh](#service-mesh)
  * [Cloud Build & Cloud Code with Containers](#cloud-build---cloud-code-with-containers)
  * [K8s monitoring](#k8s-monitoring)
  * [Configuration as Data](#configuration-as-data)
  * [Binary Authorizations](#binary-authorizations)
  * [Scaling](#scaling)
  * [Qwiklabs](#qwiklabs)

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

https://github.com/bobbae/gcp/wiki/Cloud-Build



## K8s monitoring
https://github.com/bobbae/gcp/wiki/Kubernetes-Monitoring

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