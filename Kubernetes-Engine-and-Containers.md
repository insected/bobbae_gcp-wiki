

## Containers

Typical [Containers](Containers)  like [Docker](https://docker.io) make use of [Namespaces](Namespaces) features in the Linux kernel.

## Kubernetes



[Kubernetes](https://kubernetes.io) is an open-source container-orchestration system for automating computer application deployment, scaling, and management. It was originally [designed by Google](https://www.youtube.com/watch?v=pQ87vVMZK-A)  and is now maintained by the Cloud Native Computing Foundation.



Kubernetes objects can quickly be created, updated, and deleted directly using imperative commands built into the kubectl command-line tool. 

<img src="http://www.aquasec.com/wp-content/uploads/2020/11/Kubernetes-101-Architecture-Diagram.jpg" width="700">


A Kubernetes cluster consists of a set of worker machines, called nodes, that run containerized applications. Every cluster has at least one worker node.



[Kubernetes](https://en.wikipedia.org/wiki/Kubernetes) is an open source container orchestration engine for automating deployment, scaling, and management of containerized applications. 


[Kubernetes](https://www.youtube.com/watch?v=X48VuDVv0do) is a portable, extensible, open-source platform for managing [containerized workloads and services](https://www.youtube.com/watch?v=cC46cg5FFAM&list=PLIivdWyY5sqLmnGdKSdQIXq2sd_1bWSnx), that facilitates both [declarative configuration](https://www.youtube.com/watch?v=qmDzcu5uY1I) and automation. It has a large, rapidly growing ecosystem. Kubernetes services, support, and tools are widely available.




[Kubernetes](https://cloud.google.com/learn/what-is-kubernetes) API lets you query and manipulate the state of objects in Kubernetes. The core of Kubernetes' control plane is the API server and the HTTP API that it exposes. Users, the different parts of your cluster, and external components all communicate with one another through the API server.




## GKE

[GKE](GKE) provides a managed environment for deploying, managing, and scaling your containerized applications using Google infrastructure. The GKE environment consists of multiple machines (specifically, Compute Engine instances) grouped together to form a cluster.

[GKE](https://www.youtube.com/watch?v=Rl5M1CzgEH4) clusters are powered by the Kubernetes open source cluster management system. Kubernetes provides the mechanisms through which you interact with your cluster. You use Kubernetes commands and resources to deploy and manage your applications, perform administration tasks, set policies, and monitor the health of your deployed workloads.

[GKE](GKE) is Secured and fully managed Kubernetes service with revolutionary autopilot mode of operation.


## Kubernetes Control Plane

<img src="https://d33wubrfki0l68.cloudfront.net/d35c2b375b43b4fa374ae834f95224975418e33f/6b47b/images/blog/2018-06-05-11-ways-not-to-get-hacked/kubernetes-control-plane.png" width="600">

A [Kubernetes cluster](https://kubernetes.io/docs/concepts/overview/components/) consists of a set of worker machines, called nodes, that run containerized applications. [Every cluster](https://www.youtube.com/watch?v=Krpb44XR0bk) has at least one worker node.

The worker node(s) host the Pods that are the components of the application workload. The control plane manages the worker nodes and the Pods in the cluster. In production environments, the control plane usually runs across multiple computers and a cluster usually runs multiple nodes, providing fault-tolerance and high availability.



## API

The core of Kubernetes' control plane is the [API](https://kubernetes.io/docs/concepts/overview/kubernetes-api/) server. The API server exposes an HTTP API that lets end users, different parts of your cluster, and external components communicate with one another.

The Kubernetes API lets you query and manipulate the state of API objects in Kubernetes (for example: Pods, Namespaces, ConfigMaps, and Events).

Most operations can be performed through the kubectl command-line interface or other command-line tools, such as kubeadm, which in turn use the API. However, you can also access the API directly using REST calls.

Consider using one of the client libraries if you are writing an application using the Kubernetes API.



## Objects

A Kubernetes [object](https://kubernetes.io/docs/concepts/overview/working-with-objects/) is a "record of intent"--once you create the object, the Kubernetes system will constantly work to ensure that object exists. By creating an object, you're effectively telling the Kubernetes system what you want your cluster's workload to look like; this is your cluster's desired state.



## Kubectl

The Kubernetes command-line tool, [kubectl](https://kubernetes.io/docs/reference/kubectl/kubectl/), allows you to run commands against Kubernetes clusters. You can use [kubectl](https://www.youtube.com/watch?v=azuwXALfyRg) to deploy applications, inspect and manage cluster resources, and view logs. For a complete list of kubectl operations, see [Overview of kubectl](https://kubernetes.io/docs/reference/kubectl/overview/).



### Kustomize

<img src="https://miro.medium.com/max/1575/1*qZV6wiQr4yet746qAl-G7A.png" width="600">

[Kustomize](https://kustomize.io/) introduces a [template-free way](https://itnext.io/helm-is-not-enough-you-also-need-kustomize-82bae896816e) to [customize application configuration]((https://www.youtube.com/watch?v=uvH84BviDS4)) that simplifies the use of off-the-shelf applications. Now, built into `kubectl as apply -k`.






## Kubernetes Details

[Kubernetes is influenced](Kubernetes-Origin)  by Borg, Omega and other systems.  You should check out various
[Kubernetes Examples](Kubernetes-Examples) to learn more about [Kubernetes Architecture](Kubernetes-Architecture).




[Kubernetes Networking](Kubernetes-Networking) can be complicated but it is worth studying in depth.


As Kubernetes evolved the support for [Stateful Applications](https://thenewstack.io/the-evolution-of-stateful-applications-on-kubernetes/) the
[Kubernetes Storage](Kubernetes-Storage) architecture has evolved over time.

## Authentication and Authorization in Kubernetes

[https://www.youtube.com/watch?v=dAUJ3TBwDWo](https://www.youtube.com/watch?v=dAUJ3TBwDWo)

## Ingress

Kubernetes [Ingress](Ingress) may provide load balancing, SSL termination and name-based virtual hosting.


Ingress exposes HTTP and HTTPS routes from outside the cluster to services within the cluster. Traffic routing is controlled by rules defined on the Ingress resource.



## Service Mesh

Kubernetes [Service Mesh](Service-Mesh) is configurable infrastructure layer for a microservices application.


## Cloud Build & Cloud Code with Containers

[Cloud Build](Cloud-Build) provides a `gke-deploy` builder that enables you to deploy a containerized application to a GKE cluster.


## K8s monitoring

There are many [Kubernetes Monitoring](Kubernetes-Monitoring) tools.

<img src="https://d1jnx9ba8s6j9r.cloudfront.net/blog/wp-content/uploads/2018/08/29.png" width="600">

## Configuration as Data

[https://cloud.google.com/blog/products/containers-kubernetes/understanding-configuration-as-data-in-kubernetes](https://cloud.google.com/blog/products/containers-kubernetes/understanding-configuration-as-data-in-kubernetes)


## Binary Authorizations

[Binary Authorization](https://cloud.google.com/binary-authorization/docs/overview) is a service on Google Cloud that provides software supply-chain security for container-based applications. Binary Authorization extends Google Kubernetes Engine (GKE) and Anthos clusters on VMware with deploy time enforcement of security policies. On Anthos clusters on VMware, Binary Authorization extends this policy enforcement to hybrid-cloud architectures. Binary Authorization works with container images from Container Registry, Artifact Registry and other container image registries.

With Binary Authorization, you can automatically check each component of your software supply chain, ensuring the quality and integrity of your software before an application is deployed to your production environment.

## Stateless Applications

https://kubernetes.io/docs/tutorials/stateless-application/


## Stateful Apps

https://kubernetes.io/docs/tutorials/stateful-application/

## Scaling

[Kubernetes Scaling](Kubernetes-scaling) has evolved over time to include VPA and HPA.

## Federation

[Multiple Kubernetes clusters can be managed as a single cluster](https://github.com/kubernetes-sigs/kubefed) with the help of federated clusters. So, you can create multiple Kubernetes clusters within a data center/cloud and use federation to control/manage them all at one place.

<img src="https://d1jnx9ba8s6j9r.cloudfront.net/blog/wp-content/uploads/2018/08/30.png" width="600">



<img src="https://github.com/kubernetes-sigs/kubefed/raw/master/docs/images/concepts.png" width="600">

## Kubernetes & AI

Kubernetes has [awesome](https://github.com/CognonicLabs/awesome-AI-kubernetes) support and integration with AI [Workflows](Workflows) such as [Kubeflow](Kubeflow).

## Kubernetes & GitOps



Kubernetes supports various [Workflows](Workflows) for [DevOps](DevOps) as discussed [here](https://faun.pub/workflow-for-kubernetes-devops-15f0dbb560ff).

It is possible to support [GitOps CICD](https://itnext.io/continuous-gitops-the-way-to-do-devops-in-kubernetes-896b0ea1d0fb) in Kubernetes.

## Tutorials

https://kubernetes.io/docs/tutorials/


## Qwiklabs

There are many interesting [Kubernetes Qwiklabs](Kubernetes-Qwiklabs).