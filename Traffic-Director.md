[Traffic Director](https://cloud.google.com/traffic-director/docs
) is Google Cloud's fully managed application networking platform and service mesh. With Traffic Director, you can deploy global load balancing across clusters and virtual machine (VM) instances in multiple regions, offload health checking from service proxies, and configure sophisticated traffic control policies.

https://cloud.google.com/traffic-director/docs

## Traffic Director and Layer 7 proxies

Traffic Director is toil-free, GCP-managed control plane with SLA for Service Meshes.

In Istio environments, Traffic Director provides a GCP-managed Pilot for your service mesh. 

Traffic Director delivers traffic management and multi-region global load balancing for service meshes built using open proxies like Envoy and through the open xDSv2 APIs. It provides policy driven traffic routing, enabling you to control the flow of traffic between services. All of this makes load balancing, scaling, A/B testing, canary roll outs, and blue-green deployments easy  to set up. Traffic Director also provides centralized high fidelity health checking, and traffic driven autoscaling. Envoy-based Layer 7 Internal Load Balancing (L7 ILB), another flavor of Traffic Director, brings modern traffic management capabilities to traditional environments. With L7 ILB, Traffic Director controls a pool of GCP-managed Envoy proxies under the hood but presents this service as a traditional Layer 7 ILB middle proxy to front your legacy apps. 

## Beyond Service Mesh

A common pattern for solving application networking challenges is to use a service mesh. Traffic Director supports service mesh and many other deployment patterns that fit your needs.



[[https://cloud.google.com/traffic-director/images/service-mesh.svg]]

In a typical service mesh, the following is true:

- You deploy your services to a Kubernetes cluster.
- Each of the services' Pods has a dedicated proxy (usually Envoy) running as a sidecar proxy.
- Each sidecar proxy talks to the networking infrastructure (a control plane) that is installed in your cluster. The control plane tells the sidecar proxies about services, endpoints, and policies in your service mesh.
- When a Pod sends or receives a request, the request goes to the Pod's sidecar proxy. The sidecar proxy handles the request, for example, by sending it to its intended destination.
- In the diagrams in this document, the six-sided pink icons represent proxies. The control plane is connected to each proxy and provides information that the proxies need to handle requests. Arrows between boxes show traffic flows. For example, application code in Service A sends a request. The proxy handles the request and forwards it to Service B.

This model enables you to move networking logic out of your application code. You can focus on delivering business value while letting your infrastructure take care of application networking.



Traffic Director works similarly to that model, but it's different in important ways. It all starts with the fact that Traffic Director is a Google Cloud-managed service. You don't install it, it doesn't run in your cluster, and you don't need to maintain it.

In the following diagram, Traffic Director is the control plane. There are four services in this Kubernetes cluster, each with sidecar proxies that are connected to Traffic Director. Traffic Director provides the information that the proxies need to route requests. For example, application code on a Pod that belongs to Service A sends a request. The sidecar proxy running alongside this Pod handles the request and routes it to a Pod that belongs to Service B.


[[https://cloud.google.com/traffic-director/images/service-mesh-td.svg]]

https://cloud.google.com/traffic-director/docs/overview#how_is_different

Traffic Director supports more types of deployments than a typical service mesh.



https://cloud.google.com/traffic-director/docs/overview#beyond_service_mesh


With Traffic Director, you get application networking that works across Kubernetes clusters. In the following diagram, Traffic Director provides the control plane for Kubernetes clusters in us-central1 and europe-west1. Requests can be routed among the three services in us-central1, among the two services in europe-west1, and between services in the two clusters.

[[https://cloud.google.com/traffic-director/images/multi-cluster-service-mesh.svg]]


Kubernetes is becoming increasingly popular, but many workloads are deployed to virtual machine (VM) instances. Traffic Director solves application networking for these workloads, too; your VM-based workloads easily interoperate with your Kubernetes-based workloads.

In the following diagram, traffic enters your deployment through External HTTP(S) Load Balancing. It is routed to Service A in the Kubernetes cluster in asia-southeast1 and to Service D on a VM in europe-west1.



[[https://cloud.google.com/traffic-director/images/vms-kubernetes.svg]]


[gRPC](GRPC) is a feature-rich open source RPC framework that you can use to write high-performance microservices. With Traffic Director, you can easily bring application networking capabilities (such as service discovery, load balancing, and traffic management) to your gRPC applications. For more information, see [Traffic Director and gRPC—proxyless services for your service mesh](https://cloud.google.com/blog/products/networking/traffic-director-supports-proxyless-grpc).

In the following diagram, gRPC applications route traffic to services based in Kubernetes clusters in one region and to services running on VMs in different regions. Two of the services include sidecar proxies, and the others are proxyless.


[[https://cloud.google.com/traffic-director/images/proxyless-grpc.svg]]



## Apps supported

Traffic Director supports VM-based, Kubernetes and GKE apps.

[https://www.youtube.com/watch?v=FUITCYMCEhU](https://www.youtube.com/watch?v=FUITCYMCEhU)

## Deploying Traffic Director

https://cloud.google.com/traffic-director/docs/install-overview

## Example

https://cloud.google.com/traffic-director/docs/prepare-proxyless-grpc