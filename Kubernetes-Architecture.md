
[Kubernetes]( kubernetes  ) is a portable, extensible, open-source platform for managing [containerized](Containers) workloads and services, that facilitates both declarative configuration and automation. 

https://cloud.google.com/kubernetes-engine/kubernetes-comic

## Kubernetes Cluster Architecture

https://kubernetes.io/docs/concepts/architecture/


A [Kubernetes cluster](  https://kubernetes.io/docs/tasks/administer-cluster/   ) consists of the components that represent the [control plane](https://kubernetes.io/docs/concepts/architecture/control-plane-node-communication/) and a set of machines called [nodes](https://kubernetes.io/docs/concepts/architecture/nodes/).

The [Kubernetes API]( https://kubernetes.io/docs/concepts/overview/kubernetes-api/   ) lets you query and manipulate the state of [objects in Kubernetes](https://kubernetes.io/docs/concepts/overview/working-with-objects/). 

The core of Kubernetes' control plane is the [API server](https://kubernetes.io/docs/reference/command-line-tools-reference/kube-apiserver/) and the HTTP API that it exposes. Users, the different parts of your cluster, and external components all communicate with one another through the API server.

Kubernetes [objects](  https://kubernetes.io/docs/concepts/overview/working-with-objects/kubernetes-objects/  ) are persistent entities in the Kubernetes system. Kubernetes uses these entities to represent the state of your cluster. Learn about the Kubernetes object model and how to work with these objects.

https://kubernetes.io/docs/concepts/architecture/

## Components

https://kubernetes.io/docs/concepts/overview/components/

## Networking

[Kubernetes Networking](Kubernetes-Networking)  model supports different types of open source implementations. Kubernetes provides an IP address to each pod so that there is no need to map host ports to container ports as in the [Docker networking model](https://docs.docker.com/network/). Pods behave much like VMs or physical hosts with respect to port allocation, naming, load balancing and application configuration. 




## Kubernetes features

https://www.guru99.com/kubernetes-tutorial.html


## Cattle vs. Pets

http://cloudscaling.com/blog/cloud-computing/the-history-of-pets-vs-cattle/

## Nodes


Kubernetes runs your workload by placing containers into Pods to run on [Nodes](https://kubernetes.io/docs/concepts/architecture/nodes/
). A node may be a virtual or physical machine, depending on the cluster. Each node is managed by the control plane and contains the services necessary to run Pods

Typically you have several nodes in a cluster; in a learning or resource-limited environment, you might have only one node.




## Pods


https://kubernetes.io/docs/concepts/workloads/pods/

[Pods](https://kubernetes.io/docs/concepts/workloads/pods/
) are the smallest deployable units of computing that you can create and manage in Kubernetes.

https://medium.com/google-cloud/understanding-kubernetes-networking-pods-7117dd28727

A Pod (as in a pod of whales or pea pod) is a group of one or more containers, with shared storage and network resources, and a specification for how to run the containers. A Pod's contents are always co-located and co-scheduled, and run in a shared context. A Pod models an application-specific "logical host": it contains one or more application containers which are relatively tightly coupled. In non-cloud contexts, applications executed on the same physical or virtual machine are analogous to cloud applications executed on the same logical host.




## Control Plane


Kubernetes has a "hub-and-spoke" API pattern. All API usage from nodes (or the pods they run) terminates at the apiserver. None of the other control plane components are designed to expose remote services. The apiserver is configured to listen for remote connections on a secure HTTPS port (typically 443) with one or more forms of client authentication enabled. One or more forms of authorization should be enabled, especially if anonymous requests or service account tokens are allowed.

https://kubernetes.io/docs/concepts/architecture/control-plane-node-communication/

## Controller 


In Kubernetes, [controllers are control loops](https://kubernetes.io/docs/concepts/architecture/controller/
) that watch the state of your cluster, then make or request changes where needed. Each controller tries to move the current cluster state closer to the desired state.


## Cloud Controller Manager

The [cloud-controller-manager](https://kubernetes.io/docs/concepts/architecture/cloud-controller/) is a Kubernetes control plane component that embeds cloud-specific control logic. The cloud controller manager lets you link your cluster into your cloud provider's API, and separates out the components that interact with that cloud platform from components that only interact with your cluster.

By decoupling the interoperability logic between Kubernetes and the underlying cloud infrastructure, the cloud-controller-manager component enables cloud providers to release features at a different pace compared to the main Kubernetes project.





## Components

A Kubernetes cluster consists of a set of worker machines, called nodes, that run containerized applications. Every cluster has at least one worker node.

The worker node(s) host the Pods that are the components of the application workload. The control plane manages the worker nodes and the Pods in the cluster. In production environments, the control plane usually runs across multiple computers and a cluster usually runs multiple nodes, providing fault-tolerance and high availability.


https://kubernetes.io/docs/concepts/overview/components/

### etcd

https://kubernetes.io/docs/concepts/overview/components/#etcd


Consistent and highly-available key value store used as Kubernetes' backing store for all cluster data.

If your Kubernetes cluster uses etcd as its backing store, make sure you have a back up plan for those data.


### kube-controller-manager

Control plane component that runs controller processes.

Logically, each controller is a separate process, but to reduce complexity, they are all compiled into a single binary and run in a single process.



https://kubernetes.io/docs/concepts/overview/components/#kube-controller-manager

### cloud-controller-manager


A Kubernetes control plane component that embeds cloud-specific control logic. The cloud controller manager lets you link your cluster into your cloud provider's API, and separates out the components that interact with that cloud platform from components that only interact with your cluster.

The cloud-controller-manager only runs controllers that are specific to your cloud provider. If you are running Kubernetes on your own premises, or in a learning environment inside your own PC, the cluster does not have a cloud controller manager.



https://kubernetes.io/docs/concepts/overview/components/#cloud-controller-manager

### Kubelet

An agent that runs on each node in the cluster. It makes sure that containers are running in a Pod.

https://kubernetes.io/docs/concepts/overview/components/#kubelet

#### Virtual Kubelet

https://github.com/virtual-kubelet/virtual-kubelet

### kube-proxy

[kube-proxy](https://kubernetes.io/docs/concepts/overview/components/#kube-proxy
) is a network proxy that runs on each node in your cluster, implementing part of the Kubernetes Service concept.




### cluster DNS

[Cluster DNS](https://kubernetes.io/docs/concepts/services-networking/dns-pod-service/
) is a DNS server, in addition to the other DNS server(s) in your environment, which serves DNS records for Kubernetes services.

Containers started by Kubernetes automatically include this DNS server in their DNS searches.




### resource monitoring

To scale an application and provide a reliable service, you need to understand how the application behaves when it is deployed. You can examine application performance in a Kubernetes cluster by examining the containers, pods, services, and the characteristics of the overall cluster. Kubernetes provides detailed information about an application's resource usage at each of these levels. This information allows you to evaluate your application's performance and where bottlenecks can be removed to improve overall performance.

In Kubernetes, application monitoring does not depend on a single monitoring solution. On new clusters, you can use resource metrics or full metrics pipelines to collect monitoring statistics.


https://kubernetes.io/docs/tasks/debug-application-cluster/resource-usage-monitoring/

### kube-scheduler

Control plane component that watches for newly created Pods with no assigned node, and selects a node for them to run on.

https://kubernetes.io/docs/concepts/scheduling-eviction/kube-scheduler/



## Cluster Administration

https://kubernetes.io/docs/concepts/cluster-administration/


## Resource Limits

When you specify a Pod, you can optionally specify how much of each resource a Container needs. The most common resources to specify are CPU and memory (RAM); there are others.

When you specify the resource request for Containers in a Pod, the scheduler uses this information to decide which node to place the Pod on. When you specify a resource limit for a Container, the [kubelet](https://kubernetes.io/docs/reference/command-line-tools-reference/kubelet/) enforces those limits so that the running container is not allowed to use more of that resource than the limit you set. The kubelet also reserves at least the request amount of that system resource specifically for that container to use.

## Requests and limits 

If the node where a Pod is running has enough of a resource available, it's possible (and allowed) for a container to use more resource than its request for that resource specifies. However, a container is not allowed to use more than its resource limit.

[https://www.youtube.com/watch?v=xjpHggHKm78&list=PLIivdWyY5sqL3xfXz5xJvwzFW_tlQB_GB&index=4](https://www.youtube.com/watch?v=xjpHggHKm78&list=PLIivdWyY5sqL3xfXz5xJvwzFW_tlQB_GB&index=4)


## RBAC

Role-based access control (RBAC) is a method of regulating access to computer or network resources based on the roles of individual users within your organization.

RBAC authorization uses the rbac.authorization.k8s.io API group to drive authorization decisions, allowing you to dynamically configure policies through the Kubernetes API.

[https://www.youtube.com/watch?v=4HMRFcg6nEY](https://www.youtube.com/watch?v=4HMRFcg6nEY)

## Workload Resources


https://kubernetes.io/docs/concepts/workloads/controllers/

### Deployment & Service

A [Deployment](https://kubernetes.io/docs/concepts/workloads/controllers/deployment/) provides declarative updates for Pods and [ReplicaSets](https://kubernetes.io/docs/concepts/workloads/controllers/replicaset/).

You describe a desired state in a Deployment, and the Deployment Controller changes the actual state to the desired state at a controlled rate. You can define Deployments to create new ReplicaSets, or to remove existing Deployments and adopt all their resources with new Deployments.

A [Service](https://kubernetes.io/docs/concepts/services-networking/service/) is an abstract way to expose an application running on a set of Pods as a network service.
With Kubernetes you don't need to modify your application to use an unfamiliar service discovery mechanism. Kubernetes gives Pods their own IP addresses and a single DNS name for a set of Pods, and can [load-balance](https://kubernetes.io/docs/concepts/services-networking/) across them


[https://www.youtube.com/watch?v=qmDzcu5uY1I](https://www.youtube.com/watch?v=qmDzcu5uY1I)

https://kubernetes.io/docs/concepts/services-networking/connect-applications-service/

### Stateful Sets

[StatefulSet](https://kubernetes.io/docs/concepts/workloads/controllers/statefulset/) is the workload API object used to manage stateful applications.



[https://www.youtube.com/watch?v=pPQKAR1pA9U](https://www.youtube.com/watch?v=pPQKAR1pA9U)






https://kubernetes.io/docs/concepts/workloads/controllers/statefulset/


### DaemonSet

A [DaemonSet](https://kubernetes.io/docs/concepts/workloads/controllers/daemonset/) ensures that all (or some) Nodes run a copy of a Pod. As nodes are added to the cluster, Pods are added to them. As nodes are removed from the cluster, those Pods are garbage collected. Deleting a DaemonSet will clean up the Pods it created.

[https://kubernetes.io/docs/concepts/workloads/controllers/daemonset/](https://kubernetes.io/docs/concepts/workloads/controllers/daemonset/)

Some typical uses of a DaemonSet are:

* running a cluster storage daemon on every node
* running a logs collection daemon on every node
* running a node monitoring daemon on every node




https://kubernetes.io/docs/concepts/workloads/controllers/daemonset/

### ReplicaSet

A [ReplicaSet](https://kubernetes.io/docs/concepts/workloads/controllers/replicaset/
) maintains a stable set of replica Pods running at any given time. As such, it is often used to guarantee the availability of a specified number of identical Pods.




#### Alternative to ReplicaSets


https://kubernetes.io/docs/concepts/workloads/controllers/replicaset/#alternatives-to-replicaset

## Configmaps & Secrets

A [ConfigMap]( https://kubernetes.io/docs/concepts/configuration/configmap/   ) is an API object used to store non-confidential data in key-value pairs. Pods can consume ConfigMaps as environment variables, command-line arguments, or as configuration files in a volume.



Kubernetes [Secrets](   https://kubernetes.io/docs/concepts/configuration/secret/  ) let you store and manage sensitive information, such as passwords, OAuth tokens, and ssh keys.



[https://www.youtube.com/watch?v=FAnQTgr04mU](https://www.youtube.com/watch?v=FAnQTgr04mU)

#### Secret encryption

https://kubernetes.io/docs/tasks/administer-cluster/encrypt-data/


### Replication Controller

A [ReplicationController](https://kubernetes.io/docs/concepts/workloads/controllers/replicationcontroller/
) ensures that a specified number of pod replicas are running at any one time. In other words, a ReplicationController makes sure that a pod or a homogeneous set of pods is always up and available.


### Alternatives to ReplicationController

https://kubernetes.io/docs/concepts/workloads/controllers/replicationcontroller/#alternatives-to-replicationcontroller

ReplicaSet is the next-generation ReplicationController that supports the new set-based label selector. It's mainly used by Deployment as a mechanism to orchestrate pod creation, deletion and updates. 

Use Deployments instead of directly using Replica Sets, unless you require custom update orchestration or don't require updates at all.

### Jobs

A [Job](https://kubernetes.io/docs/concepts/workloads/controllers/job/
) creates one or more Pods and will continue to retry execution of the Pods until a specified number of them successfully terminate. 

As pods successfully complete, the Job tracks the successful completions. When a specified number of successful completions is reached, the task (ie, Job) is complete. 

Deleting a Job will clean up the Pods it created. 

Suspending a Job will delete its active Pods until the Job is resumed again.


Jobs are complementary to Replication Controllers. A Replication Controller manages Pods which are not expected to terminate (e.g. web servers), and a Job manages Pods that are expected to terminate (e.g. batch tasks).



Job is only appropriate for pods with RestartPolicy equal to OnFailure or Never. (Note: If RestartPolicy is not set, the default value is Always.)

#### Cron Jobs

You can use a [CronJob](https://kubernetes.io/docs/concepts/workloads/controllers/cron-jobs/
) to create a Job that will run at specified times/dates, similar to the Unix tool cron.

A CronJob creates Jobs on a repeating schedule.

One CronJob object is like one line of a crontab (cron table) file. It runs a job periodically on a given schedule, written in Cron format.



Cron jobs are useful for creating periodic and recurring tasks, like running backups or sending emails. Cron jobs can also schedule individual tasks for a specific time, such as if you want to schedule a job for a low activity period.

Cron jobs have limitations and idiosyncrasies. For example, in certain circumstances, a single cron job can create multiple jobs. Therefore, jobs should be idempotent.


https://kubernetes.io/docs/tasks/job/automated-tasks-with-cron-jobs/

## CRD


[CRD](https://kubernetes.io/docs/tasks/extend-kubernetes/custom-resources/custom-resource-definitions/) stands for  Custom Resource Definition.

https://insujang.github.io/2020-02-13/programming-kubernetes-crd/

A resource is an endpoint in the [Kubernetes API](https://kubernetes.io/docs/reference/using-api/api-overview/) that stores a collection of [API objects](https://kubernetes.io/docs/concepts/overview/working-with-objects/kubernetes-objects/) of a certain kind; for example, the built-in pods resource contains a collection of Pod objects.

https://itnext.io/building-your-own-kubernetes-crds-701de1c9a161


A custom resource is an extension of the Kubernetes API that is not necessarily available in a default Kubernetes installation. 

It represents a customization of a particular Kubernetes installation. 

However, many core Kubernetes functions are now built using custom resources, making Kubernetes more modular. 

Custom resources can appear and disappear in a running cluster through dynamic registration, and cluster admins can update custom resources independently of the cluster itself. 


Once a custom resource is installed, users can create and access its objects using [kubectl](https://kubernetes.io/docs/reference/kubectl/overview/), just as they do for built-in resources like Pods.

[https://kubernetes.io/docs/concepts/extend-kubernetes/api-extension/custom-resources/](https://kubernetes.io/docs/concepts/extend-kubernetes/api-extension/custom-resources/)


[Kubebuilder](https://github.com/kubernetes-sigs/kubebuilder
) is a framework for building Kubernetes APIs using custom resource definitions (CRDs).

https://book.kubebuilder.io/quick-start.html



## Operator Pattern


In Kubernetes, objects are analogous to a job or a completed task in the real world. You can use them to define common tasks, store them in a version control system, and apply them with [kubectl](https://kubernetes.io/docs/tasks/tools/) apply. Kubernetes ensures that this triggers everything necessary to bring your declarative description to life by creating the dependent resources (like pods) to run your software. Kubernetes contains a number of built-in object types that can be created with this workflow, like Deployments and Services. 


With [Operators](https://kubernetes.io/docs/concepts/extend-kubernetes/operator/), Kubernetes allows cluster maintainers or software providers to define their own Kubernetes object types, called custom resource definitions (CRDs). These objects can be handled by the Kubernetes API, just like built-in object types. Inside the Operator code, authors can define how to act on those custom objects. 


[Operators](https://www.youtube.com/watch?v=ha3LjlD6g7g) are software extensions to Kubernetes that make use of [custom resources](https://kubernetes.io/docs/concepts/extend-kubernetes/api-extension/custom-resources/) to manage applications and their components. Operators follow Kubernetes principles, notably the [control loop](https://kubernetes.io/docs/concepts/architecture/controller).

https://blog.container-solutions.com/kubernetes-operators-explained

Operators make it easy to manage complex state-ful applications on top of Kubernetes. 

[https://kubernetes.io/docs/concepts/extend-kubernetes/operator/](https://kubernetes.io/docs/concepts/extend-kubernetes/operator/)

The Operator SDK is a framework that uses the controller-runtime library to make writing operators easier by providing:

* High level APIs and abstractions to write the operational logic more intuitively
* Tools for scaffolding and code generation to bootstrap a new project fast
* Extensions to cover common Operator use cases

https://github.com/operator-framework/operator-sdk
 
[https://opensource.com/article/20/3/kubernetes-operator-sdk](https://opensource.com/article/20/3/kubernetes-operator-sdk)

[Shell-operator](https://github.com/flant/shell-operator
) is a tool for running event-driven scripts in a Kubernetes cluster.



[Kubernetes Universal Declarative Operator](https://d2iq.com/products/kudo
) (KUDO) provides a declarative approach to building production-grade Kubernetes operators. 


### Operator Hub

OperatorHub.io is a home for the Kubernetes community to share Operators.

[https://operatorhub.io/](https://operatorhub.io/)



### Operator Sprawl

[https://thenewstack.io/the-runaway-problem-of-kubernetes-operators-and-dependency-lifecycles/](https://thenewstack.io/the-runaway-problem-of-kubernetes-operators-and-dependency-lifecycles/)


## Certificates Manager

https://cert-manager.io/

## Krew

[Krew](  https://krew.sigs.k8s.io/  ) is the plugin manager for kubectl command-line tool.

https://krew.sigs.k8s.io/docs/user-guide/setup/install/



## Garbage Collection

Garbage collection is a collective term for the various mechanisms Kubernetes uses to clean up cluster resources. 

https://kubernetes.io/docs/concepts/architecture/garbage-collection/



## Add-ons

Add-ons extend the functionality of Kubernetes.

https://kubernetes.io/docs/concepts/cluster-administration/addons/


## JSONPATH

[JSONPath](JSONPath) is a query language for JSON, similar to XPath for XML. 

[Kubectl](https://kubernetes.io/docs/reference/kubectl/) supports JSONPath template.

JSONPath template is composed of JSONPath expressions enclosed by curly braces {}. Kubectl uses JSONPath expressions to filter on specific fields in the JSON object and format the output. 

https://kubernetes.io/docs/reference/kubectl/jsonpath/

## Bootstrapping a Kubernetes cluster using kubeadm

https://kubernetes.io/docs/setup/production-environment/tools/kubeadm/



## Awesome links for Kubernetes

[https://github.com/ramitsurana/awesome-kubernetes](https://github.com/ramitsurana/awesome-kubernetes)


## Examples

### Online boutique micro services in GKE

https://github.com/GoogleCloudPlatform/microservices-demo

