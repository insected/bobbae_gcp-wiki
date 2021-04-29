# Kubernetes  service

An abstract way to expose an application running on a set of Pods as a network service.
With Kubernetes you don't need to modify your application to use an unfamiliar service discovery mechanism. Kubernetes gives Pods their own IP addresses and a single DNS name for a set of Pods, and can load-balance across them.

https://kubernetes.io/docs/concepts/services-networking/service/

A service can be exposed via NodePort, LoadBalancer or ClusterIP.

https://cloud.google.com/kubernetes-engine/docs/concepts/service

When to use NodePort vs. LoadBalancer  can be confusing. 

https://medium.com/google-cloud/kubernetes-nodeport-vs-loadbalancer-vs-ingress-when-should-i-use-what-922f010849e0

## GKE

https://cloud.google.com/kubernetes-engine/docs/how-to/exposing-apps

## Service Types

## ClusterIP

A ClusterIP service is the default Kubernetes service. It gives you a service inside your cluster that other apps inside your cluster can access. There is no external access. It exposes the Service on a cluster-internal IP. Choosing this value makes the Service only reachable from within the cluster. This is the default ServiceType.

### iptables

In iptables proxy mode, kube-proxy watches  the Kubernetes control plane for the addition and removal of Service and Endpoint objects. For each Service, it installs iptables rules, which capture traffic to the Service's clusterIP and port, and redirect that traffic to one of the Service's backend sets. For each Endpoint object, it installs iptables rules which select a backend Pod.

By default, kube-proxy in iptables mode chooses a backend at random.

https://kubernetes.io/docs/concepts/services-networking/service/#proxy-mode-iptables

### ipvs

In ipvs mode, kube-proxy watches Kubernetes Services and Endpoints, calls netlink interface to create IPVS rules accordingly and synchronizes IPVS rules with Kubernetes Services and Endpoints periodically. This control loop ensures that IPVS status matches the desired state. When accessing a Service, IPVS directs traffic to one of the backend Pods.

https://kubernetes.io/docs/concepts/services-networking/service/#proxy-mode-iptables

## NodePort

A NodePort service is the most primitive way to get external traffic directly to your service. NodePort, as the name implies, opens a specific port on all the Nodes (the VMs), and any traffic that is sent to this port is forwarded to the service.

NodePort exposes the Service on each Node's IP at a static port (the NodePort). A ClusterIP Service, to which the NodePort Service routes, is automatically created. You'll be able to contact the NodePort Service, from outside the cluster, by requesting <NodeIP>:<NodePort>.

https://kubernetes.io/docs/concepts/services-networking/service/#nodeport

## LoadBalancer

A LoadBalancer service is the standard way to expose a service to the internet. On GKE, this will spin up a [Network Load Balancer](https://cloud.google.com/compute/docs/load-balancing/network/) that will give you a single IP address that will forward all traffic to your service.

https://kubernetes.io/docs/concepts/services-networking/service/#loadbalancer

https://github.com/bobbae/gcp/wiki/Load-Balancer

### MetalLB

Kubernetes does not offer an implementation of network load-balancers (Services of type LoadBalancer) for bare metal clusters. The implementations of Network LB that Kubernetes does ship with are all glue code that calls out to various IaaS platforms (GCP, AWS, Azure…). If you’re not running on a supported IaaS platform (GCP, AWS, Azure…), LoadBalancers will remain in the “pending” state indefinitely when created.

Bare metal cluster operators are left with two lesser tools to bring user traffic into their clusters, “NodePort” and “externalIPs” services. Both of these options have significant downsides for production use, which makes bare metal clusters second class citizens in the Kubernetes ecosystem.

MetalLB aims to redress this imbalance by offering a Network LB implementation that integrates with standard network equipment, so that external services on bare metal clusters also “just work” as much as possible.

MetalLB is a load-balancer implementation for bare metal Kubernetes clusters, using standard routing protocols.
https://metallb.universe.tf/

## External Name

Services of type ExternalName map a Service to a DNS name, not to a typical selector such as my-service or cassandra. You specify these Services with the spec.externalName parameter.

https://kubernetes.io/docs/concepts/services-networking/service/#externalname

# Ingress

https://github.com/bobbae/gcp/wiki/Ingress

https://kubernetes.io/docs/concepts/services-networking/ingress/

