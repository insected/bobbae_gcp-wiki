## Kubernetes  service

Kubernetes [service](https://kubernetes.io/docs/concepts/services-networking/service/) is an abstract way to expose an application running on a set of Pods as a [Network](Kubernetes-Networking) service.

With Kubernetes you don't need to modify your application to use an unfamiliar service discovery mechanism. Kubernetes gives Pods their own IP addresses and a single DNS name for a set of Pods, and can load-balance across them.

https://kubernetes.io/docs/concepts/services-networking/service/

A service can be [exposed](https://kubernetes.io/docs/concepts/services-networking/connect-applications-service/) via [NodePort](https://kubernetes.io/docs/concepts/services-networking/service/#nodeport), [LoadBalancer](https://kubernetes.io/docs/concepts/services-networking/service/#loadbalancer) or ClusterIP.

A NodePort is an open port on every node of your cluster. Kubernetes transparently routes incoming traffic on the NodePort to your service, even if your application is running on a different node.

Using a LoadBalancer service type automatically deploys an external load balancer. This external load balancer is associated with a specific IP address and routes external traffic to a Kubernetes service in your cluster.

https://cloud.google.com/kubernetes-engine/docs/concepts/service


When to use NodePort vs. LoadBalancer  can be confusing. 

https://medium.com/google-cloud/kubernetes-nodeport-vs-loadbalancer-vs-ingress-when-should-i-use-what-922f010849e0

## GKE

[GKE](GKE) is a Secured and fully managed Kubernetes service with revolutionary autopilot mode of operation.



## Service Types


Services can be exposed in [different ways](https://cloud.google.com/kubernetes-engine/docs/how-to/exposing-apps)

## ClusterIP

A [ClusterIP](https://wikipedia.org/wiki/Cluster_IP) service is the default Kubernetes service. It gives you a service inside your cluster that other apps inside your cluster can access. There is no external access. It exposes the Service on a cluster-internal IP. Choosing this value makes the Service only reachable from within the cluster. This is the default ServiceType.

The ClusterIP in kubernetes is a service type which has its origins in the iptables CLUSTERIP.  

https://book.huihoo.com/iptables-tutorial/x8906.htm

### Kube-proxy

There are several types of proxies in Kubernetes, and among them is the node proxier, or [kube-proxy](https://kubernetes.io/docs/reference/command-line-tools-reference/kube-proxy/), which [reflects services defined in Kubernetes API on each node](https://kubernetes.io/docs/reference/command-line-tools-reference/kube-proxy/)  and performs simple TCP/UDP/SCTP stream [forwarding across a set of backends](https://arthurchiao.art/blog/cracking-k8s-node-proxy/).




### iptables

In [iptables](https://en.wikipedia.org/wiki/Iptables)  proxy mode, kube-proxy watches  the Kubernetes control plane for the addition and removal of Service and Endpoint objects. For each Service, it installs iptables rules, which capture traffic to the Service's clusterIP and port, and redirect that traffic to one of the Service's backend sets. For each Endpoint object, it installs iptables rules which select a backend Pod.


By default, [kube-proxy](https://kubernetes.io/docs/concepts/overview/components/#kube-proxy) in iptables mode chooses a backend at random.

https://kubernetes.io/docs/concepts/services-networking/service/#proxy-mode-iptables


https://www.digitalocean.com/community/tutorials/a-deep-dive-into-iptables-and-netfilter-architecture

### ipvs

In [ipvs](http://www.linuxvirtualserver.org/software/ipvs.html) mode, kube-proxy watches Kubernetes Services and Endpoints, calls netlink interface to create IPVS rules accordingly and synchronizes IPVS rules with Kubernetes Services and Endpoints periodically. This control loop ensures that IPVS status matches the desired state. When accessing a Service, IPVS directs traffic to one of the backend Pods.

https://kubernetes.io/docs/concepts/services-networking/service/#proxy-mode-iptables

## NodePort

A [NodePort](   https://kubernetes.io/docs/concepts/services-networking/service/#nodeport ) service is the most primitive way to get external traffic directly to your service. NodePort, as the name implies, opens a specific port on all the Nodes (the VMs), and any traffic that is sent to this port is forwarded to the service.

NodePort exposes the Service on each Node's IP at a static port (the NodePort). A ClusterIP Service, to which the NodePort Service routes, is automatically created. You'll be able to contact the NodePort Service, from outside the cluster, by requesting ’<NodeIP>:<NodePort>'.





https://hackernoon.com/introducing-nodeport-service-in-kubernetes-ear0360s

## LoadBalancer

A [LoadBalancer](  https://kubernetes.io/docs/concepts/services-networking/service/#loadbalancer ) service is the [standard way to expose a service](  Load-Balancer ) to the internet. On GKE, this will spin up a [Network Load Balancer](https://cloud.google.com/compute/docs/load-balancing/network/) that will give you a single IP address that will forward all traffic to your service.






### MetalLB

Kubernetes does not offer an implementation of network load-balancers (Services of type LoadBalancer) for bare metal clusters. The implementations of Network LB that Kubernetes does ship with are all glue code that calls out to various IaaS platforms (GCP, AWS, Azure…). If you’re not running on a supported IaaS platform (GCP, AWS, Azure…), LoadBalancers will remain in the “pending” state indefinitely when created.

Bare metal cluster operators are left with two lesser tools to bring user traffic into their clusters, “NodePort” and “externalIPs” services. Both of these options have significant downsides for production use, which makes bare metal clusters second class citizens in the Kubernetes ecosystem.

[MetalLB](https://metallb.universe.tf/) aims to redress this imbalance by offering a Network LB implementation that integrates with standard network equipment, so that external services on bare metal clusters also “just work” as much as possible.

MetalLB is a load-balancer implementation for bare metal Kubernetes clusters, using standard routing protocols.


## External Name

Services of type [ExternalName](https://kubernetes.io/docs/concepts/services-networking/service/#externalname) map a Service to a DNS name, not to a typical selector such as my-service or cassandra. You specify these Services with the spec.externalName parameter.



## Ingress

[Ingress](Ingress)  is not a Service type, but it acts as the entry point for your cluster. It lets you consolidate your routing rules into a single resource as it can expose multiple services under the same IP address.


https://kubernetes.io/docs/concepts/services-networking/ingress/

## ECMP

[ECMP](  https://wikipedia.org/wiki/Equal-cost_multi-path_routing ) stands for “equal-cost multi-path”; it’s a routing strategy where packets are forwarded to one of any “best paths” in a network. How the best paths are determined depends on a lot of factors, but typically, the best path is likely the shortest path (the path with the least amount of hops). The most common example of using [anycast](  https://en.m.wikipedia.org/wiki/Anycast  ) is with global DNS services where we want one IP (think 1.1.1.1 or 8.8.8.8) to be routed to the closest site that is running a globally distributed DNS service. [BGP](  https://en.m.wikipedia.org/wiki/Border_Gateway_Protocol  ) is one of many routing protocols that allows us to implement ECMP routing.
 

If you’ve already configured your network to handle ECMP routing, then all that’s left to implement anycast is to advertise your anycast IP over multiple BGP peers. With Kubernetes, we can advertise service IPs to accomplish anycast routing for any of our services.

https://www.asykim.com/blog/kubernetes-traffic-engineering-with-bgp
