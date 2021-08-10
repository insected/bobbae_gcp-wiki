[Traffic Director](https://cloud.google.com/traffic-director/docs
) is Google Cloud's fully managed application networking platform and service mesh. With Traffic Director, you can deploy global load balancing across clusters and virtual machine (VM) instances in multiple regions, offload health checking from service proxies, and configure sophisticated traffic control policies.

https://cloud.google.com/traffic-director/docs

## Traffic Director and Layer 7 proxies

Traffic Director is toil-free, GCP-managed control plane with SLA for Service Meshes.

In Istio environments, Traffic Director provides a GCP-managed Pilot for your service mesh. 

Traffic Director delivers traffic management and multi-region global load balancing for service meshes built using open proxies like Envoy and through the open xDSv2 APIs. It provides policy driven traffic routing, enabling you to control the flow of traffic between services. All of this makes load balancing, scaling, A/B testing, canary roll outs, and blue-green deployments easy  to set up. Traffic Director also provides centralized high fidelity health checking, and traffic driven autoscaling. Envoy-based Layer 7 Internal Load Balancing (L7 ILB), another flavor of Traffic Director, brings modern traffic management capabilities to traditional environments. With L7 ILB, Traffic Director controls a pool of GCP-managed Envoy proxies under the hood but presents this service as a traditional Layer 7 ILB middle proxy to front your legacy apps. 

## Apps supported

Traffic Director supports VM-based, Kubernetes and GKE apps.

[https://www.youtube.com/watch?v=FUITCYMCEhU](https://www.youtube.com/watch?v=FUITCYMCEhU)

## Deploying Traffic Director

https://cloud.google.com/traffic-director/docs/install-overview

## Example

https://cloud.google.com/traffic-director/docs/prepare-proxyless-grpc