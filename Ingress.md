

[Ingress](https://kubernetes.io/docs/concepts/services-networking/ingress/) may provide load balancing, SSL termination and name-based virtual hosting.

[Ingress](https://cloud.google.com/kubernetes-engine/docs/concepts/ingress) exposes HTTP and HTTPS routes from outside the cluster to services within the cluster. Traffic routing is controlled by rules defined on the Ingress resource.



## GCP Ingress

### Ingress for GKE

https://cloud.google.com/kubernetes-engine/docs/concepts/ingress


### Ingress for External HTTP(S) Load Balancing


https://cloud.google.com/kubernetes-engine/docs/concepts/ingress-xlb


### Ingress for Internal HTTP(S) Load Balancing

https://cloud.google.com/kubernetes-engine/docs/concepts/ingress-ilb


### Multi cluster ingress

https://cloud.google.com/kubernetes-engine/docs/concepts/multi-cluster-ingress


### Comparison of Ingress and Gateway

https://cloud.google.com/kubernetes-engine/docs/concepts/gateway-api#comparison_of_ingress_and_gateway


## GCP Network Endpoint Groups

In GCP, a Network Endpoint Group (NEG) is a configuration object that specifies a group of backend endpoints or services. 
A common use case for this configuration is deploying services in containers.
You can also distribute traffic in a granular fashion to applications running on your backend instances.

* Zonal and internet NEGs define how endpoints should be reached, whether they are reachable, and where they are located. Unlike these NEG types, serverless NEGs don't contain endpoints.

* A zonal NEG contains one or more endpoints that can be Compute Engine VMs or services running on the VMs. Each endpoint is specified either by an IP address or an IP:port combination.

* An internet NEG contains a single endpoint that is hosted outside of Google Cloud. This endpoint is specified by hostname FQDN:port or IP:port.

https://cloud.google.com/load-balancing/docs/negs

### Ingress with NEGs

When NEGs are used with GKE Ingress, the Ingress controller facilitates the creation of all aspects of the L7 load balancer. This includes creating the virtual IP address, forwarding rules, health checks, firewall rules, and more.

https://cloud.google.com/kubernetes-engine/docs/how-to/standalone-neg#ingress_with_negs

## Kubernetes Ingress

A [Kubernetes Ingress](  https://kubernetes.io/docs/concepts/services-networking/ingress/ ) is not a type of [Service](  https://kubernetes.io/docs/concepts/services-networking/service/ ). It is a collection of rules. An Ingress Controller in your cluster watches for Ingress resources, and attempts to update the server side configuration according to the rules specified in the Ingress.

Kubernetes ingress is a collection of routing rules that govern how external users access services running in a [Kubernetes cluster](https://www.getambassador.io/docs/edge-stack/latest/topics/concepts/kubernetes-network-architecture/  
) .

In a typical Kubernetes application, you have pods running inside a cluster and a load balancer running outside. The load balancer takes connections from the internet and routes the traffic to an edge proxy that sits inside your cluster. This edge proxy is then responsible for routing traffic into your pods. The [edge proxy](https://www.getambassador.io/docs/edge-stack/latest/topics/concepts/kubernetes-network-architecture/#edge-proxy--ingress-controller) is commonly called an ingress controller because it is commonly configured using ingress resources in Kubernetes, however the edge proxy can also be configured with custom resource definitions (CRDs) or annotations.


You can do a lot of different things with an Ingress, and there are many types of Ingress controllers that have different capabilities.
The default GKE ingress controller will spin up a [HTTP(S) Load Balancer](https://cloud.google.com/compute/docs/load-balancing/http/) for you. This will let you do both path based and subdomain based routing to backend services. For example, you can send everything on foo.yourdomain.com to the foo service, and everything under the yourdomain.com/bar/ path to the bar service.

https://kubernetes.io/docs/concepts/services-networking/ingress/

## The Ingress resource 

An example:

```
apiVersion: networking.k8s.io/v1
kind: Ingress
metadata:
  name: ingress-wildcard-host
spec:
  rules:
  - host: "foo.bar.com"
    http:
      paths:
      - pathType: Prefix
        path: "/bar"
        backend:
          service:
            name: service1
            port:
              number: 80
  - host: "*.foo.com"
    http:
      paths:
      - pathType: Prefix
        path: "/foo"
        backend:
          service:
            name: service2
            port:
              number: 80
```
## List of Ingress Controllers

In order for the Ingress resource to work, the cluster must have an ingress controller running.

Unlike other types of controllers which run as part of the kube-controller-manager binary, Ingress controllers are not started automatically with a cluster. Use this page to choose the ingress controller implementation that best fits your cluster.

https://kubernetes.io/docs/concepts/services-networking/ingress-controllers/


https://liejuntao001.medium.com/some-details-about-how-kubernetes-ingress-controller-works-99deb529f2e4

## Load Balancing

An Ingress controller is bootstrapped with some load balancing policy settings that it applies to all Ingress, such as the load balancing algorithm, backend weight scheme, and others. More advanced load balancing concepts (e.g. persistent sessions, dynamic weights) are not yet exposed through the Ingress. You can instead get these features through the load balancer used for a Service.

## Ingress and Load balancer

In GKE, an Ingress object defines rules for routing HTTP(S) traffic to applications running in a cluster. An Ingress object is associated with one or more Service objects, each of which is associated with a set of Pods. To learn more about how Ingress exposes applications using Services, see Service networking overview.

When you create an Ingress object, the [GKE Ingress controller](https://github.com/kubernetes/ingress-gce) creates a [Google Cloud HTTP(S) Load Balancer](https://cloud.google.com/load-balancing/docs/https) and configures it according to the information in the Ingress and its associated Services.

To use Ingress, you must have the HTTP [load balancing](Load-Balancer) add-on enabled. GKE clusters have HTTP load balancing enabled by default; you must not disable it.



## Alternatives


You can expose a Service in multiple ways that don't directly involve the Ingress resource:

* Use [Service.Type=LoadBalancer](https://kubernetes.io/docs/concepts/services-networking/service/#loadbalancer)
* Use [Service.Type=NodePort](https://kubernetes.io/docs/concepts/services-networking/service/#nodeport)


Services can be [exposed](ClusterIP,-Ingress,-NodePort,-Load-Balancer) in a variety of ways.



## Multi-cluster ingress

Multi-cluster Ingress (MCI) is a cloud-hosted multi-cluster Ingress controller for Anthos clusters. It's a Google-hosted service that supports deploying shared load balancing resources across clusters and across regions.

https://cloud.google.com/kubernetes-engine/docs/how-to/multi-cluster-ingress-setup

## Ingress examples

### Set up an ingress on minikube via nginx

https://kubernetes.io/docs/tasks/access-application-cluster/ingress-minikube/

### Multicluster ingress example

https://faun.pub/multi-cluster-ingress-gke-57be59ced00d