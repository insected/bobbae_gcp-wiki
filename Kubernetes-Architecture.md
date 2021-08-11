
Kubernetes is a portable, extensible, open-source platform for managing containerized workloads and services, that facilitates both declarative configuration and automation. It has a large, rapidly growing ecosystem. Kubernetes services, support, and tools are widely available.

## Kubernetes Cluster Architecture

A Kubernetes cluster consists of the components that represent the control plane and a set of machines called nodes.

The Kubernetes API lets you query and manipulate the state of objects in Kubernetes. The core of Kubernetes' control plane is the API server and the HTTP API that it exposes. Users, the different parts of your cluster, and external components all communicate with one another through the API server.

Kubernetes objects are persistent entities in the Kubernetes system. Kubernetes uses these entities to represent the state of your cluster. Learn about the Kubernetes object model and how to work with these objects.

https://kubernetes.io/docs/concepts/architecture/

<img src="https://d1jnx9ba8s6j9r.cloudfront.net/blog/wp-content/uploads/2018/08/16-1.png" width="600">

## Kubernetes features

Kubernetes progressively rolls out changes to your application or its configuration, while monitoring application health to ensure it doesn't kill all your instances at the same time. If something goes wrong, Kubernetes will rollback the change for you. 

Restarts containers that fail, replaces and reschedules containers when nodes die, kills containers that don't respond to your user-defined health check, and doesn't advertise them to clients until they are ready to serve.

Deploy and update secrets and application configuration without rebuilding your image and without exposing secrets in your stack configuration.

Scale your application up and down with a simple command, with a UI, or automatically based on CPU usage.

In addition to services, Kubernetes can manage your batch and CI workloads, replacing containers that fail, if desired.

Kubernetes gives Pods their own IP addresses and a single DNS name for a set of Pods, and can load-balance across them.

Automatically places containers based on their resource requirements and other constraints, while not sacrificing availability. Mix critical and best-effort workloads in order to drive up utilization and save even more resources.

Allocation of IPv4 and IPv6 addresses to Pods and Services.

Automatically mount the storage system of your choice, whether from local storage, a public cloud provider such as GCP or AWS, or a network storage system such as NFS, iSCSI, Gluster, Ceph, Cinder, or Flocker.


Add features to your Kubernetes cluster without changing upstream source code.

<img src="https://d1jnx9ba8s6j9r.cloudfront.net/blog/wp-content/uploads/2018/08/7.png" width="600">

## Cattle vs. Pets

http://cloudscaling.com/blog/cloud-computing/the-history-of-pets-vs-cattle/

## Nodes

<img src="https://d1jnx9ba8s6j9r.cloudfront.net/blog/wp-content/uploads/2018/08/15-1.png" width="500">


Kubernetes runs your workload by placing containers into Pods to run on Nodes. A node may be a virtual or physical machine, depending on the cluster. Each node is managed by the control plane and contains the services necessary to run Pods

Typically you have several nodes in a cluster; in a learning or resource-limited environment, you might have only one node.

<img src="https://d1jnx9ba8s6j9r.cloudfront.net/blog/wp-content/uploads/2018/08/18-1.png" width="600">

## Pods

Pods are the smallest deployable units of computing that you can create and manage in Kubernetes.

https://medium.com/google-cloud/understanding-kubernetes-networking-pods-7117dd28727

A Pod (as in a pod of whales or pea pod) is a group of one or more containers, with shared storage and network resources, and a specification for how to run the containers. A Pod's contents are always co-located and co-scheduled, and run in a shared context. A Pod models an application-specific "logical host": it contains one or more application containers which are relatively tightly coupled. In non-cloud contexts, applications executed on the same physical or virtual machine are analogous to cloud applications executed on the same logical host.

https://kubernetes.io/docs/concepts/workloads/pods/


<!--<img src="https://miro.medium.com/max/1575/1*Ow5A6_zjjwdKkf2Yi1KgYw.png" width="600">-->

## Control Plane

<img src="https://d1jnx9ba8s6j9r.cloudfront.net/blog/wp-content/uploads/2018/08/25-1.png" width="600">

Kubernetes has a "hub-and-spoke" API pattern. All API usage from nodes (or the pods they run) terminates at the apiserver. None of the other control plane components are designed to expose remote services. The apiserver is configured to listen for remote connections on a secure HTTPS port (typically 443) with one or more forms of client authentication enabled. One or more forms of authorization should be enabled, especially if anonymous requests or service account tokens are allowed.


<img src="https://miro.medium.com/max/5400/1*QWJijlj7kwd0hIYk8Wsnow.png" width="600">

## Controller 

In robotics and automation, a control loop is a non-terminating loop that regulates the state of a system.

Here is one example of a control loop: a thermostat in a room.

When you set the temperature, that's telling the thermostat about your desired state. The actual room temperature is the current state. The thermostat acts to bring the current state closer to the desired state, by turning equipment on or off.

In Kubernetes, controllers are control loops that watch the state of your cluster, then make or request changes where needed. Each controller tries to move the current cluster state closer to the desired state.


## Cloud Controller Manager

The [cloud-controller-manager](https://kubernetes.io/docs/concepts/architecture/cloud-controller/) is a Kubernetes control plane component that embeds cloud-specific control logic. The cloud controller manager lets you link your cluster into your cloud provider's API, and separates out the components that interact with that cloud platform from components that only interact with your cluster.

By decoupling the interoperability logic between Kubernetes and the underlying cloud infrastructure, the cloud-controller-manager component enables cloud providers to release features at a different pace compared to the main Kubernetes project.

https://kubernetes.io/docs/concepts/architecture/


<img src="https://miro.medium.com/proxy/1*ax_IkyNCNlNUYY8WKrawaA.png" width="600">

## Networking

[Kubernetes Networking](Kubernetes-Networking)  model supports different types of open source implementations. Kubernetes provides an IP address to each pod so that there is no need to map host ports to container ports as in the Docker networking model. Pods behave much like VMs or physical hosts with respect to port allocation, naming, load balancing and application configuration. 


<img src="https://d1jnx9ba8s6j9r.cloudfront.net/blog/wp-content/uploads/2018/08/Pods.png" width="600">

## Components

A Kubernetes cluster consists of a set of worker machines, called nodes, that run containerized applications. Every cluster has at least one worker node.

The worker node(s) host the Pods that are the components of the application workload. The control plane manages the worker nodes and the Pods in the cluster. In production environments, the control plane usually runs across multiple computers and a cluster usually runs multiple nodes, providing fault-tolerance and high availability.

[[https://d33wubrfki0l68.cloudfront.net/2475489eaf20163ec0f54ddc1d92aa8d4c87c96b/e7c81/images/docs/components-of-kubernetes.svg]]

https://kubernetes.io/docs/concepts/overview/components/

### etcd

https://kubernetes.io/docs/concepts/overview/components/#etcd

<img src="https://superuser.openstack.org/wp-content/uploads/2019/11/etcd-in-Kubernetes.png" width="600">

Consistent and highly-available key value store used as Kubernetes' backing store for all cluster data.

If your Kubernetes cluster uses etcd as its backing store, make sure you have a back up plan for those data.

<img src="https://superuser.openstack.org/wp-content/uploads/2019/11/etcd-in-Kubernetes-2.png" width="600">

### kube-controller-manager

Control plane component that runs controller processes.

Logically, each controller is a separate process, but to reduce complexity, they are all compiled into a single binary and run in a single process.



https://kubernetes.io/docs/concepts/overview/components/#kube-controller-manager

### cloud-controller-manager


A Kubernetes control plane component that embeds cloud-specific control logic. The cloud controller manager lets you link your cluster into your cloud provider's API, and separates out the components that interact with that cloud platform from components that only interact with your cluster.

The cloud-controller-manager only runs controllers that are specific to your cloud provider. If you are running Kubernetes on your own premises, or in a learning environment inside your own PC, the cluster does not have a cloud controller manager.



https://kubernetes.io/docs/concepts/overview/components/#cloud-controller-manager

### kubelet

An agent that runs on each node in the cluster. It makes sure that containers are running in a Pod.

https://kubernetes.io/docs/concepts/overview/components/#kubelet

### kube-proxy

kube-proxy is a network proxy that runs on each node in your cluster, implementing part of the Kubernetes Service concept.



https://kubernetes.io/docs/concepts/overview/components/#kube-proxy

### cluster DNS

Cluster DNS is a DNS server, in addition to the other DNS server(s) in your environment, which serves DNS records for Kubernetes services.

Containers started by Kubernetes automatically include this DNS server in their DNS searches.



https://kubernetes.io/docs/concepts/services-networking/dns-pod-service/

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

When you specify the resource request for Containers in a Pod, the scheduler uses this information to decide which node to place the Pod on. When you specify a resource limit for a Container, the kubelet enforces those limits so that the running container is not allowed to use more of that resource than the limit you set. The kubelet also reserves at least the request amount of that system resource specifically for that container to use.

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

A Deployment provides declarative updates for Pods and ReplicaSets.

You describe a desired state in a Deployment, and the Deployment Controller changes the actual state to the desired state at a controlled rate. You can define Deployments to create new ReplicaSets, or to remove existing Deployments and adopt all their resources with new Deployments.

A Service is an abstract way to expose an application running on a set of Pods as a network service.
With Kubernetes you don't need to modify your application to use an unfamiliar service discovery mechanism. Kubernetes gives Pods their own IP addresses and a single DNS name for a set of Pods, and can load-balance across them


[https://www.youtube.com/watch?v=qmDzcu5uY1I](https://www.youtube.com/watch?v=qmDzcu5uY1I)

https://kubernetes.io/docs/concepts/services-networking/connect-applications-service/

### Stateful Sets

[StatefulSet](https://www.youtube.com/watch?v=pPQKAR1pA9U) is the workload API object used to manage stateful applications.

Manages the deployment and scaling of a set of Pods, and provides guarantees about the ordering and uniqueness of these Pods.

[https://www.youtube.com/watch?v=pPQKAR1pA9U](https://www.youtube.com/watch?v=pPQKAR1pA9U)

Like a Deployment, a StatefulSet manages Pods that are based on an identical container spec. Unlike a Deployment, a StatefulSet maintains a sticky identity for each of their Pods. These pods are created from the same spec, but are not interchangeable: each has a persistent identifier that it maintains across any rescheduling.

If you want to use storage volumes to provide persistence for your workload, you can use a StatefulSet as part of the solution. Although individual Pods in a StatefulSet are susceptible to failure, the persistent Pod identifiers make it easier to match existing volumes to the new Pods that replace any that have failed.


StatefulSets are valuable for applications that require one or more of the following.

- Stable, unique network identifiers.
- Stable, persistent storage.
- Ordered, graceful deployment and scaling.
- Ordered, automated rolling updates.


In the above, stable is synonymous with persistence across Pod (re)scheduling. If an application doesn't require any stable identifiers or ordered deployment, deletion, or scaling, you should deploy your application using a workload object that provides a set of stateless replicas. Deployment or ReplicaSet may be better suited to your stateless needs.

The storage for a given Pod must either be provisioned by a PersistentVolume Provisioner based on the requested storage class, or pre-provisioned by an admin.

Deleting and/or scaling a StatefulSet down will not delete the volumes associated with the StatefulSet. This is done to ensure data safety, which is generally more valuable than an automatic purge of all related StatefulSet resources.

StatefulSets currently require a Headless Service to be responsible for the network identity of the Pods. You are responsible for creating this Service.

StatefulSets do not provide any guarantees on the termination of pods when a StatefulSet is deleted. To achieve ordered and graceful termination of the pods in the StatefulSet, it is possible to scale the StatefulSet down to 0 prior to deletion.

When using Rolling Updates with the default Pod Management Policy (OrderedReady), it's possible to get into a broken state that requires manual intervention to repair.

https://kubernetes.io/docs/concepts/workloads/controllers/statefulset/


### DaemonSet

A DaemonSet ensures that all (or some) Nodes run a copy of a Pod. As nodes are added to the cluster, Pods are added to them. As nodes are removed from the cluster, those Pods are garbage collected. Deleting a DaemonSet will clean up the Pods it created.

[https://kubernetes.io/docs/concepts/workloads/controllers/daemonset/](https://kubernetes.io/docs/concepts/workloads/controllers/daemonset/)

Some typical uses of a DaemonSet are:

* running a cluster storage daemon on every node
* running a logs collection daemon on every node
* running a node monitoring daemon on every node

In a simple case, one DaemonSet, covering all nodes, would be used for each type of daemon. 

A more complex setup might use multiple DaemonSets for a single type of daemon, but with different flags and/or different memory and cpu requests for different hardware types.


https://kubernetes.io/docs/concepts/workloads/controllers/daemonset/

### ReplicaSet

A ReplicaSet's purpose is to maintain a stable set of replica Pods running at any given time. As such, it is often used to guarantee the availability of a specified number of identical Pods.

A ReplicaSet ensures that a specified number of pod replicas are running at any given time. However, a Deployment is a higher-level concept that manages ReplicaSets and provides declarative updates to Pods along with a lot of other useful features. Therefore, use Deployments instead of directly using ReplicaSets, unless you require custom update orchestration or don't require updates at all.

https://kubernetes.io/docs/concepts/workloads/controllers/replicaset/

#### Alternative to ReplicaSets


https://kubernetes.io/docs/concepts/workloads/controllers/replicaset/#alternatives-to-replicaset

## Configmaps & Secrets

A ConfigMap is an API object used to store non-confidential data in key-value pairs. Pods can consume ConfigMaps as environment variables, command-line arguments, or as configuration files in a volume.

A ConfigMap allows you to decouple environment-specific configuration from your container images, so that your applications are easily portable.

Kubernetes Secrets let you store and manage sensitive information, such as passwords, OAuth tokens, and ssh keys. Storing confidential information in a Secret is safer and more flexible than putting it verbatim in a Pod definition or in a container image. See Secrets design document for more information.

A Secret is an object that contains a small amount of sensitive data such as a password, a token, or a key. Such information might otherwise be put in a Pod specification or in an image. Users can create Secrets and the system also creates some Secrets.

[https://www.youtube.com/watch?v=FAnQTgr04mU](https://www.youtube.com/watch?v=FAnQTgr04mU)


### Replication Controller

A ReplicationController ensures that a specified number of pod replicas are running at any one time. In other words, a ReplicationController makes sure that a pod or a homogeneous set of pods is always up and available.

https://kubernetes.io/docs/concepts/workloads/controllers/replicationcontroller/

### Alternatives to ReplicationController

https://kubernetes.io/docs/concepts/workloads/controllers/replicationcontroller/#alternatives-to-replicationcontroller

ReplicaSet is the next-generation ReplicationController that supports the new set-based label selector. It's mainly used by Deployment as a mechanism to orchestrate pod creation, deletion and updates. Note that we recommend using Deployments instead of directly using Replica Sets, unless you require custom update orchestration or don't require updates at all.

### Jobs

A Job creates one or more Pods and will continue to retry execution of the Pods until a specified number of them successfully terminate. As pods successfully complete, the Job tracks the successful completions. When a specified number of successful completions is reached, the task (ie, Job) is complete. Deleting a Job will clean up the Pods it created. Suspending a Job will delete its active Pods until the Job is resumed again.

https://kubernetes.io/docs/concepts/workloads/controllers/job/

Jobs are complementary to Replication Controllers. A Replication Controller manages Pods which are not expected to terminate (e.g. web servers), and a Job manages Pods that are expected to terminate (e.g. batch tasks).



Job is only appropriate for pods with RestartPolicy equal to OnFailure or Never. (Note: If RestartPolicy is not set, the default value is Always.)

#### Cron Jobs

You can use a CronJob to create a Job that will run at specified times/dates, similar to the Unix tool cron.

A CronJob creates Jobs on a repeating schedule.

One CronJob object is like one line of a crontab (cron table) file. It runs a job periodically on a given schedule, written in Cron format.

https://kubernetes.io/docs/concepts/workloads/controllers/cron-jobs/


Cron jobs are useful for creating periodic and recurring tasks, like running backups or sending emails. Cron jobs can also schedule individual tasks for a specific time, such as if you want to schedule a job for a low activity period.

Cron jobs have limitations and idiosyncrasies. For example, in certain circumstances, a single cron job can create multiple jobs. Therefore, jobs should be idempotent.


https://kubernetes.io/docs/tasks/job/automated-tasks-with-cron-jobs/

## CRD


CRD stands for  Custom Resource Definition.

https://insujang.github.io/2020-02-13/programming-kubernetes-crd/

A resource is an endpoint in the [Kubernetes API](https://kubernetes.io/docs/reference/using-api/api-overview/) that stores a collection of [API objects](https://kubernetes.io/docs/concepts/overview/working-with-objects/kubernetes-objects/) of a certain kind; for example, the built-in pods resource contains a collection of Pod objects.

https://itnext.io/building-your-own-kubernetes-crds-701de1c9a161

<img src="https://miro.medium.com/max/1575/1*1HdQc8st8vYA33ZwwYA7fA.png" width="600">

A custom resource is an extension of the Kubernetes API that is not necessarily available in a default Kubernetes installation. It represents a customization of a particular Kubernetes installation. However, many core Kubernetes functions are now built using custom resources, making Kubernetes more modular. Custom resources can appear and disappear in a running cluster through dynamic registration, and cluster admins can update custom resources independently of the cluster itself. Once a custom resource is installed, users can create and access its objects using [kubectl](https://kubernetes.io/docs/reference/kubectl/overview/), just as they do for built-in resources like Pods.

[https://kubernetes.io/docs/concepts/extend-kubernetes/api-extension/custom-resources/](https://kubernetes.io/docs/concepts/extend-kubernetes/api-extension/custom-resources/)

<!--<img src="https://miro.medium.com/max/5400/1*PTT5VXpyYHu1SQxXcULqhg.png" width="600">-->

Kubebuilder is a framework for building Kubernetes APIs using custom resource definitions (CRDs).

https://book.kubebuilder.io/quick-start.html

https://github.com/kubernetes-sigs/kubebuilder


## Operator Pattern

<img src="https://blog.container-solutions.com/hs-fs/hubfs/kubernetes_operators_diagram2.png?width=1875&name=kubernetes_operators_diagram2.png" width="600">

In Kubernetes, objects are analogous to a job or a completed task in the real world. You can use them to define common tasks, store them in a version control system, and apply them with kubectl apply. Kubernetes ensures that this triggers everything necessary to bring your declarative description to life by creating the dependent resources (like pods) to run your software. Kubernetes contains a number of built-in object types that can be created with this workflow, like Deployments and Services. 

<img src="https://blog.container-solutions.com/hs-fs/hubfs/kubernetes_operators_diagram1.png?width=1875&name=kubernetes_operators_diagram1.png" width="600">

With [Operators](https://www.youtube.com/watch?v=ha3LjlD6g7g), Kubernetes allows cluster maintainers or software providers to define their own Kubernetes object types, called custom resource definitions (CRDs). These objects can be handled by the Kubernetes API, just like built-in object types. Inside the Operator code, authors can define how to act on those custom objects. Operators are software extensions to Kubernetes that make use of [custom resources](https://kubernetes.io/docs/concepts/extend-kubernetes/api-extension/custom-resources/) to manage applications and their components. Operators follow Kubernetes principles, notably the [control loop](https://kubernetes.io/docs/concepts/architecture/controller).

https://blog.container-solutions.com/kubernetes-operators-explained

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

<img src="https://miro.medium.com/max/5400/1*jrkpUKU9pX9og6NNdnsbIw.jpeg" width="600">

## Certificates

https://cert-manager.io/docs/installation/kubernetes/

<img src="https://vocon-it.com/wp-content/uploads/2019/01/2019-01-08-00_15_00-Minikube-and-Kubeadm-Google-Pr%C3%A4sentationen.jpg" width="600">

https://krew.sigs.k8s.io/docs/user-guide/setup/install/

## Operator Hub

[https://operatorhub.io/](https://operatorhub.io/)

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


## Operator Sprawl

[https://thenewstack.io/the-runaway-problem-of-kubernetes-operators-and-dependency-lifecycles/](https://thenewstack.io/the-runaway-problem-of-kubernetes-operators-and-dependency-lifecycles/)

## Awesome links

[https://github.com/ramitsurana/awesome-kubernetes](https://github.com/ramitsurana/awesome-kubernetes)
