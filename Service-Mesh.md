
https://cloud.google.com/architecture/service-meshes-in-microservices-architecture

## What is Service Mesh?

A service mesh is a platform layer on top of the infrastructure layer that enables managed, observable, and secure communication between individual services.

Enterprises are adopting microservices and [service mesh](https://www.nginx.com/blog/what-is-a-service-mesh/) to enable new levels of IT [agility](https://www.infoworld.com/article/3237508/what-is-agile-methodology-modern-software-development-explained.html) but a successful [microservices](Microservices)  implementation is complicated. As the number of services an organization uses grows, [complexity and risk](https://stackoverflow.blog/2020/11/23/the-macro-problem-with-microservices/) can increase rapidly. The [microservices](https://microservices.io/) need to be exposed as APIs to enable access via features such as discovery, load balancing, failure recovery, metrics, monitoring, [A/B testing](https://en.wikipedia.org/wiki/A/B_testing), [canary rollouts](https://argoproj.github.io/argo-rollouts/features/canary/), rate limiting, access control, and end-to-end authentication.

The [service mesh](https://en.wikipedia.org/wiki/Service_mesh) is typically implemented as a scalable set of network proxies deployed alongside application code (a pattern sometimes called a [sidecar](https://docs.microsoft.com/en-us/azure/architecture/patterns/sidecar). 

The [rise of the service mesh](https://www.talentica.com/blogs/the-rise-of-service-mesh-how-can-businesses-use-it/) is tied to the rise of the [cloud native](https://cloud.google.com/solutions/cloud-native-app-development) application. In the [cloud native world](https://www.cncf.io/), an application might consist of hundreds of services and each service might have thousands of instances and each of those instances might be in a constantly-changing state as they are dynamically scheduled by an orchestrator like [Kubernetes](Kubernetes). 

### Anthos Service Mesh

https://cloud.google.com/anthos/service-mesh

### Anthos
https://cloud.google.com/blog/topics/anthos/anthos-service-mesh-deep-dive

### Sidecar proxy


A [sidecar proxy](https://medium.com/@lukas.eichler/securing-pods-with-sidecar-proxies-d84f8d34be3e) is an application design pattern which abstracts certain features, such as inter-service communications, monitoring and security, away from the main architecture to ease the tracking and maintenance of the application as a whole.

[Nginx](https://en.wikipedia.org/wiki/Nginx) and [Envoy](https://en.wikipedia.org/wiki/Envoy) are common proxies used this way and controlled by service mesh controllers. 

#### L7 Proxies

[L7 Proxies](L7-Proxies) maintain two TCP connections: one with the client and one with the server. The packets are re-assembled then the load-balancer can take a routing decision based on the information it can find in the application requests or responses.

### istio
https://istio.io/

### Service Mesh Manifesto

https://buoyant.io/service-mesh-manifesto/

### Comparisons

https://logz.io/blog/istio-linkerd-consul-comparison-service-meshes/

### When not to use Service Mesh

https://medium.com/google-cloud/when-not-to-use-service-mesh-1a44abdeea31

## Istio

[Istio](https://istio.io/) is an open source service mesh that helps organizations run distributed, microservices-based apps anywhere. Why use Istio? Istio enables organizations to secure, connect, and monitor microservices, so they can modernize their enterprise apps more swiftly and securely.



[https://blog.christianposta.com/microservices/istio-as-an-example-of-when-not-to-do-microservices/](https://blog.christianposta.com/microservices/istio-as-an-example-of-when-not-to-do-microservices/)

## Anthos Service Mesh

[Anthos Service Mesh](https://cloud.google.com/anthos/service-mesh) is a suite of tools that helps you monitor and manage a reliable service mesh on-premises or on Google Cloud.

https://cloud.google.com/service-mesh/docs/overview


https://blog.searce.com/anthos-blog-series-part-1-anthos-service-mesh-a258ba621732

## Envoy

[Envoy](https://www.envoyproxy.io/) is  a L7 edge service Proxy used widely by service mesh controllers such as [Consul](https://www.consul.io/), [Contour](https://projectcontour.io/) and istio. Envoy is also used by API gateway like [Ambassador](https://github.com/datawire/ambassador).

[Watch a Video about Borg, Cloud Load Balancing, Kubernetes and Envoy into service mesh driven by Istio](https://www.youtube.com/watch?v=glATqKI-WR8).



There are many [Open source projects built on Envoy Proxy](https://www.envoyproxy.io/community).

### Life of a request through Envoy proxy

https://www.envoyproxy.io/docs/envoy/latest/intro/life_of_a_request

## Apigee Envoy

Apigee adapter for Envoy. 

[https://www.youtube.com/watch?v=BNkfoZt-jvU](https://www.youtube.com/watch?v=BNkfoZt-jvU)


## Ambassador Edge Stack and Consul Service Mesh

[Consul](https://www.consul.io/)  is a widely used service mesh. You can use Consul with [Ambassador Edge Stack](https://www.getambassador.io/docs/).

[https://www.youtube.com/watch?v=XW3AXQfAaQc](https://www.youtube.com/watch?v=XW3AXQfAaQc)


## Linkerd

https://linkerd.io/

[https://www.youtube.com/watch?v=Bj7gGQUiDuk](https://www.youtube.com/watch?v=Bj7gGQUiDuk)

Linkerd and istio comparison. 

https://www.infracloud.io/blogs/service-mesh-comparison-istio-vs-linkerd/


## KUMA

https://konghq.com/blog/envoy-service-mesh/

## Multi-cluster services

Multi-cluster Services (MCS)  is a cross-cluster Service discovery and invocation mechanism for Google Kubernetes Engine (GKE) that leverages the existing Service object. Services enabled with this feature are discoverable and accessible across clusters with a virtual IP, matching the behavior of a ClusterIP Service accessible in a cluster. 

https://cloud.google.com/kubernetes-engine/docs/concepts/multi-cluster-services

### Configuring GKE MCS

The Google Kubernetes Engine (GKE) MCS feature extends the reach of the Kubernetes Service beyond the cluster boundary and lets you discover and invoke Services across multiple GKE clusters.

https://cloud.google.com/kubernetes-engine/docs/how-to/multi-cluster-services

### Multi-cluster ingress

Multi-cluster Ingress (MCI) is a cloud-hosted multi-cluster Ingress controller for Anthos clusters. It's a Google-hosted service that supports deploying shared load balancing resources across clusters and across regions.

https://cloud.google.com/kubernetes-engine/docs/how-to/multi-cluster-ingress-setup


