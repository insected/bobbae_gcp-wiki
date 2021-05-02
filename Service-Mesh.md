# What is Service Mesh?


Enterprises are increasingly adopting microservices to enable new levels of IT agility, scale, and innovation — but a successful microservices implementation is notoriously complicated. As the number of services an organization uses grows, complexity and risk can increase rapidly. Moreover, microservices need to be exposed as APIs to enable seamless access for internal groups — or with external partners to increase operational efficiency and speed up development. 

A service mesh is a tool for adding observability, security, and reliability features to applications by inserting these features at the platform layer rather than the application layer.

The term service mesh is used to describe the network of microservices that make up such applications and the interactions between them. As a service mesh grows in size and complexity, it can become harder to understand and manage. Its requirements can include discovery, load balancing, failure recovery, metrics, and monitoring. A service mesh also often has more complex operational requirements, like A/B testing, canary rollouts, rate limiting, access control, and end-to-end authentication.

The service mesh is typically implemented as a scalable set of network proxies deployed alongside application code (a pattern sometimes called a sidecar). These proxies handle the communication between the microservices and also act as a point at which the service mesh features can be introduced. The proxies comprise the service mesh’s data plane, and are controlled as a whole by its control plane.

The rise of the service mesh is tied to the rise of the “cloud native” application. In the cloud native world, an application might consist of hundreds of services; each service might have thousands of instances; and each of those instances might be in a constantly-changing state as they are dynamically scheduled by an orchestrator like Kubernetes. Not only is service-to-service communication in this world incredibly complex, it’s a fundamental part of the application’s runtime behavior

### Sidecar proxy


A sidecar proxy is an application design pattern which abstracts certain features, such as inter-service communications, monitoring and security, away from the main architecture to ease the tracking and maintenance of the application as a whole.

Nginx and envoy are common proxies used this way and controlled by service mesh controllers. 

[L7 Proxies](L7-Proxies)


### Service Mesh Manifesto

https://buoyant.io/service-mesh-manifesto/

### Comparisons

https://logz.io/blog/istio-linkerd-consul-comparison-service-meshes/


## Istio

Istio is an open source service mesh that helps organizations run distributed, microservices-based apps anywhere. Why use Istio? Istio enables organizations to secure, connect, and monitor microservices, so they can modernize their enterprise apps more swiftly and securely.

Istio is a service mesh—a modernized service networking layer that provides a transparent and language-independent way to flexibly and easily automate application network functions. It is a popular solution for managing the different microservices that make up a cloud-native application. Istio service mesh also supports how those microservices communicate and share data with one another.

As organizations accelerate their moves to the cloud, they are, by necessity, modernizing their applications as well. But shifting from monolithic legacy apps to cloud-native ones can raise challenges for DevOps teams.

Developers must learn to assemble apps using loosely coupled microservices to ensure portability in the cloud. At the same time, ops teams must manage the new cloud-native apps within increasingly large hybrid and multi-cloud environments. Istio allows them to do this.

### Istiod vs microservices


The term service mesh is used to describe the network of microservices that make up such applications and the interactions between them. As a service mesh grows in size and complexity, it can become harder to understand and manage. Its requirements can include discovery, load balancing, failure recovery, metrics, and monitoring. A service mesh also often has more complex operational requirements, like A/B testing, canary rollouts, rate limiting, access control, and end-to-end authentication.


Istio provides behavioral insights and operational control over the service mesh as a whole, offering a complete solution to satisfy the diverse requirements of microservice applications.



[https://blog.christianposta.com/microservices/istio-as-an-example-of-when-not-to-do-microservices/](https://blog.christianposta.com/microservices/istio-as-an-example-of-when-not-to-do-microservices/)

## Anthos Service Mesh

Anthos Service Mesh is a suite of tools that helps you monitor and manage a reliable service mesh on-premises or on Google Cloud.

https://cloud.google.com/service-mesh/docs/overview




## Envoy

Envoy is  a L7 edge service Proxy used widely by service mesh controllers such as Consul, Contour and istio. Envoy is also used by API gateway like Ambassador.

[Watch a Video about Borg, Cloud Load Balancing, Kubernetes and Envoy into service mesh driven by Istio](https://www.youtube.com/watch?v=glATqKI-WR8).



There are many [Open source projects built on Envoy Proxy](https://www.envoyproxy.io/community).

[Events in the life of a request](https://www.envoyproxy.io/docs/envoy/latest/intro/life_of_a_request) passing through an Envoy proxy is complicated.
How a request flows through the components in a network depends on the network topology. Envoy can be used in a wide variety of networking topologies. Envoy originated as a service mesh sidecar proxy, factoring out load balancing, routing, observability, security and discovery services from applications. In the service mesh model, requests flow through Envoys as a gateway to the network. Requests arrive at an Envoy via either ingress or egress listeners.  

## Apigee Envoy

Wanting to know how to use Envoy to protect your microservices? In this video, we give you a demo on how to enforce policies for any microservice within a service mesh via the Apigee adapter for Envoy. Watch to learn about this tool, and see if it’s the best choice for your specific use case! 

[https://www.youtube.com/watch?v=BNkfoZt-jvU](https://www.youtube.com/watch?v=BNkfoZt-jvU)


## Ambassador Edge Stack and Consul Service Mesh

[Consul](https://www.consul.io/)  is a widely used service mesh. You can use Consul with [Ambassador Edge Stack](https://www.getambassador.io/docs/), as it natively supports Consul for service discovery and end-to-end TLS (including mTLS between services). This capability is particularly useful when deploying Ambassador Edge Stack in so-called hybrid clouds, where applications are deployed on VMs and Kubernetes. In this environment, Ambassador Edge Stack can securely route over TLS to any application regardless of where it is deployed.


[https://www.youtube.com/watch?v=XW3AXQfAaQc](https://www.youtube.com/watch?v=XW3AXQfAaQc)


## Linkerd

https://linkerd.io/

[https://www.youtube.com/watch?v=Bj7gGQUiDuk](https://www.youtube.com/watch?v=Bj7gGQUiDuk)

Linkerd and istio comparison. 

https://www.infracloud.io/blogs/service-mesh-comparison-istio-vs-linkerd/

## Multi-cluster services

Multi-cluster Services (MCS)  is a cross-cluster Service discovery and invocation mechanism for Google Kubernetes Engine (GKE) that leverages the existing Service object. Services enabled with this feature are discoverable and accessible across clusters with a virtual IP, matching the behavior of a ClusterIP Service accessible in a cluster. Just like your existing Services, MCS is compatible with community-driven and open APIs, ensuring your workloads remain portable.

https://cloud.google.com/kubernetes-engine/docs/concepts/multi-cluster-services

### Configuring GKE MCS

The Google Kubernetes Engine (GKE) MCS feature extends the reach of the Kubernetes Service beyond the cluster boundary and lets you discover and invoke Services across multiple GKE clusters. You can export a subset of existing Services or new Services.

https://cloud.google.com/kubernetes-engine/docs/how-to/multi-cluster-services

### Multi-cluster ingress

Multi-cluster Ingress (MCI) is a cloud-hosted multi-cluster Ingress controller for Anthos clusters. It's a Google-hosted service that supports deploying shared load balancing resources across clusters and across regions.

https://cloud.google.com/kubernetes-engine/docs/how-to/multi-cluster-ingress-setup


