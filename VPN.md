
# Introduction

Cloud VPN securely extends your [peer](https://cloud.google.com/network-connectivity/docs/vpn/concepts/key-terms#peer-definition) network to Google's network through an IPsec VPN tunnel. Traffic is encrypted and travels between the two networks over the public internet. Cloud VPN is useful for low-volume data connections.

[https://cloud.google.com/network-connectivity/docs/vpn](https://cloud.google.com/network-connectivity/docs/vpn)


<img src="https://cloud.google.com/network-connectivity/docs/vpn/images/ha-vpn-gcp-to-on-prem-2-a.svg" width="700">

# Types of Cloud VPN


## Classic VPN

[ Classic VPN ](https://cloud.google.com/network-connectivity/docs/vpn/concepts/overview#classic-vpn)gateways have a single interface, a single external IP address, and support tunnels that use dynamic (BGP) or static routing (policy-based or route-based). They provide an SLA of 99.9% service availability.


## HA VPN

[HA VPN](https://cloud.google.com/network-connectivity/docs/vpn/concepts/overview#ha-vpn) lets you easily set up redundant VPNs to isolate failures and provide continuous connectivity for workloads that are too important to fail. 

Use Case 1: Migrate an existing Classic VPN solution to HA VPN utilizing BGP as the routing protocol to an on-premises network (or any non Google Networks). Use Case 2: Migrate an existing Classic VPN utilizing policy based VPN to HA VPN utilizing BGP between two projects or VPCs within Google Cloud Platform.

[https://www.youtube.com/watch?v=lIEExVWf5bg](https://www.youtube.com/watch?v=lIEExVWf5bg)

If a Cloud VPN tunnel goes down, it restarts automatically. If an entire virtual VPN device fails, Cloud VPN automatically instantiates a new one with the same configuration. The new gateway and tunnel connect automatically.

VPN tunnels connected to HA VPN gateways must use dynamic (BGP) routing. Depending on the way that you configure route priorities for HA VPN tunnels, you can create an active/active or active/passive routing configuration. For both of these routing configurations, both VPN tunnels remain active.


# Active/active vs. active/passive routing options for HA VPN

[https://cloud.google.com/network-connectivity/docs/vpn/concepts/overview#active](https://cloud.google.com/network-connectivity/docs/vpn/concepts/overview#active)


# Comparison between HA VPN and Classic VPN

[https://cloud.google.com/network-connectivity/docs/vpn/concepts/overview#comparison_table](https://cloud.google.com/network-connectivity/docs/vpn/concepts/overview#comparison_table)


# Cloud VPN Topologies

With Cloud VPN, your on-premises hosts communicate through one or more IPsec VPN tunnels to Compute Engine Virtual Machine (VM) instances in your project's VPC networks.

[https://cloud.google.com/network-connectivity/docs/vpn/concepts/topologies](https://cloud.google.com/network-connectivity/docs/vpn/concepts/topologies)


# HA VPN to peer VPN Gateways

[https://cloud.google.com/network-connectivity/docs/vpn/concepts/topologies#to_peer_vpn_gateways](https://cloud.google.com/network-connectivity/docs/vpn/concepts/topologies#to_peer_vpn_gateways)


# HA VPN to AWS peer Gateways

[https://cloud.google.com/network-connectivity/docs/vpn/concepts/topologies#to_aws_peer_gateways](https://cloud.google.com/network-connectivity/docs/vpn/concepts/topologies#to_aws_peer_gateways)


# HA VPN between Google Cloud networks

[https://cloud.google.com/network-connectivity/docs/vpn/concepts/topologies#2-gcp-gateways](https://cloud.google.com/network-connectivity/docs/vpn/concepts/topologies#2-gcp-gateways)

# Advanced configurations

You can create a VPN tunnel that has the same IP range as another tunnel, a subset of the other tunnel's range, or a superset of the other tunnel's range.

For details, see [Order of routes](https://cloud.google.com/network-connectivity/docs/vpn/concepts/order-of-routes).




In [Networks and tunnel routing](https://cloud.google.com/network-connectivity/docs/vpn/concepts/choosing-networks-routing), you can find information about supported Virtual Private Cloud (VPC) networks and routing options, including traffic selectors.

# IPSec & Cryptography

https://github.com/bobbae/gcp/wiki/Cryptography
