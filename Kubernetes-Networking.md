## Basic Networking Model

The [Kubernetes networking model](https://www.aquasec.com/cloud-native-academy/kubernetes-101/kubernetes-networking) supports different types of open source implementations. [Kubernetes provides an IP address to each pod](https://www.youtube.com/watch?v=WwQ62OyCNz4) so that there is no need to map host ports to container ports as in the Docker networking model. In [Kubernetes Networking Model](https://kubernetes.io/docs/concepts/cluster-administration/networking/#kubernetes-model) Pods behave much like VMs or physical hosts with respect to port allocation, naming, load balancing and application configuration. 

Every [Pod](https://www.youtube.com/watch?v=5cNrTU6o3Fw) gets its own IP address. This means you do not need to explicitly create links between Pods and you almost never need to deal with mapping container ports to host ports. This creates a clean, backwards-compatible model where Pods can be treated much like VMs or physical hosts from the perspectives of port allocation, naming, service discovery, load balancing, application configuration, and migration.

Pods on a node can communicate with all pods on all nodes without NAT.

Agents on a node (e.g. system daemons, [kubelet](https://kubernetes.io/docs/reference/command-line-tools-reference/kubelet/)) can communicate with all pods on that node.

Pods in the host network of a node can communicate with all pods on all nodes without NAT.

This model is not only less complex overall, but it is principally compatible with the desire for Kubernetes to enable low-friction porting of apps from VMs to containers. If your job previously ran in a VM, your VM had an IP and could talk to other VMs in your project. This is the same basic model.

Kubernetes IP addresses exist at the Pod scope - containers within a Pod share their [network namespaces](https://www.youtube.com/watch?v=j_UUnlVC2Ss) - including their IP address and MAC address. 

This means that containers within a Pod can all reach each other's ports on localhost. 

This also means that containers within a Pod must coordinate port usage, but this is no different from processes in a VM. This is called the "IP-per-pod" model.

## Cluster Networking



<img src="https://d33wubrfki0l68.cloudfront.net/e351b830334b8622a700a8da6568cb081c464a9b/13020/images/docs/services-userspace-overview.svg" width="500">

[Kubernetes Networking](https://kubernetes.io/docs/concepts/cluster-administration/networking/) is a central part of Kubernetes, but it can be challenging to understand exactly how it is expected to work. There are 4 distinct networking problems to address:

1. Highly-coupled container-to-container communications
2. Pod-to-Pod communications
3. Pod-to-Service communications
4. External-to-Service communications

## Docker Networking vs. Kubernetes Networking

The [Docker networking model](https://docs.docker.com/network/) relies, by default, on a virtual bridge network called Docker0. It is a per-host private network where containers get attached (and thus can reach each other) and allocated a private IP address. This means containers running on different machines are not able to communicate with each other (as they are attached to different hosts’ networks). In order to communicate across nodes with Docker, we have to map host ports to container ports and proxy the traffic. In this scenario, it’s up to the Docker operator to avoid port clashes between containers.

The [Kubernetes networking model](https://kubernetes.io/docs/concepts/cluster-administration/networking/), on the other hand, natively supports multi-host networking in which pods are able to communicate with each other by default, regardless of which host they live in. Kubernetes does not provide an implementation of this model by default, rather it relies on third-party tools that comply with the following requirements: all containers are able to communicate with each other without NAT; nodes are able to communicate with containers without NAT; and a container’s IP address is the same from inside and outside the container.

Kubernetes follows an “IP-per-pod” model where each pod get assigned an IP address and all containers in a single pod share the same network namespaces and IP address. Containers in the same pod can therefore reach each other’s ports via localhost:<port>. However, it is not recommended to communicate directly with a pod via its IP address due to pod’s volatility (a pod can be killed and replaced at any moment). Instead, use a Kubernetes service which represents a group of pods acting as a single entity to the outside. Services get allocated their own IP address in the cluster and provide a reliable entry point.

## ClusterIP, [Ingress](https://www.youtube.com/watch?v=GhZi4DxaxxE), NodePort, Load Balancer

It is useful to study [how services are exposed](ClusterIP,-Ingress,-NodePort,-Load-Balancer).

## More on use of iptables and ipvs in Kubernetes


[Here](https://www.stackrox.com/post/2020/01/kubernetes-networking-demystified/) is an introduction into the complexities of Kubernetes networking by following the journey of an HTTP request to a service running on a basic Kubernetes cluster.

<img src="https://miro.medium.com/max/1575/1*UetnYP8uE05GAqQD0tbtBQ.png" width="600">

You can use a pod IP address as an endpoint but there is no guarantee that the address won’t change the next time the pod is recreated, which might happen for any number of reasons.

The kubernetes designers [solved this problem](https://medium.com/google-cloud/understanding-kubernetes-networking-services-f0cb48e4cc82) in a way that builds on the basic capabilities of the platform to deliver on all three of those requirements, and it starts with a resource type called a service.



<img src="https://miro.medium.com/max/1575/1*iezVQZMVEqzic_yfREO8Jw.png" width="400">


## Policies

If you want to control traffic flow at the IP address or port level (OSI layer 3 or 4), then you might consider using Kubernetes NetworkPolicies for particular applications in your cluster. NetworkPolicies are an application-centric construct which allow you to specify how a pod is allowed to communicate with various network "entities" (we use the word "entity" here to avoid overloading the more common terms such as "endpoints" and "services", which have specific Kubernetes connotations) over the network.

https://kubernetes.io/docs/concepts/services-networking/network-policies/

## Kubernetes Services Networking

In Kubernetes, a [Service is an abstraction](https://www.youtube.com/watch?v=T4Z7visMM4E) which defines a logical set of Pods and a policy by which to access them (sometimes this pattern is called a micro-service). The set of Pods targeted by a Service is usually determined by a selector. For example, consider a stateless image-processing backend which is running with 3 replicas. Those replicas are fungible—frontends do not care which backend they use. While the actual Pods that compose the backend set may change, the frontend clients should not need to be aware of that, nor should they need to keep track of the set of backends themselves.

https://kubernetes.io/docs/concepts/services-networking/service/

By default, Docker uses host-private networking, so containers can talk to other containers only if they are on the same machine. In order for Docker containers to communicate across nodes, there must be allocated ports on the machine's own IP address, which are then forwarded or proxied to the containers. This obviously means that containers must either coordinate which ports they use very carefully or ports must be allocated dynamically.

<img src="https://d1jnx9ba8s6j9r.cloudfront.net/blog/wp-content/uploads/2018/08/22-1.png" width="600">

Coordinating port allocations across multiple developers or teams that provide containers is very difficult to do at scale, and exposes users to cluster-level issues outside of their control. Kubernetes assumes that pods can communicate with other pods, regardless of which host they land on. Kubernetes gives every pod its own cluster-private IP address, so you do not need to explicitly create links between pods or map container ports to host ports. This means that containers within a Pod can all reach each other's ports on localhost, and all pods in a cluster can see each other without NAT. The rest of this document elaborates on how you can run reliable services on such a networking model.

https://kubernetes.io/docs/concepts/services-networking/connect-applications-service/

## Topology aware traffic

By default, traffic sent to a ClusterIP or NodePort Service may be routed to any backend address for the Service. Kubernetes 1.7 made it possible to route "external" traffic to the Pods running on the same Node that received the traffic. For ClusterIP Services, the equivalent same-node preference for routing wasn't possible; nor could you configure your cluster to favor routing to endpoints within the same zone.

https://kubernetes.io/docs/concepts/services-networking/service-topology/

## CNI

[CNI](https://www.youtube.com/watch?v=l2BS_kuQxBA) (Container Network Interface), a Cloud Native Computing Foundation project, consists of a specification and libraries for writing plugins to configure network interfaces in Linux containers, along with a number of supported plugins. CNI concerns itself only with network connectivity of containers and removing allocated resources when the container is deleted. Because of this focus, CNI has a wide range of support and the specification is simple to implement.

https://github.com/containernetworking/cni

<img src="https://d1jnx9ba8s6j9r.cloudfront.net/blog/wp-content/uploads/2018/08/Pods.png" width="600">
