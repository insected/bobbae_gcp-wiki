

[Cloud VPN](https://cloud.google.com/network-connectivity/docs/vpn) securely extends your [peer](https://cloud.google.com/network-connectivity/docs/vpn/concepts/key-terms#peer-definition) network to Google's network through an [IPsec](https://en.wikipedia.org/wiki/IPsec) VPN tunnel. Traffic is encrypted and travels between the two networks over the public internet. 

https://cloud.google.com/network-connectivity/docs/vpn

If you need an enterprise-grade connection to Google Cloud that has higher throughput, you can choose Dedicated [Interconnect](Interconnect) or Partner Interconnect.

https://cloud.google.com/network-connectivity/docs/how-to/choose-product#compare-interconnect-solutions

https://cloud.google.com/architecture/patterns-for-connecting-other-csps-with-gcp

Cloud VPN is easy to set up and cheaper than other interconnect options.

https://cloud.google.com/network-connectivity/docs/vpn/concepts/overview#specifications

https://cloud.google.com/network-connectivity/pricing

## Cloud Interconnect
https://cloud.google.com/network-connectivity/docs/how-to/choose-product#cloud-interconnect

## Private Google Access for on-premises hosts

https://cloud.google.com/vpc/docs/private-google-access-hybrid

## Shared VPC
https://cloud.google.com/vpc/docs/shared-vpc

## Network Connectivity

https://cloud.google.com/network-connectivity/docs/concepts

## Types of Cloud VPN


### Classic VPN

[ Classic VPN ](https://cloud.google.com/network-connectivity/docs/vpn/concepts/overview#classic-vpn)gateways have a single interface, a single external IP address, and support tunnels that use dynamic (BGP) or static routing (policy-based or route-based). They provide an SLA of 99.9% service availability.


### HA VPN

[HA VPN](https://cloud.google.com/network-connectivity/docs/vpn/concepts/overview#ha-vpn) lets you easily set up redundant VPNs to isolate failures and provide continuous connectivity for workloads that are too important to fail. 

Use Case 1: Migrate an existing Classic VPN solution to HA VPN utilizing BGP as the routing protocol to an on-premises network (or any non Google Networks). Use Case 2: Migrate an existing Classic VPN utilizing policy based VPN to HA VPN utilizing BGP between two projects or VPCs within Google Cloud Platform.

[https://www.youtube.com/watch?v=lIEExVWf5bg](https://www.youtube.com/watch?v=lIEExVWf5bg)

If a Cloud VPN tunnel goes down, it restarts automatically. If an entire virtual VPN device fails, Cloud VPN automatically instantiates a new one with the same configuration. The new gateway and tunnel connect automatically.

VPN tunnels connected to HA VPN gateways must use dynamic (BGP) routing. Depending on the way that you configure route priorities for HA VPN tunnels, you can create an active/active or active/passive routing configuration. For both of these routing configurations, both VPN tunnels remain active.

https://cloud.google.com/network-connectivity/docs/vpn/concepts/topologies


## Active/active vs. active/passive routing options for HA VPN

[https://cloud.google.com/network-connectivity/docs/vpn/concepts/overview#active](https://cloud.google.com/network-connectivity/docs/vpn/concepts/overview#active)


## Comparison between HA VPN and Classic VPN

[https://cloud.google.com/network-connectivity/docs/vpn/concepts/overview#comparison_table](https://cloud.google.com/network-connectivity/docs/vpn/concepts/overview#comparison_table)


## Organization policy and VPC service controls

### Constraints
https://cloud.google.com/resource-manager/docs/organization-policy/org-policy-constraints#constraints-for-specific-services

### VPC service controls
https://cloud.google.com/vpc-service-controls/docs/overview

### Service perimeter
https://cloud.google.com/vpc-service-controls/docs/overview#isolate

## BYOIP - Bring your own IP

https://cloud.google.com/vpc/docs/bring-your-own-ip#planning

## Limiting use of external IP

https://cloud.google.com/architecture/best-practices-vpc-design#limit-access

https://cloud.google.com/architecture/building-internet-connectivity-for-private-vms

## IP address management
https://cloud.google.com/architecture/gke-ip-address-mgmt-strategies





## Cloud VPN Topologies

With Cloud VPN, your on-premises hosts communicate through one or more IPsec VPN tunnels to Compute Engine Virtual Machine (VM) instances in your project's VPC networks.

[https://cloud.google.com/network-connectivity/docs/vpn/concepts/topologies](https://cloud.google.com/network-connectivity/docs/vpn/concepts/topologies)


## HA VPN to peer VPN Gateways

[https://cloud.google.com/network-connectivity/docs/vpn/concepts/topologies#to_peer_vpn_gateways](https://cloud.google.com/network-connectivity/docs/vpn/concepts/topologies#to_peer_vpn_gateways)


## HA VPN to AWS peer Gateways

[https://cloud.google.com/network-connectivity/docs/vpn/concepts/topologies#to_aws_peer_gateways](https://cloud.google.com/network-connectivity/docs/vpn/concepts/topologies#to_aws_peer_gateways)


## HA VPN between Google Cloud networks

[https://cloud.google.com/network-connectivity/docs/vpn/concepts/topologies#2-gcp-gateways](https://cloud.google.com/network-connectivity/docs/vpn/concepts/topologies#2-gcp-gateways)

## Advanced configurations

You can create a VPN tunnel that has the same IP range as another tunnel, a subset of the other tunnel's range, or a superset of the other tunnel's range.

For details, see [Order of routes](https://cloud.google.com/network-connectivity/docs/vpn/concepts/order-of-routes).




In [Networks and tunnel routing](https://cloud.google.com/network-connectivity/docs/vpn/concepts/choosing-networks-routing), you can find information about supported Virtual Private Cloud (VPC) networks and routing options, including traffic selectors.


### Generating a strong pre-shared key

https://cloud.google.com/network-connectivity/docs/vpn/how-to/generating-pre-shared-key


## VPN Terms
https://cloud.google.com/network-connectivity/docs/vpn/concepts/key-terms

## Comparisons of different kinds of VPNs


https://www.ivpn.net/pptp-vs-ipsec-ikev2-vs-openvpn-vs-wireguard/

## NSA and VPN

https://www.schneier.com/blog/archives/2020/07/nsa_on_securing.html


## Interopating with third-party VPNs

https://cloud.google.com/network-connectivity/docs/vpn/how-to/interop-guides


## Examples

### Simulated on-prem for GCP VPN

https://medium.com/@sruffilli/setting-up-a-simulated-on-prem-environment-for-gcp-90dcbb2d57f8

### Creating a Cloud VPN connection to a remote site 
https://cloud.google.com/network-connectivity/docs/vpn/tutorials/configure-vpn-between-onprem-cloud

### Deploy HA VPN with Terraform
https://cloud.google.com/community/tutorials/deploy-ha-vpn-with-terraform

### Multicloud VPN - GCP-AWS VPN

https://github.com/GoogleCloudPlatform/autonetdeploy-multicloudvpn

### Creating an HA VPN gateway to a peer VPN gateway 
https://cloud.google.com/network-connectivity/docs/vpn/how-to/creating-ha-vpn

### Terraform examples for HA VPN gateways

https://cloud.google.com/network-connectivity/docs/vpn/how-to/automate-vpn-setup-with-terraform


### Configuring the peer VPN gateway

https://cloud.google.com/network-connectivity/docs/vpn/how-to/configuring-peer-gateway

### Creating a Classic VPN using static routing

https://cloud.google.com/network-connectivity/docs/vpn/how-to/creating-static-vpns