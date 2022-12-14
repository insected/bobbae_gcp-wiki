

## Containers

Typical [Containers](Containers)  like [Docker](https://docker.io) make use of [Namespaces](Namespaces) and [CGroups](https://en.wikipedia.org/wiki/Cgroups) features in the Linux kernel.

## Kubernetes



[Kubernetes](https://kubernetes.io) is an open-source container-orchestration system for automating computer application deployment, scaling, and management. It was [originally](https://cloud.google.com/blog/products/containers-kubernetes/from-google-to-the-world-the-kubernetes-origin-story) [designed by Google](https://www.youtube.com/watch?v=pQ87vVMZK-A)  and is now maintained by the Cloud Native Computing Foundation.



[Kubernetes is influenced](Kubernetes-Origin)  by Borg, Omega and other systems.  You should check out various
[Kubernetes Examples](Kubernetes-Examples) to learn more about [Kubernetes Architecture](Kubernetes-Architecture).

[Kubernetes Networking](Kubernetes-Networking) implements flat pod networking where pods in the host network of a node can communicate with all pods on all nodes without NAT.  This model enables low-friction porting of apps from VMs to containers. 

[As Kubernetes evolved](https://medium.com/swlh/kubernetes-the-evolution-of-a-technology-revolution-805302172ea6) the support for [Stateful Applications](https://blog.min.io/kubernetes-storage-patterns/) the
[Kubernetes Storage](Kubernetes-Storage) architecture has evolved over time.


[Kubernetes objects](https://kubernetes.io/docs/concepts/overview/working-with-objects/kubernetes-objects/) can quickly be created, updated, and deleted directly using imperative commands built into the [kubectl](https://kubernetes.io/docs/reference/kubectl/overview/) command-line tool. 



A [Kubernetes](https://en.wikipedia.org/wiki/Kubernetes) cluster consists of a set of worker machines, called nodes, that run containerized applications. Every cluster has at least one worker node. 




[Kubernetes](https://www.youtube.com/watch?v=X48VuDVv0do) is a portable, extensible, open-source platform for managing [containerized workloads and services](https://www.youtube.com/watch?v=cC46cg5FFAM&list=PLIivdWyY5sqLmnGdKSdQIXq2sd_1bWSnx), that facilitates both [declarative configuration](https://www.youtube.com/watch?v=qmDzcu5uY1I) and automation. 



## KubeVirt


[KubeVirt]( https://kubevirt.io/   ) technology addresses the needs of development teams that have adopted or want to adopt Kubernetes but possess existing Virtual Machine-based workloads that cannot be easily containerized. 


## Minikube

https://github.com/bobbae/gcp/wiki/Minikube,-Kind,-K3S

## GKE

[GKE](GKE) provides a managed environment for deploying, managing, and scaling your containerized applications using Google infrastructure. The GKE environment consists of multiple machines (specifically, Compute Engine instances) grouped together to form a cluster.

[GKE](https://www.youtube.com/watch?v=Rl5M1CzgEH4) clusters are powered by the Kubernetes open source cluster management system. Kubernetes provides the mechanisms through which you interact with your cluster. You use Kubernetes commands and resources to deploy and manage your applications, perform administration tasks, set policies, and monitor the health of your deployed workloads.

[GKE](GKE) is Secured and fully managed Kubernetes service with revolutionary autopilot mode of operation.


## Kubernetes Control Plane


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

The Kubernetes command-line tool, [kubectl](Kubectl), allows you to run commands against Kubernetes clusters. 



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





## Kubernetes & AI

Kubernetes has [awesome](https://github.com/CognonicLabs/awesome-AI-kubernetes) support and integration with AI [Workflows](Workflows) such as [Kubeflow](Kubeflow).

## Kubernetes & GitOps



Kubernetes supports various [Workflows](Workflows) for [DevOps](DevOps) as discussed [here](https://faun.pub/workflow-for-kubernetes-devops-15f0dbb560ff).

It is possible to support [GitOps CICD](https://itnext.io/continuous-gitops-the-way-to-do-devops-in-kubernetes-896b0ea1d0fb) in Kubernetes.

## Kubernetes Security

https://kubernetes.io/docs/concepts/security/overview/


## Tutorials

https://kubernetes.io/docs/tutorials/


## Qwiklabs

There are many interesting [Kubernetes Qwiklabs](Kubernetes-Qwiklabs).