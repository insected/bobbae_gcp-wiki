

# Containers

https://github.com/bobbae/gcp/wiki/Containers

## Namespaces

https://github.com/bobbae/gcp/wiki/Namespaces

# Kubernetes

<img src="http://www.aquasec.com/wp-content/uploads/2020/11/Kubernetes-101-Architecture-Diagram.jpg" width="700">

https://kubernetes.io/

https://www.youtube.com/watch?v=Rl5M1CzgEH4

<img src="https://d1jnx9ba8s6j9r.cloudfront.net/blog/wp-content/uploads/2018/08/q1-1.png" width="300">

Kubernetes is an open source container orchestration engine for automating deployment, scaling, and management of containerized applications. The open source project is hosted by the Cloud Native Computing Foundation (CNCF).

https://www.youtube.com/watch?v=cC46cg5FFAM&list=PLIivdWyY5sqLmnGdKSdQIXq2sd_1bWSnx

Kubernetes is a portable, extensible, open-source platform for managing containerized workloads and services, that facilitates both declarative configuration and automation. It has a large, rapidly growing ecosystem. Kubernetes services, support, and tools are widely available.

https://www.youtube.com/watch?v=X48VuDVv0do

<img src="https://d1jnx9ba8s6j9r.cloudfront.net/blog/wp-content/uploads/2018/08/Application.png" width="700">

Kubernetes API lets you query and manipulate the state of objects in Kubernetes. The core of Kubernetes' control plane is the API server and the HTTP API that it exposes. Users, the different parts of your cluster, and external components all communicate with one another through the API server.

<img src="https://d33wubrfki0l68.cloudfront.net/2475489eaf20163ec0f54ddc1d92aa8d4c87c96b/e7c81/images/docs/components-of-kubernetes.svg" width="700">

## GKE

https://github.com/bobbae/gcp/wiki/GKE

## Kubernetes Control Plane

<img src="https://d33wubrfki0l68.cloudfront.net/d35c2b375b43b4fa374ae834f95224975418e33f/6b47b/images/blog/2018-06-05-11-ways-not-to-get-hacked/kubernetes-control-plane.png" width="600">

https://kubernetes.io/docs/concepts/overview/components/

## API

https://kubernetes.io/docs/concepts/overview/kubernetes-api/

## Objects

A Kubernetes object is a "record of intent"--once you create the object, the Kubernetes system will constantly work to ensure that object exists. By creating an object, you're effectively telling the Kubernetes system what you want your cluster's workload to look like; this is your cluster's desired state.

https://kubernetes.io/docs/concepts/overview/working-with-objects/


## Google Kubernetes Engine (GKE)

https://github.com/bobbae/gcp/wiki/GKE

## An introduction to Kubernetes

<img src="https://d1jnx9ba8s6j9r.cloudfront.net/blog/wp-content/uploads/2018/08/5-1.png" width="700">

[Kubernetes](https://kubernetes.io) is an open-source container-orchestration system for automating computer application deployment, scaling, and management. It was originally designed by Google and is now maintained by the Cloud Native Computing Foundation.

[https://www.youtube.com/watch?v=pQ87vVMZK-A](https://www.youtube.com/watch?v=pQ87vVMZK-A)

[https://www.youtube.com/watch?v=Krpb44XR0bk](https://www.youtube.com/watch?v=Krpb44XR0bk)

<img src="https://d1jnx9ba8s6j9r.cloudfront.net/blog/wp-content/uploads/2018/08/Containers-1.png" width="600">

## Kubectl

The Kubernetes command-line tool, [kubectl](https://kubernetes.io/docs/reference/kubectl/kubectl/), allows you to run commands against Kubernetes clusters. You can use kubectl to deploy applications, inspect and manage cluster resources, and view logs. For a complete list of kubectl operations, see [Overview of kubectl](https://kubernetes.io/docs/reference/kubectl/overview/).

[https://www.youtube.com/watch?v=azuwXALfyRg](https://www.youtube.com/watch?v=azuwXALfyRg)


### Kustomize

<img src="https://miro.medium.com/max/1575/1*qZV6wiQr4yet746qAl-G7A.png" width="600">

Kustomize introduces a template-free way to customize application configuration that simplifies the use of off-the-shelf applications. Now, built into kubectl as apply -k.

[https://www.youtube.com/watch?v=uvH84BviDS4](https://www.youtube.com/watch?v=uvH84BviDS4)

https://kustomize.io/

https://itnext.io/helm-is-not-enough-you-also-need-kustomize-82bae896816e


## Kubernetes origin

https://github.com/bobbae/gcp/wiki/Kubernetes-Origin

## Kubernetes Examples

https://github.com/bobbae/gcp/wiki/Kubernetes-Examples


## Kubernetes Architecture

https://github.com/bobbae/gcp/wiki/Kubernetes-Architecture

<img src="https://d1jnx9ba8s6j9r.cloudfront.net/blog/wp-content/uploads/2018/08/15-1.png" width="700">

## Kubernetes Networking

https://github.com/bobbae/gcp/wiki/Kubernetes-Networking

<img src="https://d1jnx9ba8s6j9r.cloudfront.net/blog/wp-content/uploads/2018/08/16-1.png" width="600">

## Kubernetes Storage

https://github.com/bobbae/gcp/wiki/Kubernetes-Storage

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

<img src="https://d1jnx9ba8s6j9r.cloudfront.net/blog/wp-content/uploads/2018/08/29.png" width="600">

## Configuration as Data

[https://cloud.google.com/blog/products/containers-kubernetes/understanding-configuration-as-data-in-kubernetes](https://cloud.google.com/blog/products/containers-kubernetes/understanding-configuration-as-data-in-kubernetes)


## Binary Authorizations

Binary Authorization is a service on Google Cloud that provides software supply-chain security for container-based applications. Binary Authorization extends Google Kubernetes Engine (GKE) and Anthos clusters on VMware with deploy time enforcement of security policies. On Anthos clusters on VMware, Binary Authorization extends this policy enforcement to hybrid-cloud architectures. Binary Authorization works with container images from Container Registry, Artifact Registry and other container image registries.

With Binary Authorization, you can automatically check each component of your software supply chain, ensuring the quality and integrity of your software before an application is deployed to your production environment.

[https://cloud.google.com/binary-authorization/docs/overview](https://cloud.google.com/binary-authorization/docs/overview)


## Scaling

https://github.com/bobbae/gcp/wiki/Kubernetes-scaling

## Federation

Multiple Kubernetes clusters can be managed as a single cluster with the help of federated clusters. So, you can create multiple Kubernetes clusters within a data center/cloud and use federation to control/manage them all at one place.

<img src="https://d1jnx9ba8s6j9r.cloudfront.net/blog/wp-content/uploads/2018/08/30.png" width="600">

https://github.com/kubernetes-sigs/kubefed

<img src="https://github.com/kubernetes-sigs/kubefed/raw/master/docs/images/concepts.png" width="600">

## Workflow

<img src="https://miro.medium.com/max/1575/1*HFUAAjfQo4ZeJVKPSObgZg.png" width="600">

https://faun.pub/workflow-for-kubernetes-devops-15f0dbb560ff

## Qwiklabs

https://github.com/bobbae/gcp/wiki/Kubernetes-Qwiklabs