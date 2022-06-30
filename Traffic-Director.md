[Traffic Director](https://cloud.google.com/traffic-director/docs
) is Google Cloud's fully managed application networking platform and service mesh. With Traffic Director, you can deploy global load balancing across clusters and virtual machine (VM) instances in multiple regions, offload health checking from service proxies, and configure sophisticated traffic control policies.

https://cloud.google.com/traffic-director/docs

## Traffic Director and Layer 7 proxies

Traffic Director is toil-free, GCP-managed control plane with SLA for Service Meshes.

In Istio environments, Traffic Director provides a GCP-managed Pilot for your service mesh. 


## Beyond Service Mesh

A common pattern for solving application networking challenges is to use a service mesh. Traffic Director supports service mesh and many other deployment patterns that fit your needs.


In a typical service mesh, the following is true:

- You deploy your services to a Kubernetes cluster.
- Each of the services' Pods has a dedicated proxy (usually Envoy) running as a sidecar proxy.
- Each sidecar proxy talks to the networking infrastructure (a control plane) that is installed in your cluster. The control plane tells the sidecar proxies about services, endpoints, and policies in your service mesh.
- When a Pod sends or receives a request, the request goes to the Pod's sidecar proxy. The sidecar proxy handles the request, for example, by sending it to its intended destination.
- In the diagrams in this document, the six-sided pink icons represent proxies. The control plane is connected to each proxy and provides information that the proxies need to handle requests. Arrows between boxes show traffic flows. For example, application code in Service A sends a request. The proxy handles the request and forwards it to Service B.

This model enables you to move networking logic out of your application code. You can focus on delivering business value while letting your infrastructure take care of application networking.



Traffic Director works similarly to that model, but it's different in important ways. It all starts with the fact that Traffic Director is a Google Cloud-managed service. You don't install it, it doesn't run in your cluster, and you don't need to maintain it.

https://cloud.google.com/traffic-director/docs/overview#how_is_different

Traffic Director supports more types of deployments than a typical service mesh.



https://cloud.google.com/traffic-director/docs/overview#beyond_service_mesh


With Traffic Director, you get application networking that works across Kubernetes clusters.



Kubernetes is becoming increasingly popular, but many workloads are deployed to virtual machine (VM) instances. Traffic Director solves application networking for these workloads, too; your VM-based workloads easily interoperate with your Kubernetes-based workloads.



[gRPC](GRPC) is a feature-rich open source RPC framework that you can use to write high-performance microservices. With Traffic Director, you can easily bring application networking capabilities (such as service discovery, load balancing, and traffic management) to your gRPC applications. For more information, see [Traffic Director and gRPC—proxyless services for your service mesh](https://cloud.google.com/blog/products/networking/traffic-director-supports-proxyless-grpc).




## Apps supported

Traffic Director supports VM-based, Kubernetes and GKE apps.

[https://www.youtube.com/watch?v=FUITCYMCEhU](https://www.youtube.com/watch?v=FUITCYMCEhU)

## Deploying Traffic Director

https://cloud.google.com/traffic-director/docs/install-overview

## Traffic Director with proxyless gRPC services 

https://cloud.google.com/traffic-director/docs/proxyless-overview

## Example

### Proxyless GRPC
https://cloud.google.com/traffic-director/docs/prepare-proxyless-grpc

### Load balancing Google Cloud VMware Engine with Traffic Director
https://cloud.google.com/blog/products/infrastructure-modernization/optimize-front-end-performance-for-gcve