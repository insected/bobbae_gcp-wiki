## Basic Networking Model

The [Kubernetes networking model](https://kubernetes.io/docs/concepts/cluster-administration/networking/) supports different types of open source implementations. [Kubernetes provides an IP address to each pod](https://www.youtube.com/watch?v=WwQ62OyCNz4) so that there is no need to map host ports to container ports as in the Docker networking model. In [Kubernetes Networking Model](https://kubernetes.io/docs/concepts/cluster-administration/networking/#kubernetes-model) Pods behave much like VMs or physical hosts with respect to port allocation, naming, [load balancing]( Load-balancer  ) and application configuration. 

Every [Pod](https://kubernetes.io/docs/concepts/workloads/pods/) gets its own IP address. Pods on a node can communicate with all pods on all nodes without [NAT](NAT).

Agents on a node (e.g. system daemons, [kubelet](https://kubernetes.io/docs/reference/command-line-tools-reference/kubelet/)) can communicate with all pods on that node.

Kubernetes IP addresses exist at the Pod scope - containers within a Pod share their [network namespaces](https://www.packetcoders.io/how-to-view-the-network-namespaces-in-kubernetes/) - including their IP address and MAC address. 



## Cluster Networking

https://kubernetes.io/docs/concepts/cluster-administration/networking/


## Docker Networking vs. Kubernetes Networking

The [Docker networking model](https://docs.docker.com/network/) relies, by default, on a virtual bridge network. It is a per-host private network where containers get attached and allocated a private IP address. 

The [Kubernetes networking model](https://kubernetes.io/docs/concepts/cluster-administration/networking/) supports multi-host networking in which pods are able to communicate with each other.


## Kubernetes Networking Details

### Pod Networking

https://medium.com/google-cloud/understanding-kubernetes-networking-pods-7117dd28727

### Services

https://kubernetes.io/docs/concepts/services-networking/service/

https://medium.com/google-cloud/understanding-kubernetes-networking-services-f0cb48e4cc82

### Ingress


kubernetes [ingress](ingress) is a collection of rules.


https://medium.com/google-cloud/understanding-kubernetes-networking-ingress-1bc341c84078

## ClusterIP, Ingress, NodePort, Load Balancer

They're different ways [services of different types can be exposed](ClusterIP,-Ingress,-NodePort,-Load-Balancer).

## More on use of iptables and ipvs in Kubernetes


[Here](https://www.stackrox.com/post/2020/01/kubernetes-networking-demystified/) is an introduction into the complexities of Kubernetes networking by following the journey of an HTTP request to a service running on a basic Kubernetes cluster.

## Policies

[Kubernetes Network Policies]( https://kubernetes.io/docs/concepts/services-networking/network-policies/  ) are an application-centric construct which allow you to specify how a pod is allowed to communicate with various network entities over the network.



## Kubernetes Services Networking

In Kubernetes, a [Service is an abstraction](https://kubernetes.io/docs/concepts/services-networking/service/) which defines a logical set of Pods and a policy by which to [access them](  https://kubernetes.io/docs/concepts/services-networking/connect-applications-service/ 
). The set of Pods targeted by a [Service](   https://kubernetes.io/docs/concepts/services-networking/service/ ) is usually determined by a selector. 


## Topology aware traffic

https://kubernetes.io/docs/concepts/services-networking/service-topology/


## CNI

[CNI](https://github.com/containernetworking/cni) (Container Network Interface), a Cloud Native Computing Foundation project, consists of a specification and libraries for writing plugins to configure network interfaces in Linux containers, along with a number of supported plugins. CNI concerns itself only with network connectivity of containers and removing allocated resources when the container is deleted. 


### Calico

[Calico](https://docs.projectcalico.org/) supports multiple data planes including: a pure Linux [eBPF](eBPF) dataplane, a standard Linux networking dataplane, and a Windows HNS dataplane. 

https://www.tigera.io/blog/kubernetes-networking-with-calico/

While solutions like Flannel operate over layer 2, Calico makes use of layer 3 to route packets to pods. Calico can also provide network policy for Kubernetes. 


https://docs.projectcalico.org/networking/determine-best-networking#calico-compatible-cni-plugins-and-cloud-provider-integrations

#### BIRD

[BIRD](https://bird.network.cz/) is a [BGP](BGP) routing daemon which runs on every host. Calico makes uses of BGP to propagate routes between hosts. 

BIRD daemon runs on every host in the Kubernetes cluster, usually as a DaemonSet. It’s included in the calico/node container.



### Flannel

[Flannel](https://github.com/coreos/flannel#flannel) routes pod traffic using static per-node CIDRs obtained from the host-local IPAM CNI plugin. Flannel provides a number of networking backends, but is predominantly used with its [VXLAN](VLAN) overlay backend. Calico CNI and Calico network policy can be combined with flannel and the host-local IPAM plugin to provide a VXLAN network with policy enforcement. This combination is sometimes referred to as “Canal”.


https://github.com/flannel-io/flannel/blob/master/Documentation/backends.md

Calico now has built in support for VXLAN, which we generally recommend for simplicity in preference to using the Calico+Flannel combination.


### Cilium

[Cilium](Cilium) is open source software for providing and transparently securing network connectivity between application containers. 

#### Installing Cilium via kubeadm

https://docs.cilium.io/en/v1.9/gettingstarted/k8s-install-kubeadm/

### Contiv

[Contiv](https://github.com/contiv/netplugin) provides configurable networking (native L3 using BGP, overlay using vxlan, classic L2, or Cisco-SDN/ACI) for various use cases. 

### Contrail

[Contrail](https://www.juniper.net/us/en/products-services/sdn/contrail/contrail-networking/), based on [Tungsten Fabric](https://tungsten.io/), is a open, multi-cloud network virtualization and policy management platform. Contrail and Tungsten Fabric are integrated with various orchestration systems such as Kubernetes, OpenShift, OpenStack and Mesos, and provide different isolation modes for virtual machines, containers/pods and bare metal workloads.

### Kube-router  

[Kube-router](https://github.com/cloudnativelabs/kube-router) is a purpose-built networking solution for Kubernetes that aims to provide high performance and operational simplicity. Kube-router provides a Linux LVS/IPVS-based service proxy, a Linux kernel forwarding-based pod-to-pod networking solution with no overlays, and iptables/ipset-based network policy enforcer.

### OVN

[OVN](  https://www.ovn.org/  ) is an opensource network virtualization solution developed by the Open vSwitch community. OVN lets one create logical switches, logical routers, stateful ACLs, load-balancers etc to build different virtual networking topologies. 

#### OVN Kubernetes

https://github.com/openvswitch/ovn-kubernetes

### Romana

[Romana](https://romana.io/) is an open source network and security automation solution that lets you deploy Kubernetes without an overlay network. Romana supports Kubernetes Network Policy to provide isolation across network namespaces.

### Weavenet

[Weave Net](https://www.weave.works/oss/net/)  runs as a CNI plug-in or stand-alone. Weave Net creates a network bridge on the host. Each container is connected to that bridge via a veth pair, the container side of which is given an IP address and netmask supplied either by the user or by Weave Net’s IP address allocator.

Weave Net routes packets between containers on different hosts via two methods: a fast data path method, which operates entirely in kernel space, and a fallback [sleeve method](https://www.weave.works/docs/net/latest/concepts/router-encapsulation/), in which packets destined for non-local containers are captured by the kernel and processed by the Weave Net router in user space, forwarded over UDP to weave router peers running on other hosts, and there injected back into the kernel which in turn passes them to local destination containers.

https://www.weave.works/docs/net/latest/concepts/how-it-works/



### kilo

[Kilo](  https://github.com/squat/kilo  ) is a multi-cloud network overlay built on [WireGuard](  https://www.wireguard.com/ ) and designed for Kubernetes.


