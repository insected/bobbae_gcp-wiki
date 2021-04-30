# Cluster Architecture

[[https://d1jnx9ba8s6j9r.cloudfront.net/blog/wp-content/uploads/2018/08/16-1.png]]

[[https://d1jnx9ba8s6j9r.cloudfront.net/blog/wp-content/uploads/2018/08/7.png]]

## Cattle vs. Pets

http://cloudscaling.com/blog/cloud-computing/the-history-of-pets-vs-cattle/

## Nodes

[[https://d1jnx9ba8s6j9r.cloudfront.net/blog/wp-content/uploads/2018/08/15-1.png]]


Kubernetes runs your workload by placing containers into Pods to run on Nodes. A node may be a virtual or physical machine, depending on the cluster. Each node is managed by the control plane and contains the services necessary to run Pods

Typically you have several nodes in a cluster; in a learning or resource-limited environment, you might have only one node.

[[https://d1jnx9ba8s6j9r.cloudfront.net/blog/wp-content/uploads/2018/08/18-1.png]]

## Pods

Pods are the smallest deployable units of computing that you can create and manage in Kubernetes.

https://medium.com/google-cloud/understanding-kubernetes-networking-pods-7117dd28727

A Pod (as in a pod of whales or pea pod) is a group of one or more containers, with shared storage and network resources, and a specification for how to run the containers. A Pod's contents are always co-located and co-scheduled, and run in a shared context. A Pod models an application-specific "logical host": it contains one or more application containers which are relatively tightly coupled. In non-cloud contexts, applications executed on the same physical or virtual machine are analogous to cloud applications executed on the same logical host.

https://kubernetes.io/docs/concepts/workloads/pods/

[[https://miro.medium.com/max/1575/1*oyGbXt7kStLd85ZT4it3oQ.png]]

[[https://miro.medium.com/max/1575/1*Ow5A6_zjjwdKkf2Yi1KgYw.png]]

## Control Plane

[[https://d1jnx9ba8s6j9r.cloudfront.net/blog/wp-content/uploads/2018/08/25-1.png]]

Kubernetes has a "hub-and-spoke" API pattern. All API usage from nodes (or the pods they run) terminates at the apiserver. None of the other control plane components are designed to expose remote services. The apiserver is configured to listen for remote connections on a secure HTTPS port (typically 443) with one or more forms of client authentication enabled. One or more forms of authorization should be enabled, especially if anonymous requests or service account tokens are allowed.

## Controller 
In robotics and automation, a control loop is a non-terminating loop that regulates the state of a system.

Here is one example of a control loop: a thermostat in a room.

When you set the temperature, that's telling the thermostat about your desired state. The actual room temperature is the current state. The thermostat acts to bring the current state closer to the desired state, by turning equipment on or off.

In Kubernetes, controllers are control loops that watch the state of your cluster, then make or request changes where needed. Each controller tries to move the current cluster state closer to the desired state.


## Cloud Controller Manager

The cloud-controller-manager is a Kubernetes control plane component that embeds cloud-specific control logic. The cloud controller manager lets you link your cluster into your cloud provider's API, and separates out the components that interact with that cloud platform from components that only interact with your cluster.

By decoupling the interoperability logic between Kubernetes and the underlying cloud infrastructure, the cloud-controller-manager component enables cloud providers to release features at a different pace compared to the main Kubernetes project.

https://kubernetes.io/docs/concepts/architecture/

[[https://miro.medium.com/proxy/1*ax_IkyNCNlNUYY8WKrawaA.png]]

## Networking

https://github.com/bobbae/gcp/wiki/Kubernetes-Networking

[[https://d1jnx9ba8s6j9r.cloudfront.net/blog/wp-content/uploads/2018/08/18-1.png]]

[[https://d1jnx9ba8s6j9r.cloudfront.net/blog/wp-content/uploads/2018/08/Pods.png]]

## Components

### etcd

https://kubernetes.io/docs/concepts/overview/components/#etcd

[[https://superuser.openstack.org/wp-content/uploads/2019/11/etcd-in-Kubernetes.png]]


[[https://superuser.openstack.org/wp-content/uploads/2019/11/etcd-in-Kubernetes-2.png]]

### kube-controller-manager
https://kubernetes.io/docs/concepts/overview/components/#kube-controller-manager

### cloud-controller-manager
https://kubernetes.io/docs/concepts/overview/components/#cloud-controller-manager

### kubelet

https://kubernetes.io/docs/concepts/overview/components/#kubelet

### kube-proxy

https://kubernetes.io/docs/concepts/overview/components/#kube-proxy

### cluster DNS

https://kubernetes.io/docs/concepts/services-networking/dns-pod-service/

### resource monitoring

https://kubernetes.io/docs/tasks/debug-application-cluster/resource-usage-monitoring/

### kube-scheduler

https://kubernetes.io/docs/concepts/scheduling-eviction/kube-scheduler/


# Kubernetes URLs

[https://github.com/ramitsurana/awesome-kubernetes](https://github.com/ramitsurana/awesome-kubernetes)


# Resource Limits

When you specify a Pod, you can optionally specify how much of each resource a Container needs. The most common resources to specify are CPU and memory (RAM); there are others.

When you specify the resource request for Containers in a Pod, the scheduler uses this information to decide which node to place the Pod on. When you specify a resource limit for a Container, the kubelet enforces those limits so that the running container is not allowed to use more of that resource than the limit you set. The kubelet also reserves at least the request amount of that system resource specifically for that container to use.

# Requests and limits 

If the node where a Pod is running has enough of a resource available, it's possible (and allowed) for a container to use more resource than its request for that resource specifies. However, a container is not allowed to use more than its resource limit.

[https://www.youtube.com/watch?v=xjpHggHKm78&list=PLIivdWyY5sqL3xfXz5xJvwzFW_tlQB_GB&index=4](https://www.youtube.com/watch?v=xjpHggHKm78&list=PLIivdWyY5sqL3xfXz5xJvwzFW_tlQB_GB&index=4)


# RBAC

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

# Configmaps & Secrets

A ConfigMap is an API object used to store non-confidential data in key-value pairs. Pods can consume ConfigMaps as environment variables, command-line arguments, or as configuration files in a volume.

A ConfigMap allows you to decouple environment-specific configuration from your container images, so that your applications are easily portable.

Kubernetes Secrets let you store and manage sensitive information, such as passwords, OAuth tokens, and ssh keys. Storing confidential information in a Secret is safer and more flexible than putting it verbatim in a Pod definition or in a container image. See Secrets design document for more information.

A Secret is an object that contains a small amount of sensitive data such as a password, a token, or a key. Such information might otherwise be put in a Pod specification or in an image. Users can create Secrets and the system also creates some Secrets.

[https://www.youtube.com/watch?v=FAnQTgr04mU](https://www.youtube.com/watch?v=FAnQTgr04mU)


# Stateful Sets

StatefulSet is the workload API object used to manage stateful applications.

Manages the deployment and scaling of a set of Pods, and provides guarantees about the ordering and uniqueness of these Pods.

[https://www.youtube.com/watch?v=pPQKAR1pA9U](https://www.youtube.com/watch?v=pPQKAR1pA9U)


# DaemonSet

A DaemonSet ensures that all (or some) Nodes run a copy of a Pod. As nodes are added to the cluster, Pods are added to them. As nodes are removed from the cluster, those Pods are garbage collected. Deleting a DaemonSet will clean up the Pods it created.

[https://kubernetes.io/docs/concepts/workloads/controllers/daemonset/](https://kubernetes.io/docs/concepts/workloads/controllers/daemonset/)


# CRD

CRD stands for  Custom Resource Definition.

A resource is an endpoint in the [Kubernetes API](https://kubernetes.io/docs/reference/using-api/api-overview/) that stores a collection of [API objects](https://kubernetes.io/docs/concepts/overview/working-with-objects/kubernetes-objects/) of a certain kind; for example, the built-in pods resource contains a collection of Pod objects.

A custom resource is an extension of the Kubernetes API that is not necessarily available in a default Kubernetes installation. It represents a customization of a particular Kubernetes installation. However, many core Kubernetes functions are now built using custom resources, making Kubernetes more modular. Custom resources can appear and disappear in a running cluster through dynamic registration, and cluster admins can update custom resources independently of the cluster itself. Once a custom resource is installed, users can create and access its objects using [kubectl](https://kubernetes.io/docs/reference/kubectl/overview/), just as they do for built-in resources like Pods.

[https://kubernetes.io/docs/concepts/extend-kubernetes/api-extension/custom-resources/](https://kubernetes.io/docs/concepts/extend-kubernetes/api-extension/custom-resources/)

Kubebuilder is a framework for building Kubernetes APIs using custom resource definitions (CRDs).

https://book.kubebuilder.io/quick-start.html

https://github.com/kubernetes-sigs/kubebuilder


# Operator Pattern

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

# Operator Hub

[https://operatorhub.io/](https://operatorhub.io/)


# Operator Sprawl

[https://thenewstack.io/the-runaway-problem-of-kubernetes-operators-and-dependency-lifecycles/](https://thenewstack.io/the-runaway-problem-of-kubernetes-operators-and-dependency-lifecycles/)

