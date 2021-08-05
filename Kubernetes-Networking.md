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

https://kubernetes.io/docs/concepts/cluster-administration/networking/

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

<!--<img src="https://miro.medium.com/max/1575/1*UetnYP8uE05GAqQD0tbtBQ.png" width="600">-->

You can use a pod IP address as an endpoint but there is no guarantee that the address won’t change the next time the pod is recreated, which might happen for any number of reasons.

The kubernetes designers [solved this problem](https://medium.com/google-cloud/understanding-kubernetes-networking-services-f0cb48e4cc82) in a way that builds on the basic capabilities of the platform to deliver on all three of those requirements, and it starts with a resource type called a service.



<!--<img src="https://miro.medium.com/max/1575/1*iezVQZMVEqzic_yfREO8Jw.png" width="400">-->


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

https://kubernetes.io/docs/concepts/cluster-administration/networking/

### Calico

[Calico](https://docs.projectcalico.org/) is an open source networking and network security solution for containers, virtual machines, and native host-based workloads. Calico supports multiple data planes including: a pure Linux eBPF dataplane, a standard Linux networking dataplane, and a Windows HNS dataplane. 

https://www.tigera.io/blog/kubernetes-networking-with-calico/

While solutions like Flannel operate over layer 2, Calico makes use of layer 3 to route packets to pods. The way it does this is relatively simple in practice. Calico can also provide network policy for Kubernetes. 

Calico provides a full networking stack but can also be used in conjunction with cloud provider CNIs to provide network policy enforcement.

https://docs.projectcalico.org/networking/determine-best-networking#calico-compatible-cni-plugins-and-cloud-provider-integrations

#### BIRD

[BIRD](https://bird.network.cz/) is a BGP routing daemon which runs on every host. Calico makes uses of BGP to propagate routes between hosts. BGP (if you’re not aware) is widely used to propagate routes over the internet. It’s suggested you make yourself familiar with some of the concepts if you’re using Calico.

BIRD daemon runs on every host in the Kubernetes cluster, usually as a DaemonSet. It’s included in the calico/node container.



### Flannel

[Flannel](https://github.com/coreos/flannel#flannel) routes pod traffic using static per-node CIDRs obtained from the host-local IPAM CNI plugin. Flannel provides a number of networking backends, but is predominantly used with its VXLAN overlay backend. Calico CNI and Calico network policy can be combined with flannel and the host-local IPAM plugin to provide a VXLAN network with policy enforcement. This combination is sometimes referred to as “Canal”.


https://github.com/flannel-io/flannel/blob/master/Documentation/backends.md

Calico now has built in support for VXLAN, which we generally recommend for simplicity in preference to using the Calico+Flannel combination.


### Cilium

[Cilium](https://github.com/cilium/cilium) is open source software for providing and transparently securing network connectivity between application containers. Cilium is L7/HTTP aware and can enforce network policies on L3-L7 using an identity based security model that is decoupled from network addressing, and it can be used in combination with other CNI plugins.

### Contiv

[Contiv](https://github.com/contiv/netplugin) provides configurable networking (native l3 using BGP, overlay using vxlan, classic l2, or Cisco-SDN/ACI) for various use cases. Contiv is all open sourced.

### Contrail

[Contrail](https://www.juniper.net/us/en/products-services/sdn/contrail/contrail-networking/), based on [Tungsten Fabric](https://tungsten.io/), is a truly open, multi-cloud network virtualization and policy management platform. Contrail and Tungsten Fabric are integrated with various orchestration systems such as Kubernetes, OpenShift, OpenStack and Mesos, and provide different isolation modes for virtual machines, containers/pods and bare metal workloads.

### Kube-router  

[Kube-router](https://github.com/cloudnativelabs/kube-router) is a purpose-built networking solution for Kubernetes that aims to provide high performance and operational simplicity. Kube-router provides a Linux LVS/IPVS-based service proxy, a Linux kernel forwarding-based pod-to-pod networking solution with no overlays, and iptables/ipset-based network policy enforcer.

### OVN

OVN is an opensource network virtualization solution developed by the Open vSwitch community. It lets one create logical switches, logical routers, stateful ACLs, load-balancers etc to build different virtual networking topologies. The project has a specific Kubernetes plugin and documentation at [ovn-kubernetes](https://github.com/openvswitch/ovn-kubernetes).

### Romana

[Romana](https://romana.io/) is an open source network and security automation solution that lets you deploy Kubernetes without an overlay network. Romana supports Kubernetes Network Policy to provide isolation across network namespaces.

### Weavenet

[Weave Net](https://www.weave.works/oss/net/) is a resilient and simple to use network for Kubernetes and its hosted applications. Weave Net runs as a CNI plug-in or stand-alone. In either version, it doesn't require any configuration or extra code to run, and in both cases, the network provides one IP address per pod - as is standard for Kubernetes.

Weave Net creates a network bridge on the host. Each container is connected to that bridge via a veth pair, the container side of which is given an IP address and netmask supplied either by the user or by Weave Net’s IP address allocator.

Weave Net routes packets between containers on different hosts via two methods: a fast data path method, which operates entirely in kernel space, and a fallback [sleeve method](https://www.weave.works/docs/net/latest/concepts/router-encapsulation/), in which packets destined for non-local containers are captured by the kernel and processed by the Weave Net router in user space, forwarded over UDP to weave router peers running on other hosts, and there injected back into the kernel which in turn passes them to local destination containers.



https://www.weave.works/docs/net/latest/concepts/how-it-works/