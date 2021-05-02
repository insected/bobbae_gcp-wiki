
# Introduction

Cloud Load Balancing allows you to put your resources behind a single IP address that is externally accessible or internal to your Virtual Private Cloud (VPC) network.

[https://cloud.google.com/load-balancing/docs](https://cloud.google.com/load-balancing/docs)

A Video about Cloud Load Balancing.

[https://www.youtube.com/watch?v=D4XZkCJyqis](https://www.youtube.com/watch?v=D4XZkCJyqis)

Google Cloud Load Balancing enables enterprises and cloud-natives to deliver highly available, scalable, low-latency cloud services with a global footprint. Use Google Global Load Balancing to deliver global reach and scale. Deploy your application backends in single or multiple regions wherever your users are, front-ending these with a single anycast VIP, and growing or shrinking your backend resources with intelligent Autoscaling. Scale private services using Internal Load Balancing (ILB) for clients in Google Cloud or on-prem across Interconnect/VPN. 

[https://www.youtube.com/watch?v=J5HJ1y6PeyE](https://www.youtube.com/watch?v=J5HJ1y6PeyE)


# Types of Load Balancing

[https://cloud.google.com/load-balancing/docs/load-balancing-overview](https://cloud.google.com/load-balancing/docs/load-balancing-overview)

[https://cloud.google.com/blog/products/networking/google-cloud-networking-in-depth-cloud-load-balancing-deconstructed](https://cloud.google.com/blog/products/networking/google-cloud-networking-in-depth-cloud-load-balancing-deconstructed)


# Maglev

Maglev is Google's network load balancer. It is a large distributed software system that runs on commodity Linux servers.

[https://research.google/pubs/pub44824/](https://research.google/pubs/pub44824/)


# Andromeda

Andromeda is the network virtualization environment for Google Cloud Platform (GCP). 

[https://www.usenix.org/system/files/conference/nsdi18/nsdi18-dalton.pdf](https://www.usenix.org/system/files/conference/nsdi18/nsdi18-dalton.pdf)


# Load Balancer Options

To decide which load balancer best suits your implementation of Google Cloud, consider the following aspects of Cloud Load Balancing:

*   Global versus regional load balancing
*   External versus internal load balancing
*   Traffic type

[https://cloud.google.com/load-balancing/docs/choosing-load-balancer](https://cloud.google.com/load-balancing/docs/choosing-load-balancer)

# Kubernetes External Load Balancer

When the Service type is set to LoadBalancer, Kubernetes provides functionality equivalent to type equals ClusterIP to pods within the cluster and extends it by programming the (external to Kubernetes) load balancer with entries for the Kubernetes pods. The Kubernetes service controller automates the creation of the external load balancer, health checks (if needed), firewall rules (if needed) and retrieves the external IP allocated by the cloud provider and populates it in the service object.

https://kubernetes.io/docs/tasks/access-application-cluster/create-external-load-balancer/

Also [ClusterIP, Ingress, NodePort, Load Balancer](ClusterIP,-Ingress,-NodePort,-Load-Balancer) are some of the ways to expose services.

# GKE Ingess Load Balancer

In GKE, an Ingress object defines rules for routing HTTP(S) traffic to applications running in a cluster. An Ingress object is associated with one or more Service objects, each of which is associated with a set of Pods. 

https://cloud.google.com/kubernetes-engine/docs/concepts/ingress
