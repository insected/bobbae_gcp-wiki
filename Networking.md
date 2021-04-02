- [Networking](#networking)
  * [Introduction](#introduction)
    + [Networking 101](#networking-101)
    + [Networking End to End](#networking-end-to-end)
    + [Two Tier vs. Three Tier Architecture](#two-tier-vs-three-tier-architecture)
  * [Jupiter](#jupiter)
  * [Network Options](#network-options)
    + [Connectivity Options](#connectivity-options)
    + [Choosing Network Products](#choosing-network-products)
    + [Compare Dedicated Interconnect vs Partner Interconnect](#compare-dedicated-interconnect-vs-partner-interconnect)
    + [Compare Direct Peering to Cloud Interconnect](#compare-direct-peering-to-cloud-interconnect)
    + [Compare Cloud Interconnect with Carrier Peering](#compare-cloud-interconnect-with-carrier-peering)
  * [Virtual Private Cloud (VPC)](#virtual-private-cloud--vpc-)
    + [Introduction](#introduction-1)
    + [Migrate from on-prem to cloud using VPC](#migrate-from-on-prem-to-cloud-using-vpc)
    + [VPC Deep Dive](#vpc-deep-dive)
    + [Shared VPC and VPC Peering](#shared-vpc-and-vpc-peering)
      - [VPC network Sharing and Peering](#vpc-network-sharing-and-peering)
  * [Cloud Router](#cloud-router)
    + [Introduction](#introduction-2)
    + [BGP](#bgp)
    + [Dynamic Routing](#dynamic-routing)
  * [Cloud VPN](#cloud-vpn)
    + [Introduction](#introduction-3)
    + [Types of Cloud VPN](#types-of-cloud-vpn)
      - [Classic VPN](#classic-vpn)
      - [HA VPN](#ha-vpn)
      - [Active/active vs. active/passive routing options for HA VPN](#active-active-vs-active-passive-routing-options-for-ha-vpn)
      - [Comparison between HA VPN and Classic VPN](#comparison-between-ha-vpn-and-classic-vpn)
    + [Cloud VPN Topologies](#cloud-vpn-topologies)
      - [HA VPN to peer VPN Gateways](#ha-vpn-to-peer-vpn-gateways)
      - [HA VPN to AWS peer Gateways](#ha-vpn-to-aws-peer-gateways)
      - [HA VPN between Google Cloud networks](#ha-vpn-between-google-cloud-networks)
  * [Cloud DNS](#cloud-dns)
    + [Introduction](#introduction-4)
    + [DNS & SSL](#dns---ssl)
      - [Cert Manager, Kubernetes, Let’s Encrypt](#cert-manager--kubernetes--let-s-encrypt)
    + [IP Addresses, Netmasks](#ip-addresses--netmasks)
  * [Identity, Security, AuthN, AuthZ](#identity--security--authn--authz)
    + [PKI](#pki)
    + [OAthu, OpenID Connect, SAML](#oathu--openid-connect--saml)
  * [Cloud CDN](#cloud-cdn)
    + [Introduction](#introduction-5)
    + [Using CDN and Load Balancing](#using-cdn-and-load-balancing)
    + [Setting up Cloud CDN with backend storage bucket](#setting-up-cloud-cdn-with-backend-storage-bucket)
  * [Hybrid Connectivity](#hybrid-connectivity)
  * [Cloud Interconnect](#cloud-interconnect)
    + [Introduction](#introduction-6)
    + [Dedicated Interconnect](#dedicated-interconnect)
    + [Partner Interconnect](#partner-interconnect)
  * [Peering](#peering)
    + [Direct Peering](#direct-peering)
    + [Carrier Peering](#carrier-peering)
  * [Cloud Load Balancing](#cloud-load-balancing)
    + [Introduction](#introduction-7)
    + [Types of Load Balancing](#types-of-load-balancing)
      - [Maglev](#maglev)
      - [Andromeda](#andromeda)
    + [Load Balancer Options](#load-balancer-options)
  * [Cloud NAT](#cloud-nat)
  * [Cloud Armor](#cloud-armor)
  * [Network Intelligence Center](#network-intelligence-center)
  * [Network Service Tiers](#network-service-tiers)
  * [Network Telemetry](#network-telemetry)
  * [Traffic Director](#traffic-director)
  * [Service Directory](#service-directory)
  * [Qwiklabs](#qwiklabs)
    + [Networking](#networking-1)
    + [Secure Networks](#secure-networks)
    + [Network Performance](#network-performance)
    + [VPC Networking Fundamentals](#vpc-networking-fundamentals)
    + [VPC Network Peering](#vpc-network-peering)
    + [Performance Optimization](#performance-optimization)
    + [VPC Flow Logs](#vpc-flow-logs)
    + [Multiple VPC Networks](#multiple-vpc-networks)
    + [Controlling Access](#controlling-access)
    + [Using VPC Network Peering](#using-vpc-network-peering)
    + [HA-VPN](#ha-vpn)
    + [Cloud Routers](#cloud-routers)
    + [Service Directory](#service-directory-1)

<small><i><a href='http://ecotrust-canada.github.io/markdown-toc/'>Table of contents generated with markdown-toc</a></i></small>

## Networking


### Introduction

Google Cloud Platform includes software-defined networking, hybrid connectivity, network performance optimization, network security, service mesh deployment, NAT, load balancing, and routing.

[https://developers.google.com/learn/topics/networking](https://developers.google.com/learn/topics/networking)

Google Cloud Platform has recently added new regions in Seoul, Salt Lake City, Las Vegas and Jakarta. GCP implements software-defined network that provides fast and reliable connections to users around the world.

[https://cloud.google.com/about/locations](https://cloud.google.com/about/locations)


Google spent $30 billion improving the infrastructure over the years. From data centers to subsea cables, GCP connects customers in different regions around the world.

[https://www.blog.google/products/google-cloud/expanding-our-global-infrastructure-new-regions-and-subsea-cables/](https://www.blog.google/products/google-cloud/expanding-our-global-infrastructure-new-regions-and-subsea-cables/)

In a traditional data center, you manage a complex network setup composed of racks of servers, storage devices, multiple layers of switches, routers, load balancers, firewall devices, and more. In addition to these hardware components, you must set up, maintain, and monitor the network's underlying software, as well as detailed device configurations for your environment. And the managerial overhead doesn't end there: you also have to worry about the security and availability of your network, and you must plan out the upgrades and expansions of your network—a lengthy and time-consuming process.

https://cloud.google.com/docs/compare/data-centers/networking

#### Networking 101

[https://www.youtube.com/watch?v=0hN-dyOV10c](https://www.youtube.com/watch?v=0hN-dyOV10c)


#### Networking End to End

[https://www.youtube.com/playlist?list=PLIivdWyY5sqJ0oXcnZYqOnuNRsLF9H48u](https://www.youtube.com/playlist?list=PLIivdWyY5sqJ0oXcnZYqOnuNRsLF9H48u)


#### Two Tier vs. Three Tier Architecture

[https://www.wwt.com/article/comparing-two-tier-three-tier-data-center-networks](https://www.wwt.com/article/comparing-two-tier-three-tier-data-center-networks)


### Jupiter

Jupiter fabrics can deliver more than 1 Petabit/sec of total bisection bandwidth. To put this in perspective, such capacity would be enough for 100,000 servers to exchange information at 10Gb/s each, enough to read the entire scanned contents of the Library of Congress in less than 1/10th of a second.

[https://cloudplatform.googleblog.com/2015/06/A-Look-Inside-Googles-Data-Center-Networks.html](https://cloudplatform.googleblog.com/2015/06/A-Look-Inside-Googles-Data-Center-Networks.html?m=1)


### Network Options


#### Connectivity Options

[https://cloud.google.com/blog/products/networking/google-cloud-network-connectivity-options-explained](https://cloud.google.com/blog/products/networking/google-cloud-network-connectivity-options-explained)

For pricing, quotas, service level agreement (SLA), and release note information for all Network Connectivity products, see the [Network Connectivity resources page](https://cloud.google.com/network-connectivity/docs/resources).

For high-level architectural guides and tutorials that describe networking scenarios for Google Cloud, see the [Technical guides for networking](https://cloud.google.com/docs/tutorials#networking).


#### Choosing Network Products

[https://cloud.google.com/network-connectivity/docs/how-to/choose-product](https://cloud.google.com/network-connectivity/docs/how-to/choose-product)


#### Compare Dedicated Interconnect vs Partner Interconnect

[https://cloud.google.com/network-connectivity/docs/how-to/choose-product#compare-interconnect-solutions](https://cloud.google.com/network-connectivity/docs/how-to/choose-product#compare-interconnect-solutions)


#### Compare Direct Peering to Cloud Interconnect

[https://cloud.google.com/network-connectivity/docs/how-to/choose-product#dp-compare](https://cloud.google.com/network-connectivity/docs/how-to/choose-product#dp-compare)


#### Compare Cloud Interconnect with Carrier Peering

[https://cloud.google.com/network-connectivity/docs/how-to/choose-product#cp-compare](https://cloud.google.com/network-connectivity/docs/how-to/choose-product#cp-compare)


### Virtual Private Cloud (VPC)


#### Introduction

Google Cloud Virtual Private Cloud (VPC) provides networking functionality to Compute Engine virtual machine (VM) instances, Google Kubernetes Engine (GKE) containers, and the App Engine flexible environment. VPC provides networking for your cloud-based services that is global, scalable, and flexible.

[https://cloud.google.com/vpc/docs](https://cloud.google.com/vpc/docs)


#### Migrate from on-prem to cloud using VPC

[https://www.youtube.com/watch?v=cNb7xKyya5c](https://www.youtube.com/watch?v=cNb7xKyya5c)


#### VPC Deep Dive

[https://www.youtube.com/watch?v=wmP6SQe5J7g](https://www.youtube.com/watch?v=wmP6SQe5J7g)

Google Cloud Virtual Private Cloud (VPC) Network Peering allows private connectivity across two VPC networks regardless of whether or not they belong to the same project or the same organization.

VPC networks use Linux's [VIRTIO network module](http://dl.acm.org/citation.cfm?id=1400097.1400108) to model Ethernet card and router functionality, but higher levels of the networking stack, such as ARP lookups, are handled using standard networking software.

[https://cloud.google.com/vpc/docs/advanced-vpc](https://cloud.google.com/vpc/docs/advanced-vpc)


#### Shared VPC and VPC Peering

[Shared VPC](https://cloud.google.com/vpc/docs/shared-vpc) allows an  [organization](https://cloud.google.com/resource-manager/docs/cloud-platform-resource-hierarchy) to connect resources from multiple projects to a common [Virtual Private Cloud (VPC) network](https://cloud.google.com/vpc/docs/vpc), so that they can communicate with each other securely and efficiently using internal IPs from that network. When you use Shared VPC, you designate a project as a host project and attach one or more other service projects to it. The VPC networks in the host project are called Shared VPC networks. [Eligible resources](https://cloud.google.com/vpc/docs/shared-vpc#resources_that_can_be_attached_to_shared_vpc_networks_from_a_service_project) from service projects can use subnets in the Shared VPC network.

Shared VPC lets [organization administrators](https://cloud.google.com/resource-manager/docs/cloud-platform-resource-hierarchy#organizations) delegate administrative responsibilities, such as creating and managing instances, to [Service Project Admins](https://cloud.google.com/vpc/docs/shared-vpc#iam_in_shared_vpc) while maintaining centralized control over network resources like subnets, routes, and firewalls.

Google Cloud VPC Network Peering allows [internal IP address](https://cloud.google.com/vpc/docs/ip-addresses) connectivity across two Virtual Private Cloud (VPC) networks regardless of whether they belong to the same project or the same organization.

[VPC Network Peering](https://cloud.google.com/vpc/docs/vpc-peering) enables you to connect VPC networks so that workloads in different VPC networks can communicate internally. Traffic stays within Google's network and doesn't traverse the public internet.

[https://cloud.google.com/vpc/docs/vpc-peering](https://cloud.google.com/vpc/docs/vpc-peering)


##### VPC network Sharing and Peering

Shared VPC allows you to export subnets from a [VPC network](https://cloud.google.com/vpc/docs/vpc) in a host project to other service projects in the same [organization](https://cloud.google.com/resource-manager/docs/creating-managing-organization). Instances in the service projects can have network connections in the shared subnets of the host project. 

[https://cloud.google.com/vpc/docs/how-to#vpc-network-sharing-and-peering](https://cloud.google.com/vpc/docs/how-to#vpc-network-sharing-and-peering)


### Cloud Router


#### Introduction

Cloud Router enables you to dynamically exchange routes between your Virtual Private Cloud (VPC) and on-premises networks by using [Border Gateway Protocol (BGP)](https://www.wikipedia.org/wiki/Border_Gateway_Protocol). For example, if you use a Cloud VPN tunnel to connect your networks, you can use Cloud Router to establish a BGP session with your on-premises router over your Cloud VPN tunnel. Cloud Router automatically learns new subnets in your VPC network and announces them to your on-premises network.

[https://cloud.google.com/network-connectivity/docs/router](https://cloud.google.com/network-connectivity/docs/router)


#### BGP

[Cloud Router uses Border Gateway Protocol ](https://cloud.google.com/network-connectivity/docs/router/how-to/configuring-bgp)(BGP) to exchange routes between your Virtual Private Cloud (VPC) network and your on-premises network. On Cloud Router, you configure an interface and a BGP peer for your on-premises router. The interface and BGP peer configuration together form a BGP session.

[https://www.youtube.com/watch?v=_Z29ZzKeZHc](https://www.youtube.com/watch?v=_Z29ZzKeZHc)


#### Dynamic Routing

Dynamic routing with Cloud Router.

[https://www.youtube.com/watch?v=K_xb_j46YOk](https://www.youtube.com/watch?v=K_xb_j46YOk)

[https://medium.com/google-cloud/dynamic-routing-with-cloud-router-9ff5c362d833](https://medium.com/google-cloud/dynamic-routing-with-cloud-router-9ff5c362d833)


### Cloud VPN


#### Introduction

Cloud VPN securely extends your [peer](https://cloud.google.com/network-connectivity/docs/vpn/concepts/key-terms#peer-definition) network to Google's network through an IPsec VPN tunnel. Traffic is encrypted and travels between the two networks over the public internet. Cloud VPN is useful for low-volume data connections.

[https://cloud.google.com/network-connectivity/docs/vpn](https://cloud.google.com/network-connectivity/docs/vpn)


#### Types of Cloud VPN


##### Classic VPN

[ Classic VPN ](https://cloud.google.com/network-connectivity/docs/vpn/concepts/overview#classic-vpn)gateways have a single interface, a single external IP address, and support tunnels that use dynamic (BGP) or static routing (policy-based or route-based). They provide an SLA of 99.9% service availability.


##### HA VPN

[HA VPN](https://cloud.google.com/network-connectivity/docs/vpn/concepts/overview#ha-vpn) lets you easily set up redundant VPNs to isolate failures and provide continuous connectivity for workloads that are too important to fail. 

Use Case 1: Migrate an existing Classic VPN solution to HA VPN utilizing BGP as the routing protocol to an on-premises network (or any non Google Networks). Use Case 2: Migrate an existing Classic VPN utilizing policy based VPN to HA VPN utilizing BGP between two projects or VPCs within Google Cloud Platform.

[https://www.youtube.com/watch?v=lIEExVWf5bg](https://www.youtube.com/watch?v=lIEExVWf5bg)

If a Cloud VPN tunnel goes down, it restarts automatically. If an entire virtual VPN device fails, Cloud VPN automatically instantiates a new one with the same configuration. The new gateway and tunnel connect automatically.

VPN tunnels connected to HA VPN gateways must use dynamic (BGP) routing. Depending on the way that you configure route priorities for HA VPN tunnels, you can create an active/active or active/passive routing configuration. For both of these routing configurations, both VPN tunnels remain active.


##### Active/active vs. active/passive routing options for HA VPN

[https://cloud.google.com/network-connectivity/docs/vpn/concepts/overview#active](https://cloud.google.com/network-connectivity/docs/vpn/concepts/overview#active)


##### Comparison between HA VPN and Classic VPN

[https://cloud.google.com/network-connectivity/docs/vpn/concepts/overview#comparison_table](https://cloud.google.com/network-connectivity/docs/vpn/concepts/overview#comparison_table)


#### Cloud VPN Topologies

With Cloud VPN, your on-premises hosts communicate through one or more IPsec VPN tunnels to Compute Engine Virtual Machine (VM) instances in your project's VPC networks.

[https://cloud.google.com/network-connectivity/docs/vpn/concepts/topologies](https://cloud.google.com/network-connectivity/docs/vpn/concepts/topologies)


##### HA VPN to peer VPN Gateways

[https://cloud.google.com/network-connectivity/docs/vpn/concepts/topologies#to_peer_vpn_gateways](https://cloud.google.com/network-connectivity/docs/vpn/concepts/topologies#to_peer_vpn_gateways)


##### HA VPN to AWS peer Gateways

[https://cloud.google.com/network-connectivity/docs/vpn/concepts/topologies#to_aws_peer_gateways](https://cloud.google.com/network-connectivity/docs/vpn/concepts/topologies#to_aws_peer_gateways)


##### HA VPN between Google Cloud networks

[https://cloud.google.com/network-connectivity/docs/vpn/concepts/topologies#2-gcp-gateways](https://cloud.google.com/network-connectivity/docs/vpn/concepts/topologies#2-gcp-gateways)

#### Advanced configurations
You can create a VPN tunnel that has the same IP range as another tunnel, a subset of the other tunnel's range, or a superset of the other tunnel's range.

For details, see [Order of routes](https://cloud.google.com/network-connectivity/docs/vpn/concepts/order-of-routes).

In [Supported IKE ciphers](https://cloud.google.com/network-connectivity/docs/vpn/concepts/supported-ike-ciphers), you can find details about how Cloud VPN supports multiple [IKE](https://en.wikipedia.org/wiki/Internet_Key_Exchange) ciphers.  IKE is the protocol used to setup a security association (SA) in the [IPSec](https://en.wikipedia.org/wiki/IPsec).  IKE uses [X.509](https://en.wikipedia.org/wiki/X.509) for certificates.  X.509 is a standard defining the format of public key certificates which are used in TLS/SSL basis for HTTPS.  Base standard for X.509 is [ASN.1](https://en.wikipedia.org/wiki/ASN.1), a kind of IDL for defining data structures that can be serialized and de-serialized.  IKE X.509 certificates
are pre-shared or distributed using DNS or DNSSEC and a [Diffie-Hellman](https://en.wikipedia.org/wiki/Diffie%E2%80%93Hellman_key_exchange) key exchange is used to set up a shared session secret from which cryptographic keys are derived.


In [Networks and tunnel routing](https://cloud.google.com/network-connectivity/docs/vpn/concepts/choosing-networks-routing), you can find information about supported Virtual Private Cloud (VPC) networks and routing options, including traffic selectors.

### Cloud DNS


#### Introduction

Publish your domain names by using Google's infrastructure for production-quality, high-volume DNS services. Google's global network of anycast name servers provides reliable, low-latency, authoritative name lookups for your domains from anywhere in the world.

[https://cloud.google.com/dns/docs](https://cloud.google.com/dns/docs)


#### DNS & SSL

[https://www.youtube.com/watch?v=sTDVsMUegL8](https://www.youtube.com/watch?v=sTDVsMUegL8)


##### Cert Manager, Kubernetes, Let’s Encrypt

[https://www.youtube.com/watch?v=LH4nLtUpuBI](https://www.youtube.com/watch?v=LH4nLtUpuBI)


#### IP Addresses, Netmasks

[https://www.youtube.com/watch?v=EkNq4TrHP_U](https://www.youtube.com/watch?v=EkNq4TrHP_U)


### Identity, Security, AuthN, AuthZ

Access control for Google Cloud APIs encompasses authentication, authorization, and auditing. Authentication determines who you are, authorization determines what you can do, and auditing logs what you did.  For authorization, see [Identity and Access Management](https://cloud.google.com/iam/docs) (IAM). For auditing, see [Cloud Audit Logs](https://cloud.google.com/logging/docs/audit).

https://cloud.google.com/docs/authentication


#### PKI

A public key infrastructure (PKI) is a set of roles, policies, hardware, software and procedures needed to create, manage, distribute, use, store and revoke [digital certificates](https://en.wikipedia.org/wiki/Public_key_certificate) and manage [public-key encryption](https://en.wikipedia.org/wiki/Public-key_cryptography). The purpose of a PKI is to facilitate the secure electronic transfer of information for a range of network activities such as e-commerce, internet banking and confidential email. It is required for activities where simple passwords are an inadequate authentication method and more rigorous proof is required to confirm the identity of the parties involved in the communication and to validate the information being transferred.

[https://www.ssh.com/pki/](https://www.ssh.com/pki/)


#### OAthu, OpenID Connect, SAML

[https://www.okta.com/identity-101/whats-the-difference-between-oauth-openid-connect-and-saml/](https://www.okta.com/identity-101/whats-the-difference-between-oauth-openid-connect-and-saml/)


### Cloud CDN


#### Introduction

Cloud CDN (Content Delivery Network) uses Google's globally distributed edge points of presence to cache external HTTP(S) load balanced content close to your users. Caching content at the edges of Google's network provides faster delivery of content to your users while reducing serving costs.

[https://cloud.google.com/cdn/docs](https://cloud.google.com/cdn/docs)


#### Using CDN and Load Balancing

[https://www.youtube.com/watch?v=NedNhOg_TgA](https://www.youtube.com/watch?v=NedNhOg_TgA)


#### Setting up Cloud CDN with backend storage bucket

[https://cloud.google.com/cdn/docs/setting-up-cdn-with-bucket](https://cloud.google.com/cdn/docs/setting-up-cdn-with-bucket)


### Hybrid Connectivity

[https://cloud.google.com/hybrid-connectivity](https://cloud.google.com/hybrid-connectivity)


### Cloud Interconnect


#### Introduction

Cloud Interconnect extends your on-premises network to Google's network through a highly available, low latency connection. You can use Dedicated Interconnect to connect directly to Google or use Partner Interconnect to connect to Google through a supported service provider.

[https://cloud.google.com/network-connectivity/docs/interconnect](https://cloud.google.com/network-connectivity/docs/interconnect)

While migrating portions of your on-prem to the cloud, it’s important for your on-prem systems to communicate with your newly minted cloud resource.

[https://www.youtube.com/watch?v=cKaryf7qp9w](https://www.youtube.com/watch?v=cKaryf7qp9w)


#### Dedicated Interconnect

Dedicated Interconnect provides direct physical connections between your on-premises network and Google's network. Dedicated Interconnect enables you to transfer large amounts of data between networks, which can be more cost effective than purchasing additional bandwidth over the public Internet.

[https://cloud.google.com/network-connectivity/docs/interconnect](https://cloud.google.com/network-connectivity/docs/interconnect)

 After you create a VLAN attachment, you need to configure your on-premises router to establish a BGP session with your Cloud Router. Use the VLAN ID, interface IP address, and peering IP address provided by the [VLAN attachment](https://cloud.google.com/network-connectivity/docs/interconnect/how-to/dedicated/creating-vlan-attachments) to configure your on-premises router.

[https://cloud.google.com/network-connectivity/docs/interconnect/how-to/dedicated/configuring-onprem-routers](https://cloud.google.com/network-connectivity/docs/interconnect/how-to/dedicated/configuring-onprem-routers)


#### Partner Interconnect

Partner Interconnect provides connectivity between your on-premises network and your VPC network through a supported [service provider](https://cloud.google.com/network-connectivity/docs/interconnect/concepts/service-providers). A Partner Interconnect connection is useful if your data center is in a physical location that can't reach a Dedicated Interconnect colocation facility or if your data needs don't warrant an entire 10 Gbps connection.

[https://cloud.google.com/network-connectivity/docs/interconnect](https://cloud.google.com/network-connectivity/docs/interconnect)

An on-premises router in this context means a Layer 2 (L2) or Layer 3 (L3) device you configure to enable Partner Interconnect.

[https://cloud.google.com/network-connectivity/docs/interconnect/how-to/partner/configuring-onprem-routers](https://cloud.google.com/network-connectivity/docs/interconnect/how-to/partner/configuring-onprem-routers)


### Peering

[https://www.peeringdb.com/net/433](https://www.peeringdb.com/net/433)


#### Direct Peering

[https://cloud.google.com/network-connectivity/docs/direct-peering](https://cloud.google.com/network-connectivity/docs/direct-peering)

Direct Peering enables you to establish a direct [peering](https://www.wikipedia.org/wiki/Peering) connection between your business network and Google's edge network and exchange high-throughput cloud traffic.

Direct Peering exists outside of Google Cloud. Unless you need to access Google Workspace applications, the recommended methods of access to Google Cloud are [Dedicated Interconnect](https://cloud.google.com/network-connectivity/docs/interconnect/concepts/dedicated-overview) or [Partner Interconnect](https://cloud.google.com/network-connectivity/docs/interconnect/concepts/partner-overview).


#### Carrier Peering

Carrier Peering enables you to access Google applications, such as Google Workspace, by using a [service provider](https://cloud.google.com/network-connectivity/docs/carrier-peering#service-providers) to obtain enterprise-grade network services that connect your infrastructure to Google.

[https://cloud.google.com/network-connectivity/docs/carrier-peering](https://cloud.google.com/network-connectivity/docs/carrier-peering)


### Cloud Load Balancing


#### Introduction

Cloud Load Balancing allows you to put your resources behind a single IP address that is externally accessible or internal to your Virtual Private Cloud (VPC) network.

[https://cloud.google.com/load-balancing/docs](https://cloud.google.com/load-balancing/docs)

A Video about Cloud Load Balancing.

[https://www.youtube.com/watch?v=D4XZkCJyqis](https://www.youtube.com/watch?v=D4XZkCJyqis)

Google Cloud Load Balancing enables enterprises and cloud-natives to deliver highly available, scalable, low-latency cloud services with a global footprint. Use Google Global Load Balancing to deliver global reach and scale. Deploy your application backends in single or multiple regions wherever your users are, front-ending these with a single anycast VIP, and growing or shrinking your backend resources with intelligent Autoscaling. Scale private services using Internal Load Balancing (ILB) for clients in Google Cloud or on-prem across Interconnect/VPN. 

[https://www.youtube.com/watch?v=J5HJ1y6PeyE](https://www.youtube.com/watch?v=J5HJ1y6PeyE)


#### Types of Load Balancing

[https://cloud.google.com/load-balancing/docs/load-balancing-overview](https://cloud.google.com/load-balancing/docs/load-balancing-overview)

[https://cloud.google.com/blog/products/networking/google-cloud-networking-in-depth-cloud-load-balancing-deconstructed](https://cloud.google.com/blog/products/networking/google-cloud-networking-in-depth-cloud-load-balancing-deconstructed)


##### Maglev

[https://research.google/pubs/pub44824/](https://research.google/pubs/pub44824/)


##### Andromeda

[https://www.usenix.org/system/files/conference/nsdi18/nsdi18-dalton.pdf](https://www.usenix.org/system/files/conference/nsdi18/nsdi18-dalton.pdf)


#### Load Balancer Options

To decide which load balancer best suits your implementation of Google Cloud, consider the following aspects of Cloud Load Balancing:



*   Global versus regional load balancing
*   External versus internal load balancing
*   Traffic type

[https://cloud.google.com/load-balancing/docs/choosing-load-balancer](https://cloud.google.com/load-balancing/docs/choosing-load-balancer)


### Cloud NAT

Cloud NAT provides fully managed, software-defined network address translation support for Google Cloud.

[https://cloud.google.com/nat/docs](https://cloud.google.com/nat/docs)

Moving your internal services to the cloud can bring you a handful of new, useful features, but one of the biggest challenges is protecting your internal endpoints. 

[https://www.youtube.com/watch?v=bmaarG0IkH8](https://www.youtube.com/watch?v=bmaarG0IkH8)


### Cloud Armor

Google Cloud Armor helps protect your infrastructure and applications from distributed denial-of-service (DDoS) attacks by using Google's global infrastructure and security systems.

[https://cloud.google.com/armor/docs](https://cloud.google.com/armor/docs)

Setting up Cloud Armor.

[https://www.youtube.com/watch?v=g_c2KLpnWck](https://www.youtube.com/watch?v=g_c2KLpnWck)


### Network Intelligence Center

Network Intelligence Center provides a single console for managing Google Cloud network visibility, monitoring, and troubleshooting.

[https://cloud.google.com/network-intelligence-center/docs](https://cloud.google.com/network-intelligence-center/docs)

Getting started with topology in network intelligence center.

[https://www.youtube.com/watch?v=ID7szIL9eew](https://www.youtube.com/watch?v=ID7szIL9eew)


### Network Service Tiers

With Network Service Tiers, Google Cloud is the first major public cloud to offer a tiered cloud network. Select the right tier of network service for your requirements and budget.

[https://cloud.google.com/network-tiers](https://cloud.google.com/network-tiers)

Cost savings using different network tiers.

[https://www.youtube.com/watch?v=wsdgWGE-mwE](https://www.youtube.com/watch?v=wsdgWGE-mwE)


### Network Telemetry

VPC Flow Logs records a sample of network flows sent from and received by VM instances, including instances used as GKE nodes. These logs can be used for network monitoring, forensics, real-time security analysis, and expense optimization.

[https://cloud.google.com/vpc/docs/using-flow-logs](https://cloud.google.com/vpc/docs/using-flow-logs)

Network and security telemetry is fundamental to operate your deployments in public clouds with confidence, providing the required visibility on the behavior of your network and Access control firewalls. 

[https://www.youtube.com/watch?v=as9mXNEcaDo](https://www.youtube.com/watch?v=as9mXNEcaDo)


### Traffic Director

Traffic Director is Google Cloud's fully managed traffic control plane for service mesh. With Traffic Director, you can deploy global load balancing across clusters and virtual machine (VM) instances in multiple regions, offload health checking from service proxies, and configure sophisticated traffic control policies.

[https://cloud.google.com/traffic-director/docs](https://cloud.google.com/traffic-director/docs)

Traffic Director is toil-free, GCP-managed control plane with SLA for Service Meshes.

 In Istio environments, Traffic Director provides a GCP-managed Pilot for your service mesh. 

Traffic Director delivers traffic management and multi-region global load balancing for service meshes built using open proxies like Envoy and through the open xDSv2 APIs. It provides policy driven traffic routing, enabling you to control the flow of traffic between services. All of this makes load balancing, scaling, A/B testing, canary roll outs, and blue-green deployments easy  to set up. Traffic Director also provides centralized high fidelity health checking, and traffic driven autoscaling. Envoy-based Layer 7 Internal Load Balancing (L7 ILB), another flavor of Traffic Director, brings modern traffic management capabilities to traditional environments. With L7 ILB, Traffic Director controls a pool of GCP-managed Envoy proxies under the hood but presents this service as a traditional Layer 7 ILB middle proxy to front your legacy apps. 

Traffic Director supports VM-based, Kubernetes and GKE apps.

[https://www.youtube.com/watch?v=FUITCYMCEhU](https://www.youtube.com/watch?v=FUITCYMCEhU)


### Service Directory

Service Directory helps reduce the complexity of management and operations by providing a single place to publish, discover, and connect services. It is a managed service that enhances service inventory management at scale so you don’t have to. Service Directory provides real-time service information, whether you have a few service endpoints or thousands. 

[https://cloud.google.com/service-directory](https://cloud.google.com/service-directory)

[https://www.youtube.com/watch?v=H9UoE_cWIEY](https://www.youtube.com/watch?v=H9UoE_cWIEY)


### Qwiklabs


#### Networking

Networking is a principle theme of cloud computing. It’s the underlying structure of Google Cloud, and it’s what connects all your resources and services to one another. This fundamental-level quest will cover essential Google Cloud networking services and will give you hands-on practice with specialized tools for developing mature networks. From learning the ins-and-outs of VPCs, to creating enterprise-grade load balancers, Networking in the Google Cloud will give you the practical experience needed so you can start building robust networks right away.

[Networking in the Google Cloud](https://www.qwiklabs.com/quests/31?catalog_rank=%7B%22rank%22%3A4%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&search_id=7467791)


#### Secure Networks

[Build and Secure Networks in Google Cloud](https://www.qwiklabs.com/quests/128?catalog_rank=%7B%22rank%22%3A1%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&search_id=7467791)


#### Network Performance

This quest is composed of labs that cover real-life use cases and it will teach you best practices for overcoming common networking bottlenecks. From getting hands-on practice with testing and improving network performance, to integrating high-throughput VPNs and networking tiers, Network Performance and Optimization is an essential quest for GCP developers who are looking to double down on application speed and robustness. \


[Network Performance and Optimization](https://www.qwiklabs.com/quests/46?catalog_rank=%7B%22rank%22%3A2%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&search_id=7467791)


#### VPC Networking Fundamentals

Google Cloud Virtual Private Cloud (VPC) provides networking functionality to Compute Engine virtual machine (VM) instances, Kubernetes Engine containers and App Engine Flex. In other words, without a VPC network you cannot create VM instances, containers or App Engine applications. Therefore, each Google Cloud project has a default network to get you started.

You can think of a VPC network the same way you would think of a physical network, except that it is virtualized within Google Cloud. A VPC network is a global resource which consists of a list of regional virtual subnetworks (subnets) in data centers, all connected by a global wide area network (WAN). VPC networks are logically isolated from each other in Google Cloud.

[VPC Networking Fundamentals](https://www.qwiklabs.com/focuses/1229?catalog_rank=%7B%22rank%22%3A11%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&parent=catalog&search_id=7467802)


#### VPC Network Peering

VPC Network Peering allows you to build SaaS (Software-as-a-Service) ecosystems in Google Cloud, making services available privately across different VPC networks within and across organizations, allowing workloads to communicate in private space.

[VPC Network Peering](https://www.qwiklabs.com/focuses/964?catalog_rank=%7B%22rank%22%3A10%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&parent=catalog&search_id=7467800)


#### Performance Optimization

This quest is composed of labs that cover real-life use cases and it will teach you best practices for overcoming common networking bottlenecks. From getting hands-on practice with testing and improving network performance, to integrating high-throughput VPNs and networking tiers, Network Performance and Optimization is an essential quest for GCP developers who are looking to double down on application speed and robustness.

[Network Performance and Optimization](https://www.qwiklabs.com/quests/46?catalog_rank=%7B%22rank%22%3A3%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&search_id=7468028)


#### VPC Flow Logs

In this lab, you will learn how to configure a network to record traffic to and from an Apache web server using VPC Flow Logs. You will then export the logs to BigQuery for analysis. There are multiple use cases for VPC Flow Logs. For example, you might use VPC Flow Logs to determine where your applications are being accessed from to optimize network traffic expense, to create HTTP Load Balancers to balance traffic globally, or to denylist unwanted IP addresses with Cloud Armor.

[VPC Flow Logs - Analyzing Network Traffic](https://www.qwiklabs.com/focuses/1236?catalog_rank=%7B%22rank%22%3A12%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&parent=catalog&search_id=7467802)


#### Multiple VPC Networks

In this lab you create several VPC networks and VM instances and test connectivity across networks. Specifically, you create two custom mode networks (managementnet and privatenet) with firewall rules and VM instances. The mynetwork network with its firewall rules and two VM instances (mynet-eu-vm and mynet-us-vm) have already been created for you in this Qwiklabs project.

[Multiple VPC Networks](https://www.qwiklabs.com/focuses/1230?catalog_rank=%7B%22rank%22%3A13%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&parent=catalog&search_id=7467802)


#### Controlling Access

In this lab, you create two nginx web servers and control external HTTP access to the web servers using tagged firewall rules. Then, you explore IAM roles and service accounts.

[VPC Networks - Controlling Access](https://www.qwiklabs.com/focuses/1231?catalog_rank=%7B%22rank%22%3A15%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&parent=catalog&search_id=7467802)


#### Using VPC Network Peering

In this lab, you configure VPC Network Peering between two networks. Then, you verify private communication between two VMs in those networks. VPC Network Peering allows you to build SaaS (Software-as-a-Service) ecosystems on Google Cloud, making services available privately across different VPC networks within and across organizations, allowing workloads to communicate in private RFC 1918 space.

[Using VPC Network Peering](https://www.qwiklabs.com/focuses/1249?catalog_rank=%7B%22rank%22%3A16%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&parent=catalog&search_id=7467802)


#### HA-VPN

HA-VPN is IPSec VPN solution to enable secure connectivity between your on-premise network to your Google Cloud Platform (GCP) Virtual Private Cloud (VPC) network through an IPSec VPN connection with 99.99% service availability at GA. HA-VPN is a regional per VPC VPN solution. HA-VPN gateways have two interfaces, each with their own public IP address. When you create a HA-VPN gateway, two public IP addresses are automatically chosen from different address pools. When HA-VPN is configured with two tunnels, Cloud VPN offers a 99.99% service availability uptime.

[VPC Networking: Cloud HA-VPN](https://www.qwiklabs.com/focuses/6270?catalog_rank=%7B%22rank%22%3A18%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&parent=catalog&search_id=7467802)


#### Cloud Routers

In this lab, you configure Cloud Routers using the Console. The Cloud Routers will implement VPN gateways configured with BGP. BGP provides dynamic network discovery and eliminates the need to configure or maintain static routes. When successful you will be able to ping the internal IP of the VM in a newly discovered subnetwork via an auto-populated route.

[Dynamic VPN Gateways - Cloud Routers ](https://www.qwiklabs.com/focuses/1233?parent=catalog)


#### Service Directory

Service Directory provides real-time service information, whether you have a few service endpoints or thousands. This helps ensure that your applications only resolve the most updated information of their resources, increasing the reachability of your services. With Service Directory, you can easily understand all your services across multi-cloud environments. This includes workloads running in Compute Engine VMs, Google Kubernetes Engine (GKE), as well as external services running on-prem and third-party clouds. It improves application reachability by maintaining the endpoint information for all your services.

[Service Directory: Qwik Start](https://www.qwiklabs.com/focuses/12412?catalog_rank=%7B%22rank%22%3A19%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&parent=catalog&search_id=7468061)

