
[MetalLB](https://metallb.universe.tf/) is a load-balancer implementation for bare metal Kubernetes clusters, using standard routing protocols.

[Kubernetes](Kubernetes) does not offer an implementation of network [load-balancers](Load-Balancer) (Services of type LoadBalancer) for bare metal clusters. The implementations of Network LB that Kubernetes does ship with are all glue code that calls out to various IaaS platforms (GCP, AWS, Azure…). If you’re not running on a supported IaaS platform (GCP, AWS, Azure…), LoadBalancers will remain in the “pending” state indefinitely when created.

[Bare metal cluster operators](https://metal.equinix.com/developers/guides/kube-vip-type-lb/) are left with two lesser tools to bring user traffic into their clusters, “NodePort” and “externalIPs” services. Both of these options have significant downsides for production use, which makes bare metal clusters second class citizens in the Kubernetes ecosystem.

[MetalLB](https://metallb.universe.tf/) aims to redress this imbalance by offering a Network LB implementation that integrates with standard network equipment, so that external services on bare metal clusters also “just work” as much as possible.


### Kube-vip

https://github.com/kube-vip/kube-vip


[Kube-Vip](https://kube-vip.io) was originally created to provide a HA solution for the Kubernetes control plane, over time it has evolved to incorporate that same functionality into Kubernetes service type load-balancers.


#### Equinix example

https://metal.equinix.com/developers/guides/kube-vip-type-lb/


#### Anthos on Bare metal with Kube-vip

https://github.com/equinix/terraform-metal-anthos-on-baremetal
