# What is Service Mesh?

A service mesh is a tool for adding observability, security, and reliability features to applications by inserting these features at the platform layer rather than the application layer.

The term service mesh is used to describe the network of microservices that make up such applications and the interactions between them. As a service mesh grows in size and complexity, it can become harder to understand and manage. Its requirements can include discovery, load balancing, failure recovery, metrics, and monitoring. A service mesh also often has more complex operational requirements, like A/B testing, canary rollouts, rate limiting, access control, and end-to-end authentication.

The service mesh is typically implemented as a scalable set of network proxies deployed alongside application code (a pattern sometimes called a sidecar). These proxies handle the communication between the microservices and also act as a point at which the service mesh features can be introduced. The proxies comprise the service mesh’s data plane, and are controlled as a whole by its control plane.

The rise of the service mesh is tied to the rise of the “cloud native” application. In the cloud native world, an application might consist of hundreds of services; each service might have thousands of instances; and each of those instances might be in a constantly-changing state as they are dynamically scheduled by an orchestrator like Kubernetes. Not only is service-to-service communication in this world incredibly complex, it’s a fundamental part of the application’s runtime behavior

### sidecar proxy


A sidecar proxy is an application design pattern which abstracts certain features, such as inter-service communications, monitoring and security, away from the main architecture to ease the tracking and maintenance of the application as a whole.

Nginx and envoy are common proxies used this way and controlled by service mesh controllers. 

### Service Mesh Manifesto

https://buoyant.io/service-mesh-manifesto/

### Comparisons

https://logz.io/blog/istio-linkerd-consul-comparison-service-meshes/


## Istio

Istio is an open source service mesh that helps organizations run distributed, microservices-based apps anywhere. Why use Istio? Istio enables organizations to secure, connect, and monitor microservices, so they can modernize their enterprise apps more swiftly and securely.

Istio is a service mesh—a modernized service networking layer that provides a transparent and language-independent way to flexibly and easily automate application network functions. It is a popular solution for managing the different microservices that make up a cloud-native application. Istio service mesh also supports how those microservices communicate and share data with one another.

As organizations accelerate their moves to the cloud, they are, by necessity, modernizing their applications as well. But shifting from monolithic legacy apps to cloud-native ones can raise challenges for DevOps teams.

Developers must learn to assemble apps using loosely coupled microservices to ensure portability in the cloud. At the same time, ops teams must manage the new cloud-native apps within increasingly large hybrid and multi-cloud environments. Istio allows them to do this.

## Anthos Service Mesh

Anthos Service Mesh is a suite of tools that helps you monitor and manage a reliable service mesh on-premises or on Google Cloud.

https://cloud.google.com/service-mesh/docs/overview

