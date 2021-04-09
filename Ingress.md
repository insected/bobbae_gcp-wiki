# Ingress

Ingress may provide load balancing, SSL termination and name-based virtual hosting.

Ingress exposes HTTP and HTTPS routes from outside the cluster to services within the cluster. Traffic routing is controlled by rules defined on the Ingress resource.

A Kubernetes Ingress is not a type of Service. It is a collection of rules. An Ingress Controller in your cluster watches for Ingress resources, and attempts to update the server side configuration according to the rules specified in the Ingress.

https://kubernetes.io/docs/concepts/services-networking/ingress/

## The Ingress resource 

[An example](https://raw.githubusercontent.com/kubernetes/website/master/content/en/examples/service/networking/minimal-ingress.yaml).

## List of Ingress Controllers

In order for the Ingress resource to work, the cluster must have an ingress controller running.

Unlike other types of controllers which run as part of the kube-controller-manager binary, Ingress controllers are not started automatically with a cluster. Use this page to choose the ingress controller implementation that best fits your cluster.

https://kubernetes.io/docs/concepts/services-networking/ingress-controllers/

## Load Balancing

An Ingress controller is bootstrapped with some load balancing policy settings that it applies to all Ingress, such as the load balancing algorithm, backend weight scheme, and others. More advanced load balancing concepts (e.g. persistent sessions, dynamic weights) are not yet exposed through the Ingress. You can instead get these features through the load balancer used for a Service.

## Alternatives


You can expose a Service in multiple ways that don't directly involve the Ingress resource:

* Use [Service.Type=LoadBalancer](https://kubernetes.io/docs/concepts/services-networking/service/#loadbalancer)
* Use [Service.Type=NodePort](https://kubernetes.io/docs/concepts/services-networking/service/#nodeport)




