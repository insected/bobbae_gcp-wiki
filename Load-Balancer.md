
[Cloud Load Balancing](https://cloud.google.com/load-balancing) allows you to put your resources behind a single IP address that is externally accessible or internal to your Virtual Private Cloud (VPC) network.

[Cloud Load Balancing](https://cloud.google.com/load-balancing/docs) can put your resources behind a single [anycast](https://en.wikipedia.org/wiki/Anycast) IP and scale your resources up or down with intelligent autoscaling. Cloud Load Balancing comes in a variety of flavors and is integrated with [Cloud CDN](CDN) for optimal application and content delivery.


A [Video](https://www.youtube.com/watch?v=D4XZkCJyqis) about Cloud Load Balancing.


Google Cloud Load Balancing enables enterprises and cloud-natives to deliver highly available, scalable, low-latency cloud services with a global footprint. Use Google Global Load Balancing to deliver [global reach and scale](https://www.youtube.com/watch?v=J5HJ1y6PeyE). Deploy your application backends in single or multiple regions wherever your users are, front-ending these with a single anycast VIP, and growing or shrinking your backend resources with intelligent Autoscaling. Scale private services using Internal Load Balancing (ILB) for clients in Google Cloud or on-prem across [Interconnect](Interconnect)/[VPN](VPN). 

## Basics

https://medium.com/google-cloud/understand-cloud-load-balancer-like-a-senior-engineer-d4f55f3111fc

## Ingress and Load balancer

In GKE, an [Ingress](Ingress) object defines rules for routing HTTP(S) traffic to applications running in a cluster. An Ingress object is associated with one or more Service objects, each of which is associated with a set of Pods. To learn more about how Ingress exposes applications using Services, see Service networking overview.

When you create an Ingress object, the [GKE Ingress controller](https://github.com/kubernetes/ingress-gce) creates a [Google Cloud HTTP(S) Load Balancer](https://cloud.google.com/load-balancing/docs/https) and configures it according to the information in the Ingress and its associated Services.

To use Ingress, you must have the HTTP load balancing add-on enabled. GKE clusters have HTTP load balancing enabled by default; you must not disable it.



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

https://blog.acolyer.org/2018/05/02/andromeda-performance-isolation-and-velocity-at-scale-in-cloud-network-virtualization/

## Types of Load Balancing

[https://cloud.google.com/load-balancing/docs/load-balancing-overview](https://cloud.google.com/load-balancing/docs/load-balancing-overview)

### 7 Types of Google Cloud Load Balancers

https://faun.pub/understand-gcp-7-types-of-load-balancers-and-their-limitations-in-less-than-10-minutes-f877d0212664

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

[MetalLB](MetalLB) is a load-balancer implementation for bare metal Kubernetes clusters, using standard routing protocols.





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

## Reverse Proxy vs Load Balancer


Reverse proxy servers and load balancers are components in a client-server computing architecture. Both act as intermediaries in the communication between the clients and servers, performing functions that improve efficiency. They can be implemented as dedicated, purpose-built devices, but increasingly in modern web architectures they are software applications that run on commodity hardware.

- A reverse proxy accepts a request from a client, forwards it to a server that can fulfill it, and returns the server’s response to the client. Sits at the edge and mitigates DDoS, implement blacklisting, or limit number of connections per each client. Scale number of servers up and down to match load. Aid in web acceleration via Compression, SSL termination, and Caching. Can be deployed with only one backend server.
- A load balancer distributes incoming client requests among a group of servers, in each case returning the response from the selected server to the appropriate client. Usually deployed in front of multiple servers. Most servers host the same content and work is distributed to them. Reduce the number of responses by detecting when servers go down and divert requests away from them to others. LB performs health check. Provide session persistence/affinity. Even though HTTP is stateless, many applications store state information.

Some software and hardware solutions perform both LB and Reverse Proxy functions.

https://www.nginx.com/resources/glossary/reverse-proxy-vs-load-balancer/

https://www.f5.com/services/resources/glossary/reverse-proxy


## Internal TCP/UDP load balancers as next hops 

https://cloud.google.com/load-balancing/docs/internal/ilb-next-hop-overview

https://medium.com/@ozcosta/google-cloud-networking-ilb-as-next-hop-with-tags-ab5f30a0e0c3


## Serverless Load Balancer with Terraform

https://engineering.premise.com/tutorial-managing-serverless-gcp-load-balancers-dynamically-with-terraform-e15751853312

## List of Load Balancers

A [list](https://github.com/cristaloleg/awesome-load-balancing) of Load Balancers.

## Examples

### HTTPS load balancer for Cloud function, Cloud run and App engine

https://cloud.google.com/load-balancing/docs/https/setting-up-https-serverless#gcloud

### Terraform examples for external HTTP(S) load balancers

https://cloud.google.com/load-balancing/docs/https/ext-http-lb-tf-module-examples#cloud-run


### Multiple SSL certificates in HTTPS load balancing with Ingress 

https://cloud.google.com/kubernetes-engine/docs/how-to/ingress-multi-ssl