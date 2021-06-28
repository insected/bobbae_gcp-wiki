

[Cloud Load Balancing](https://cloud.google.com/load-balancing) allows you to put your resources behind a single IP address that is externally accessible or internal to your Virtual Private Cloud (VPC) network.

[Cloud Load Balancing](https://cloud.google.com/load-balancing/docs) can put your resources behind a single [anycast](https://en.wikipedia.org/wiki/Anycast) IP and scale your resources up or down with intelligent autoscaling. Cloud Load Balancing comes in a variety of flavors and is integrated with [Cloud CDN](CDN) for optimal application and content delivery.


A [Video](https://www.youtube.com/watch?v=D4XZkCJyqis) about Cloud Load Balancing.


Google Cloud Load Balancing enables enterprises and cloud-natives to deliver highly available, scalable, low-latency cloud services with a global footprint. Use Google Global Load Balancing to deliver [global reach and scale](https://www.youtube.com/watch?v=J5HJ1y6PeyE). Deploy your application backends in single or multiple regions wherever your users are, front-ending these with a single anycast VIP, and growing or shrinking your backend resources with intelligent Autoscaling. Scale private services using Internal Load Balancing (ILB) for clients in Google Cloud or on-prem across [Interconnect](Interconnect)/[VPN](VPN). 





## How does a load balancer decide where to send requests?

* Round robin: The load balancer distributes connection requests to a pool of servers in a repeating loop, regardless of relative load or capacity. Server A, server B, server C, server A, server B, etc. 
* Weighted round robin: This is like the standard round robin, except for the fact that certain back end servers can be assigned to a higher priority, receiving disproportionally more traffic/requests. Server A, server A, server B, server C, server A, server A, server B, server C, etc. 
* Least connections: This algorithm is fairly self-explanatory; the load balancer sends a new request to the back end server with the least number of active connections. 
* Weighted least connections: This algorithm is like least connections, but certain back end servers can be assigned a higher priority, receiving disproportionally more traffic/requests. In a scenario where some back end servers have a larger or more performant resource configuration, you would use WLC to route them a greater share of the traffic.
* Random: Requests are sent to back end servers in a completely random fashion. No considerations are made for load levels, connection count, etc. 

## Maglev

[Maglev](https://research.google/pubs/pub44824/) is Google's network load balancer. It is [a large distributed software system](https://research.google/pubs/pub44824/) that runs on commodity Linux servers.



## Andromeda

[Andromeda](https://cloud.google.com/blog/products/gcp/enter-andromeda-zone-google-cloud-platforms-latest-networking-stack) is the [network virtualization environment](https://www.usenix.org/system/files/conference/nsdi18/nsdi18-dalton.pdf) for Google Cloud Platform (GCP). 

## Types of Load Balancing

[https://cloud.google.com/load-balancing/docs/load-balancing-overview](https://cloud.google.com/load-balancing/docs/load-balancing-overview)

## Deep dive

[https://cloud.google.com/blog/products/networking/google-cloud-networking-in-depth-cloud-load-balancing-deconstructed](https://cloud.google.com/blog/products/networking/google-cloud-networking-in-depth-cloud-load-balancing-deconstructed)


## Load Balancer Options

To decide which load balancer best suits your implementation of Google Cloud, consider the following aspects of Cloud Load Balancing:

*   Global versus regional load balancing
*   External versus internal load balancing
*   Traffic type

[https://cloud.google.com/load-balancing/docs/choosing-load-balancer](https://cloud.google.com/load-balancing/docs/choosing-load-balancer)

## Kubernetes External Load Balancer

When the Service type is set to LoadBalancer, Kubernetes provides functionality equivalent to type equals ClusterIP to pods within the cluster and extends it by programming the (external to Kubernetes) load balancer with entries for the Kubernetes pods. The Kubernetes service controller automates the creation of the external load balancer, health checks (if needed), firewall rules (if needed) and retrieves the external IP allocated by the cloud provider and populates it in the service object.

https://kubernetes.io/docs/tasks/access-application-cluster/create-external-load-balancer/

Also [ClusterIP, Ingress, NodePort, Load Balancer](ClusterIP,-Ingress,-NodePort,-Load-Balancer) are some of the ways to expose services.



### MetalLB

[MetalLB](https://metallb.universe.tf/) is a load-balancer implementation for bare metal Kubernetes clusters, using standard routing protocols.


Kubernetes does not offer an implementation of network load-balancers (Services of type LoadBalancer) for bare metal clusters. The implementations of Network LB that Kubernetes does ship with are all glue code that calls out to various IaaS platforms (GCP, AWS, Azure…). If you’re not running on a supported IaaS platform (GCP, AWS, Azure…), LoadBalancers will remain in the “pending” state indefinitely when created.

Bare metal cluster operators are left with two lesser tools to bring user traffic into their clusters, “NodePort” and “externalIPs” services. Both of these options have significant downsides for production use, which makes bare metal clusters second class citizens in the Kubernetes ecosystem.

MetalLB aims to redress this imbalance by offering a Network LB implementation that integrates with standard network equipment, so that external services on bare metal clusters also “just work” as much as possible.


## GKE Ingess Load Balancer

In GKE, an Ingress object defines rules for routing HTTP(S) traffic to applications running in a cluster. An Ingress object is associated with one or more Service objects, each of which is associated with a set of Pods. 

https://cloud.google.com/kubernetes-engine/docs/concepts/ingress

## Nginx

Nginx [HTTP Load Balancer](https://docs.nginx.com/nginx/admin-guide/load-balancer/http-load-balancer/) is widely used.
Nginx offers highly scalable performance out of the box and can be extended with additional modules like Lua. 

## Traefik

Traefik can [load balance services](https://doc.traefik.io/traefik/routing/services/).
Traefik bills itself as the “cloud native edge router.” It’s a modern microservices-focused application load balancer and reverse proxy written in Golang. With its emphasis on support for several modern container orchestration platforms, batteries-included logging, and several popular metric formats, Traefik is a top choice for container-based microservices architectures.


## HAProxy


[HAProxy](https://github.com/haproxy/) is another common name in the web ecosystem. HAProxy offers reverse proxying and load balancing of TCP and HTTP traffic. When you choose HAProxy, you’re choosing a high-performance, well-established solution.

## Seesaw


[Seesaw](https://github.com/google/seesaw) is another open-source load balancer written in Golang. It was originally created by Google SREs to provide a robust solution for load balancing internal Google infrastructure traffic. 

## Neutrino

[Neutrino](https://github.com/eBay/Neutrino) is a Scala-based software load balancer originally developed by eBay. Neutrino’s strength lies in the broad compatibility of its runtime environment, the JVM.

## Github Load Balancer Director

Github [Load Balancer Director](https://github.com/github/glb-director)  is a set of components that provide a scalable set of stateless Layer 4 load balancer servers capable of line rate packet processing in bare metal datacenter environments, and is used in production to serve all traffic from GitHub's datacenters.



## List of Load Balancers

A [list](https://github.com/cristaloleg/awesome-load-balancing) of Load Balancers.

