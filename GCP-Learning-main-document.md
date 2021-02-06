# GCP Learning main document
## A GCP Training


## Table of Contents

- [Preparation](https://github.com/bobbae/gcp/wiki/Preparation)
- [Introduction to GCP](https://github.com/bobbae/gcp/wiki/GCP-Introduction)
- [GCP Compute Engine](https://github.com/bobbae/gcp/wiki/GCP-Compute-Engine)
- [App Engine](https://github.com/bobbae/gcp/wiki/App-Engine)
- [Compute Options](https://github.com/bobbae/gcp/wiki/Compute-Options)
- [Kubernetes Engine and Containers](https://github.com/bobbae/gcp/wiki/Kubernetes-Engine-and-Containers)
- [Storage](https://github.com/bobbae/gcp/wiki/GCP-Storage)
- [Data Engineering](https://github.com/bobbae/gcp/wiki/Data-Engineering)
- [Data Science](https://github.com/bobbae/gcp/wiki/Data-Science)

## Database Related topics


### SQL, NoSQL, NewSQL

[https://www.youtube.com/watch?v=ZS_kXvOeQ5Y](https://www.youtube.com/watch?v=ZS_kXvOeQ5Y)

[https://www.virtual-dba.com/differences-between-sql-nosql-and-newsql/](https://www.virtual-dba.com/differences-between-sql-nosql-and-newsql/)


### ACID, BASE, CAP

[https://medium.com/@pranabj.aec/acid-cap-and-base-cc73dee43f8c](https://medium.com/@pranabj.aec/acid-cap-and-base-cc73dee43f8c)


### Serializability, linearizability, and locality

[https://aphyr.com/posts/333-serializability-linearizability-and-locality](https://aphyr.com/posts/333-serializability-linearizability-and-locality)


### Distributed Consensus Protocols

[https://www.alibabacloud.com/blog/a-brief-analysis-of-consensus-protocol-from-logical-clock-to-raft_594675](https://www.alibabacloud.com/blog/a-brief-analysis-of-consensus-protocol-from-logical-clock-to-raft_594675)


### Database of Databases

[https://dbdb.io/browse](https://dbdb.io/browse)


## Migration


### Introduction

A video on Cloud Migration.

[https://www.youtube.com/watch?v=Bt_cWJrdfS8](https://www.youtube.com/watch?v=Bt_cWJrdfS8)

[https://cloud.google.com/solutions/migration-to-gcp-getting-started](https://cloud.google.com/solutions/migration-to-gcp-getting-started)


### BigQuery Data Transfer Service

The BigQuery Data Transfer Service automates data movement into BigQuery on a scheduled, managed basis. Your analytics team can lay the foundation for a BigQuery data warehouse without writing a single line of code.

[https://cloud.google.com/bigquery-transfer/docs/transfer-service-overview](https://cloud.google.com/bigquery-transfer/docs/transfer-service-overview)


### Migrate for Compute Engine

Google Cloud Migrate for Compute Engine (formerly Velostrata) migrates VMs from your on-premises data center, AWS, or Azure into Compute Engine.

[https://cloud.google.com/migrate/compute-engine/docs](https://cloud.google.com/migrate/compute-engine/docs)


#### Velostrata

Google Cloud Migrate for Compute Engine (formerly Velostrata) migrates VMs from your on-premises data center, AWS, or Azure into Compute Engine.

[https://cloud.google.com/blog/products/velostrata](https://cloud.google.com/blog/products/velostrata)


#### How to move thousands of VMs to GCP

[https://www.youtube.com/watch?v=WD454APAPV8](https://www.youtube.com/watch?v=WD454APAPV8)


### Cloud Storage Transfer Service

Storage Transfer Service allows you to quickly import online data into Cloud Storage. You can also set up a repeating schedule for transferring data, as well as transfer data within Cloud Storage, from one bucket to another.

[https://cloud.google.com/storage-transfer/docs](https://cloud.google.com/storage-transfer/docs)


### Migrate for Anthos

With Migrate for Anthos, you can migrate your VMs from [supported source platforms](https://cloud.google.com/migrate/anthos/docs/migration-prerequisites) to Google Kubernetes Engine or [Anthos](https://cloud.google.com/anthos).

[https://cloud.google.com/migrate/anthos/docs/getting-started](https://cloud.google.com/migrate/anthos/docs/getting-started)


#### Migrating enterprise workloads using Migrate for Anthos

[https://www.youtube.com/watch?v=8Q1kqWVbKQY](https://www.youtube.com/watch?v=8Q1kqWVbKQY)


### Transfer Appliance

Transfer Appliance is a hardware appliance you can use to securely migrate large volumes of data (from hundreds of terabytes up to 1 petabyte) to Google Cloud Platform without disrupting business operations.

[https://cloud.google.com/transfer-appliance/docs/2.0](https://cloud.google.com/transfer-appliance/docs/2.0)


### Cloud Data Transfer

There are many different ways to transfer data in GCP: Online Transfer, Transfer Service, Transfer Appliance, BigQuery Data Transfer Service and Offline Transfer Methods.

[https://cloud.google.com/products/data-transfer](https://cloud.google.com/products/data-transfer)


### Storage Transfer Service

Whether you're coming from an online or on-premises source, our online storage transfer solutions enable you to manage large-scale data transfers easily, securely, and efficiently. Storage Transfer Service and Transfer Service for on-premises data offer two highly performant pathways to Cloud Storage—both with the scalability and speed you need to simplify the data transfer process.

[https://cloud.google.com/storage-transfer-service](https://cloud.google.com/storage-transfer-service)


### Database Migration Service

[https://cloud.google.com/database-migration](https://cloud.google.com/database-migration)

[https://cloud.google.com/blog/products/databases/database-migration-service-now-available-for-cloud-sql-and-more](https://cloud.google.com/blog/products/databases/database-migration-service-now-available-for-cloud-sql-and-more)


### All Google Cloud Migration Guides

[https://cloud.google.com/blog/products/cloud-migration/guide-to-all-google-cloud-migration-guides](https://cloud.google.com/blog/products/cloud-migration/guide-to-all-google-cloud-migration-guides)


### Big Data Transfer over WAN

[https://asperasoft.com/fileadmin/media/Asperasoft.com/Product_Briefs/Google_AoD_AsperaPB.pdf](https://asperasoft.com/fileadmin/media/Asperasoft.com/Product_Briefs/Google_AoD_AsperaPB.pdf)


### Netapp

[https://cloud.google.com/netapp](https://cloud.google.com/netapp)


#### Trident

[https://github.com/NetApp/trident](https://github.com/NetApp/trident)


#### Cloud Volumes Service 

[https://cloud.netapp.com/cloud-volumes-service-for-gcp](https://cloud.netapp.com/cloud-volumes-service-for-gcp)


### AWS to GCP Data migration

[https://cloud.google.com/migrate/compute-engine/docs/4.2/how-to/migrate-aws-to-gcp/overview](https://cloud.google.com/migrate/compute-engine/docs/4.2/how-to/migrate-aws-to-gcp/overview)


## Networking


### Introduction

Google Cloud Platform includes software-defined networking, hybrid connectivity, network performance optimization, network security, service mesh deployment, NAT, load balancing, and routing.

[https://developers.google.com/learn/topics/networking](https://developers.google.com/learn/topics/networking)

[https://cloud.google.com/about/locations](https://cloud.google.com/about/locations)

[https://www.blog.google/products/google-cloud/expanding-our-global-infrastructure-new-regions-and-subsea-cables/](https://www.blog.google/products/google-cloud/expanding-our-global-infrastructure-new-regions-and-subsea-cables/)


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


## Serverless Computing


### Introduction

Google Cloud’s serverless platform lets you write code your way without worrying about the underlying infrastructure. Deploy functions or apps as source code or as containers. Build full stack serverless applications with Google Cloud’s storage, databases, machine learning, and more. Easily extend applications with event-driven computing from Google or third-party service integrations. You can even choose to move your serverless workloads to on-premises environments or to the cloud.

[https://www.youtube.com/watch?v=PBw9vD_BO5A](https://www.youtube.com/watch?v=PBw9vD_BO5A)


### Cloud Run

Cloud Run is a managed compute platform that enables you to run stateless containers that are invocable via web requests or Pub/Sub events. 

[http://cloud.run](http://cloud.run/)

Cloud Run is serverless: it abstracts away all infrastructure management, so you can focus on what matters most — building great applications. It is built from [Knative](https://cloud.google.com/knative/), letting you choose to run your containers either fully managed with Cloud Run, in your Google Kubernetes Engine cluster, or in workloads on-premises with Cloud Run for Anthos.

[https://cloud.google.com/run/docs](https://cloud.google.com/run/docs)


#### Quickstart: Build and Deploy

This interactive tutorial can be opened in Cloud Shell editor (theia) and followed step by step.

[https://cloud.google.com/run/docs/quickstarts/build-and-deploy](https://cloud.google.com/run/docs/quickstarts/build-and-deploy)


#### Use Cases

[https://cloud.google.com/run/#section-6](https://cloud.google.com/run/#section-6)

Learn how to deploy serverless containers in 3 environments using Cloud Run and Knative.

[https://www.youtube.com/watch?v=nhwYc4StHIc](https://www.youtube.com/watch?v=nhwYc4StHIc)

A video on migrating kubernetes apps to serverless with Cloud Run on Anthos.

[https://www.youtube.com/watch?v=0T5UliS9j8A](https://www.youtube.com/watch?v=0T5UliS9j8A)


### App Engine

App Engine is a fully managed, serverless platform for developing and hosting web applications at scale. You can choose from several popular languages, libraries, and frameworks to develop your apps, then let App Engine take care of provisioning servers and scaling your app instances based on demand.

[https://cloud.google.com/appengine/docs](https://cloud.google.com/appengine/docs)

Google App Engine makes it easy to focus on your code, while letting us manage your infrastructure.

[https://www.youtube.com/watch?v=2PRciDpqpko](https://www.youtube.com/watch?v=2PRciDpqpko)


### Cloud Functions

[Google Cloud Functions](https://cloud.google.com/functions/docs/concepts/overview) is a lightweight compute solution for developers to create single-purpose, stand-alone functions that respond to Cloud events without the need to manage a server or runtime environment.

[https://cloud.google.com/functions/docs](https://cloud.google.com/functions/docs)

A video tutorial of Cloud Functions that  will show you how to deploy a Cloud Function from a Google Cloud project.  You will learn how to test your function and see your log entries. 

[https://www.youtube.com/watch?v=vM-2O-uKBNQ](https://www.youtube.com/watch?v=vM-2O-uKBNQ)


#### Cloud Functions for .NET

[https://cloud.google.com/blog/products/application-development/introducing-net-google-cloud-functions](https://cloud.google.com/blog/products/application-development/introducing-net-google-cloud-functions)


### Knative

Knative (pronounced kay-nay-tiv) extends [Kubernetes](https://kubernetes.io/docs/concepts/overview/what-is-kubernetes/) to provide a set of middleware components that are essential to build modern, source-centric, and container-based applications that can run anywhere: on premises, in the cloud, or even in a third-party data center. Each of the components under the Knative project attempt to identify common patterns and codify the best practices that are shared by successful, real-world, Kubernetes-based frameworks and applications. Knative components focus on solving mundane but difficult tasks such as:



*   [Deploying a container](https://knative.dev/docs/serving/getting-started-knative-app)
*   [Routing and managing traffic with blue/green deployment](https://knative.dev/docs/serving/samples/blue-green-deployment)
*   [Scaling automatically and sizing workloads based on demand](https://knative.dev/docs/serving/autoscaling)
*   [Binding running services to eventing ecosystems](https://knative.dev/docs/eventing/getting-started)

Developers on Knative can use familiar idioms, languages, and frameworks to deploy functions, applications, or containers workloads.

Knative consists of the Serving and Eventing components:



*   [Eventing](https://knative.dev/docs/eventing) - Management and delivery of events
*   [Serving](https://knative.dev/docs/serving) - Request-driven compute that can scale to zero

[https://knative.dev/](https://knative.dev/)

Run managed serverless containers with Knative.

[https://www.youtube.com/watch?v=wPLjUF1hFCw](https://www.youtube.com/watch?v=wPLjUF1hFCw)


#### Cloud Run

[https://cloud.google.com/blog/products/serverless/knative-based-cloud-run-services-are-ga](https://cloud.google.com/blog/products/serverless/knative-based-cloud-run-services-are-ga)


### Workflows

You can use Workflows to create serverless workflows that link a series of serverless tasks together in an order you define. Combine the power of Google Cloud's APIs, serverless products like Cloud Functions and Cloud Run, and calls to external APIs to create flexible serverless applications. Workflows require no infrastructure management and scales seamlessly with demand, including scaling down to zero.

[https://cloud.google.com/workflows/docs](https://cloud.google.com/workflows/docs)

Build serverless workflows orchestrating various products and API calls within Google Cloud and beyond. 

[https://www.youtube.com/watch?v=Uz8G8fTwwXs](https://www.youtube.com/watch?v=Uz8G8fTwwXs)


### Serverless Predictions at Scale

Cloud Machine Learning Engine Prediction Service can serve TensorFlow models and scale.

[https://www.youtube.com/watch?v=_JCMN8-yhBM](https://www.youtube.com/watch?v=_JCMN8-yhBM)


### Qwiklabs


#### Deploy on Cloud Run

This is a Qwiklab to show you how to deploy a website using Cloud Run.

[Deploy Your Website on Cloud Run](https://www.qwiklabs.com/focuses/10445?parent=catalog)


#### Web Applications on Cloud Run

It is a part of the larger “Quest”.

[Websites and Web Applications](https://www.qwiklabs.com/quests/39?catalog_rank=%7B%22rank%22%3A5%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&search_id=7467936)


#### Monitoring Cloud Functions

You can [view your Cloud Functions](https://cloud.google.com/functions) with their execution times,execution counts, and memory usage in the Cloud Console using [Cloud Monitoring](https://cloud.google.com/monitoring), where you can set up custom alerting on these metrics.

[Monitoring and Logging for Cloud Functions](https://www.qwiklabs.com/focuses/1833?catalog_rank=%7B%22rank%22%3A16%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&parent=catalog&search_id=7468061)


#### Logging in Google Cloud

Learn how to monitor, troubleshoot, and improve your infrastructure and application performance. Guided by the principles of Site Reliability Engineering (SRE), this course features a combination of lectures, demos, hands-on labs, and real-world case studies. In this course, you'll gain experience with full-stack monitoring, real-time log management and analysis, debugging code in production, and profiling CPU and memory usage.

[Logging, Monitoring and Observability in Google Cloud](https://www.qwiklabs.com/courses/1514?catalog_rank=%7B%22rank%22%3A17%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&search_id=7468061)


#### Stackdriver Cloud Functions

In this lab you will learn how to use Cloud Functions to perform lightweight processing of Stackdriver Logging messages.

[Responding to Stackdriver Messages with Cloud Functions](https://www.qwiklabs.com/focuses/8500?catalog_rank=%7B%22rank%22%3A22%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&parent=catalog&search_id=7468090)


## Hybrid and Multi-cloud


### Anthos

Anthos is a modern application management platform that provides a consistent development and operations experience for cloud and on-premises environments. This page provides an overview of each layer of the Anthos infrastructure and shows how you can leverage its features.

[https://cloud.google.com/anthos/docs](https://cloud.google.com/anthos/docs)

Getting started with Anthos.

[https://www.youtube.com/watch?v=DM8p_cnc6ZY](https://www.youtube.com/watch?v=DM8p_cnc6ZY)

A sample deployment for Anthos. 

[https://www.youtube.com/watch?v=qgg1ceR6-es](https://www.youtube.com/watch?v=qgg1ceR6-es)

VM instances can exist on premises, managed by products such as VMWare vSphere, and in public clouds such as AWS or Azure, in addition to Google Cloud Compute Engine instances.


### Anthos Deployments

GKE on-prem is hybrid cloud software that brings Google Kubernetes Engine (GKE) to on-premises data centers. GKE on-prem is a reliable, efficient, and secured way to run Kubernetes clusters anywhere.

[https://cloud.google.com/anthos/gke/docs/on-prem](https://cloud.google.com/anthos/gke/docs/on-prem)


### Anthos Config Management

Anthos Config Management is a key component of Anthos. With Anthos Config Management, you can create a common configuration across all your infrastructure, including custom policies, and apply it both on-premises and in the cloud. Anthos Config Management evaluates changes and rolls them out to all Kubernetes clusters so that your desired state is always reflected.

[https://cloud.google.com/anthos-config-management/docs](https://cloud.google.com/anthos-config-management/docs)

Learn how you can manage your Anthos deployments at scale, using Anthos Config Management.

[https://www.youtube.com/watch?v=nhXJzjITgMA](https://www.youtube.com/watch?v=nhXJzjITgMA)


### Cloud Run for Anthos

Create a cluster enabled for Cloud Run for Anthos on Google Cloud and then deploy a prebuilt sample container to the cluster.

[https://cloud.google.com/run/docs/quickstarts/prebuilt-deploy-gke](https://cloud.google.com/run/docs/quickstarts/prebuilt-deploy-gke)

Learn how Cloud Run lets you adopt the simplicity of serverless on your own terms: on Google’s fully-managed infrastructure, or in your Anthos clusters. 

[https://www.youtube.com/watch?v=0T5UliS9j8A](https://www.youtube.com/watch?v=0T5UliS9j8A)


### Migrate for Anthos

With Migrate for Anthos, you can migrate your VMs from [supported source platforms](https://cloud.google.com/migrate/anthos/docs/migration-prerequisites) to Google Kubernetes Engine or [Anthos](https://cloud.google.com/anthos).

[https://cloud.google.com/migrate/anthos/docs/getting-started](https://cloud.google.com/migrate/anthos/docs/getting-started)

Migrating and modernizing enterprise workloads using Migrate for Anthos.

[https://www.youtube.com/watch?v=8Q1kqWVbKQY](https://www.youtube.com/watch?v=8Q1kqWVbKQY)

A video about migration  and modernization a legacy on-premises application to GKE while gaining better observability and other benefits.

[https://www.youtube.com/watch?v=inEaRCFwovU](https://www.youtube.com/watch?v=inEaRCFwovU)


### Google Cloud Marketplace for Anthos

A Kubernetes app is a containerized application that you can run on your Kubernetes cluster. The Kubernetes apps in Cloud Marketplace include container images and configuration files, such as a kubectl configuration or a Helm chart. When you deploy an app from Cloud Marketplace, the Kubernetes resources are created in your cluster, and you can manage the resources as a group.

[https://cloud.google.com/marketplace/docs/kubernetes-apps](https://cloud.google.com/marketplace/docs/kubernetes-apps)


### Anthos on AWS

Anthos is Google's managed platform for application modernization and delivery, providing consistent automated operations so that an Enterprise can write once and deploy anywhere. This session will provide an overview and technical deep dive into "Extending Anthos to AWS", including capabilities that facilitate automation best practices that span across multi-cloud environments and the freedom to run, deploy and manage applications on the cloud of your choice.

[https://www.youtube.com/watch?v=qnlrEXOGFz4](https://www.youtube.com/watch?v=qnlrEXOGFz4)


### Connect

Connect allows you to connect any of your Kubernetes clusters to Google Cloud. This enables access to cluster and to workload management features, including a unified user interface, [Cloud Console](https://cloud.google.com/cloud-console), to interact with your cluster.

If your network is configured to allow outbound requests, you can configure the Connect Agent to traverse NATs, egress proxies, and firewalls to establish a long-lived, encrypted connection between your cluster's Kubernetes API server and your Google Cloud project. Once this connection is enabled, you can use your own credentials to log back into your clusters and access details about their Kubernetes resources. This effectively replicates the UI experience that is otherwise only available to GKE clusters.

After the connection is established, the Connect Agent software can exchange account credentials, technical details, and metadata about connected infrastructure and workloads necessary to manage them with Google Cloud, including the details of resources, applications, and hardware.

This cluster service data is associated with your Google Cloud project and/or account. Google uses this data to maintain a control plane between your cluster and Google Cloud, to provide you with any Google Cloud services and features you request, including facilitating support, billing, providing updates, and to measure and improve the reliability, quality, capacity, and functionality of Connect and Google Cloud services available through Connect.

You remain in control of what data is sent through Connect.

[https://cloud.google.com/anthos/multicluster-management/connect](https://cloud.google.com/anthos/multicluster-management/connect)


### Qwiklabs


#### Migrate for Anthos

[Anthos](https://cloud.google.com/anthos) is an open source application platform that enables you to modernize your existing applications on your hybrid or multi-cloud environment. You can build new VMs and run them anywhere in a secure manner. Anthos is built on open source technologies pioneered by Google — including Kubernetes, Istio, and Knative — and enables consistency between on-premises and cloud environments.

[Migrate for Anthos: Qwik Start](https://www.qwiklabs.com/focuses/10268?catalog_rank=%7B%22rank%22%3A6%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&parent=catalog&search_id=7467866)


#### Anthos Service Mesh

This intermediate-level quest is unique among Qwiklabs quests. These labs have been curated to give operators hands-on practice with Anthos—a new, open application modernization platform on GCP. Anthos enables you to build and manage modern hybrid applications. Tasks include: installing service mesh, collecting telemetry, and securing your microservices with service mesh policies. 

[Anthos: Service Mesh](https://www.qwiklabs.com/quests/100?catalog_rank=%7B%22rank%22%3A1%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&search_id=7482852)


## Operations

AKA Stackdriver


### Introduction

Monitor, troubleshoot, and improve application performance on your Google Cloud environment.

[https://cloud.google.com/stackdriver/docs](https://cloud.google.com/stackdriver/docs)

Introduction to basic logging and monitoring with Stackdriver with a quick demo.

[https://www.youtube.com/watch?v=LVFr5qW4wO4](https://www.youtube.com/watch?v=LVFr5qW4wO4)


### Cloud Logging

Cloud Logging allows you to store, search, analyze, monitor, and alert on logging data and events from Google Cloud and Amazon Web Services. Using Cloud Logging includes access to the [BindPlane service](https://bluemedora.com/products/bindplane/bindplane-for-stackdriver/), which you can use to collect logging data from over 150 common application components, on-premises systems, and hybrid cloud systems.

[https://cloud.google.com/logging/docs](https://cloud.google.com/logging/docs)

GCP Essentials: Cloud Logging.

[https://www.youtube.com/watch?v=gyDp-Cl_MdA](https://www.youtube.com/watch?v=gyDp-Cl_MdA)


### Cloud Monitoring

Cloud Monitoring collects metrics, events, and metadata from Google Cloud, Amazon Web Services (AWS), hosted uptime probes, and application instrumentation. Using the [BindPlane service](https://bluemedora.com/products/bindplane/bindplane-for-stackdriver/), you can also collect this data from over 150 common application components, on-premise systems, and hybrid cloud systems. Google Cloud's operations suite ingests that data and generates insights via dashboards, charts, and alerts. BindPlane is included with your Google Cloud project at no additional cost.

[https://cloud.google.com/monitoring/docs](https://cloud.google.com/monitoring/docs)

Getting started with Cloud Monitoring.

[https://www.youtube.com/watch?v=wY8cmFY4ua8](https://www.youtube.com/watch?v=wY8cmFY4ua8)


#### Cloud Monitoring Agents

[https://cloud.google.com/monitoring/agent](https://cloud.google.com/monitoring/agent)


#### Dashboards

[https://cloud.google.com/monitoring/charts/dashboards](https://cloud.google.com/monitoring/charts/dashboards)


#### Metrics Explorer

[https://cloud.google.com/monitoring/charts/metrics-explorer](https://cloud.google.com/monitoring/charts/metrics-explorer)


### Cloud Trace

Cloud Trace is a distributed tracing system for Google Cloud that collects latency data from applications and displays it in near real-time in the [Google Cloud Console](https://console.cloud.google.com/).

[https://cloud.google.com/trace/docs](https://cloud.google.com/trace/docs)

Cloud Trace is a feature of the Google Cloud Platform that allows you to view the RPCs (remote procedure calls) invoked by your App Engine application and to view and analyze the time taken to complete each RPC and the overall latency of processing your applications requests.

[https://www.youtube.com/watch?v=NCFDqeo7AeY](https://www.youtube.com/watch?v=NCFDqeo7AeY)


### Cloud Debugger

Cloud Debugger is a feature of Google Cloud Platform that lets you inspect the state of an application, at any code location, without stopping or slowing down the running app. Cloud Debugger makes it easier to view the application state without adding logging statements.

[https://cloud.google.com/debugger/docs](https://cloud.google.com/debugger/docs)

Cloud Debugger makes it easier to view the application state at any point in the code without any modifications to your code.  

[https://www.youtube.com/watch?v=DCtLE6zPMdQ](https://www.youtube.com/watch?v=DCtLE6zPMdQ)


### Cloud Profiler

Cloud Profiler is a statistical, low-overhead profiler that continuously gathers CPU usage and memory-allocation information from your production applications. It attributes that information to the application's source code, helping you identify the parts of the application consuming the most resources, and otherwise illuminating the performance characteristics of the code.

[https://cloud.google.com/profiler/docs](https://cloud.google.com/profiler/docs)

Introduction to Stackdriver Profiler.

[https://www.youtube.com/watch?v=KXjPhadwr8k](https://www.youtube.com/watch?v=KXjPhadwr8k)


### Error Reporting

Error Reporting aggregates and displays errors produced in your running cloud services.

[https://cloud.google.com/error-reporting/docs](https://cloud.google.com/error-reporting/docs)

Error reporting can be useful in identifying and resolving bugs in your application. 

[https://www.youtube.com/watch?v=GANi9eRxhHs](https://www.youtube.com/watch?v=GANi9eRxhHs)


### Service Level Monitoring

Service monitoring and the SLO API help you manage your services like Google manages its own services. 

[https://cloud.google.com/stackdriver/docs/solutions/slo-monitoring](https://cloud.google.com/stackdriver/docs/solutions/slo-monitoring)

Basics of Service Level Monitoring.

[https://www.youtube.com/watch?v=u84TKyX8SfU](https://www.youtube.com/watch?v=u84TKyX8SfU)


### Qwiklabs


#### Operations Suite

In this fundamental-level quest, you will learn the ins and outs of Google Cloud's operations suite, an important service for generating insights into the health of your applications. It provides a wealth of information in application monitoring, report logging, and diagnoses. The labs in this quest will give you hands-on practice with and will teach you how to monitor virtual machines, generate logs and alerts, and create custom metrics for application data.

[Google Cloud's Operations Suite](https://www.qwiklabs.com/quests/35?catalog_rank=%7B%22rank%22%3A6%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&search_id=7468028)


#### Cloud Monitoring

In this fundamental-level quest, you will learn the ins and outs of Google Cloud's operations suite, an important service for generating insights into the health of your applications. It provides a wealth of information in application monitoring, report logging, and diagnoses. The labs in this quest will give you hands-on practice with and will teach you how to monitor virtual machines, generate logs and alerts, and create custom metrics for application data. 

[Monitor and Log with Google Cloud Operations Suite](https://www.qwiklabs.com/quests/143?catalog_rank=%7B%22rank%22%3A2%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&search_id=7468028)


#### Cloud Trace

When supporting a production system that services HTTP requests or provides an API, it is important to measure the latency of your endpoints to detect when a system's performance is not operating within specification. In monolithic systems this single latency measure may be useful to detect and diagnose deteriorating behavior. With modern microservice architectures, however, this becomes much more difficult because a single request may result in numerous additional requests to other systems before the request can be fully handled. Deteriorating performance in an underlying system may impact all other systems that rely on it. While latency can be measured at each service endpoint, it can be difficult to correlate slow behavior in the public endpoint with a particular sub-service that is misbehaving.

[Using Cloud Trace on Kubernetes Engine](https://www.qwiklabs.com/focuses/5159?catalog_rank=%7B%22rank%22%3A19%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&parent=catalog&search_id=7468017)


#### Cloud Logging

Cloud Logging is a fully managed service that performs at scale. It can ingest application and system log data from thousands of VMs and, even better, analyze all that log data in real time. In this fundamental-level Quest, you learn how to store, search, analyze, monitor, and alert on log data and events from Google Cloud. 

[Cloud Logging](https://www.qwiklabs.com/quests/81?catalog_rank=%7B%22rank%22%3A1%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&search_id=7468028)


#### Application Logs

In this hands-on lab, you learn how to use Cloud Logging to accumulate application logs in a single place, filter to reach the required log, understand how to create logs based metrics for advanced analysis, examine the audit logs use case, and export logs for compliance and/or advanced analysis needs.

[Fundamentals of Cloud Logging](https://www.qwiklabs.com/focuses/10911?catalog_rank=%7B%22rank%22%3A12%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&parent=catalog&search_id=7468061)


#### BigQuery Logging

In this lab you view the BigQuery logs inside Cloud Logging, setup a sink to export them back into BigQuery, and then use SQL to analyze the logs.

[Using BigQuery and Cloud Logging to Analyze BigQuery Usage](https://www.qwiklabs.com/focuses/6100?catalog_rank=%7B%22rank%22%3A15%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&parent=catalog&search_id=7468061)


## Security and Identity


### Introduction

[https://www.youtube.com/watch?v=UOdUC8DhprQ](https://www.youtube.com/watch?v=UOdUC8DhprQ)

[https://www.youtube.com/watch?v=kd33UVZhnAA](https://www.youtube.com/watch?v=kd33UVZhnAA)


#### Authentication Options

[https://cloud.google.com/blog/products/identity-security/identity-and-authentication-the-google-cloud-way](https://cloud.google.com/blog/products/identity-security/identity-and-authentication-the-google-cloud-way)


### IAM

Cloud IAM is Google Cloud Platform’s unified system for managing access to resources and assigning permissions for users and services to access those resources.  This video will take you through the basic terms and concepts you need to use Cloud IAM.

[https://www.youtube.com/watch?v=96HlT4f2AUU](https://www.youtube.com/watch?v=96HlT4f2AUU)

Cloud Identity and Access Management (IAM) lets administrators authorize who can take action on specific resources, giving you full control and visibility to manage Google Cloud resources centrally. For enterprises with complex organizational structures, hundreds of workgroups, and many projects, Cloud IAM provides a unified view into security policy across your entire organization, with built-in auditing to ease compliance processes. Cloud IAM provides a simple and consistent access control interface for all Google Cloud services. Learn one access control interface and apply that knowledge to all Google Cloud resources. Prior to Cloud IAM, you could only grant Owner, Editor, or Viewer roles to users. A wide range of services and resources now surface additional Cloud IAM roles out of the box. For example, the Pub/Sub service exposes Publisher and Subscriber roles in addition to the Owner, Editor, and Viewer roles. Create and manage Cloud IAM policies using the Google Cloud Console, the Cloud IAM methods, and the gcloud command line tool.

[https://cloud.google.com/iam](https://cloud.google.com/iam)


#### Roles

[https://cloud.google.com/iam/docs/understanding-roles](https://cloud.google.com/iam/docs/understanding-roles)


#### Service Accounts

[https://cloud.google.com/iam/docs/service-accounts](https://cloud.google.com/iam/docs/service-accounts)


### Cloud Identity API

Cloud Identity API is an API for provisioning and managing identity resources.

[https://cloud.google.com/identity/docs](https://cloud.google.com/identity/docs)


### Identity-Aware Proxy

Identity-Aware Proxy (IAP) lets you manage access to applications running in the App Engine standard environment, App Engine flexible environment, Compute Engine, and GKE. IAP establishes a central authorization layer for applications accessed by HTTPS, so you can adopt an application-level access control model instead of using network-level firewalls. When you turn on IAP, you must also use [signed headers](https://cloud.google.com/iap/docs/signed-headers-howto) or the App Engine standard environment [Users API](https://cloud.google.com/appengine/docs/standard#users) to secure your app.

[https://cloud.google.com/iap/docs](https://cloud.google.com/iap/docs)

Identity Aware Proxy enables you to configure secure controlled access to your applications so you can enforce "who can see what" access control at the application layer.  You don't need client software, remote access VPNs, firewalls, network configurations. 

[https://www.youtube.com/watch?v=XqMY-rPk3MY](https://www.youtube.com/watch?v=XqMY-rPk3MY)


### Context-Aware Access

Based on the [BeyondCorp](https://cloud.google.com/beyondcorp) security model, Context-Aware Access is an approach that utilizes a variety of Google Cloud offerings to enforce granular access control based on a user's identity and context of the request.

[https://cloud.google.com/context-aware-access/docs/overview](https://cloud.google.com/context-aware-access/docs/overview)

Envisioned in 2011, the BeyondCorp security model leverages identity and context to evaluate trust for access decisions rather than using the corporate network as the perimeter. 

[https://www.youtube.com/watch?v=Sq9gp8KBsY0](https://www.youtube.com/watch?v=Sq9gp8KBsY0)


### Identity Platform

Identity Platform provides back-end services, SDKs, and UI libraries that make it easier to authenticate users to your apps and services.

[https://cloud.google.com/identity-platform/docs](https://cloud.google.com/identity-platform/docs)

Manage the identities of customers, partners, and Things through Identity Platform.

[https://www.youtube.com/watch?v=O_O5Hb1bJyw](https://www.youtube.com/watch?v=O_O5Hb1bJyw)


### Managed Services for Microsoft Active Directory

Managed Service for Microsoft Active Directory is a highly available, hardened Google Cloud service running actual Microsoft AD that enables you to manage your cloud-based AD-dependent workloads, automate AD server maintenance and security configuration, and connect your on-premises AD domain to the cloud.

[https://cloud.google.com/managed-microsoft-ad/docs](https://cloud.google.com/managed-microsoft-ad/docs)


### Resource Manager

Google Cloud provides container resources such as organizations and projects that allow you to group and hierarchically organize other Google Cloud resources. This hierarchical organization helps you manage common aspects of your resources, such as access control and configuration settings. The Resource Manager API enables you to programmatically manage these container resources.

[https://cloud.google.com/ntresource-manager/docs](https://cloud.google.com/resource-manager/docs)

Setting up your Google Cloud Platform resources correctly can save you a lot of trouble down the road. 

[https://www.youtube.com/watch?v=MzclA_hdNLY](https://www.youtube.com/watch?v=MzclA_hdNLY)

Folders are a powerful tool for administering GCP resources in Cloud Resource Manager. Watch this demo video to learn how to get started using folders to help organize and control your cloud resources.

[https://www.youtube.com/watch?v=0oJZhlgDbg8](https://www.youtube.com/watch?v=0oJZhlgDbg8)


### Security Key enforcement

Service to enforce usage of security keys to prevent account takeovers.

[https://vecta.io/symbols/4/google-cloud-platform/44/security-key-enforcement](https://vecta.io/symbols/4/google-cloud-platform/44/security-key-enforcement)

Use 2-Step Verification to protect accounts from unauthorized access. 2-Step Verification puts an extra barrier between your business and cybercriminals who try to steal usernames and passwords to access business data. Turning on 2-Step Verification is the single most important action you can take to protect your business.

[https://support.google.com/cloudidentity/answer/175197/](https://support.google.com/cloudidentity/answer/175197/)

Security in the Cloud vs. on-prem. Sharing responsibility of security in the Cloud.

[https://www.youtube.com/watch?v=wDwQ1YMEyE8](https://www.youtube.com/watch?v=wDwQ1YMEyE8)


### Titan Security Keys

Titan Security Keys are built with a hardware chip that includes firmware engineered by Google to verify the key’s integrity. This helps to ensure that the keys haven’t been physically tampered with.

[https://cloud.google.com/titan-security-key](https://cloud.google.com/titan-security-key)


### Access Transparency

Access Transparency provides you with logs that capture the actions Google personnel take when accessing your content. You might be familiar with [Cloud Audit Logs](https://cloud.google.com/logging/docs/audit), which can help you answer questions about "who did what, where, and when?" in your Google Cloud projects. While Cloud Audit Logs provides these logs about the actions taken by members within your own organization, Access Transparency provides logs of the actions taken by Google personnel.

[https://cloud.google.com/logging/docs/audit/access-transparency-overview](https://cloud.google.com/logging/docs/audit/access-transparency-overview)

[https://www.youtube.com/watch?v=6BCuIBO0Mhg](https://www.youtube.com/watch?v=6BCuIBO0Mhg)


### Binary Authorization

Binary Authorization is a service on Google Cloud that provides software supply-chain security for applications that run in the cloud. Binary Authorization is a service on Google Cloud Platform (GCP) that provides software supply-chain security when deploying container-based applications. Binary Authorization extends Google Kubernetes Engine (GKE) and enforces security policies at deploy time. Binary Authorization works with container images from Container Registry or another container image registry. With Binary Authorization, you can automatically and digitally check each component of your software supply chain, ensuring the quality and integrity of your software before an application is deployed to your production environment.

[https://cloud.google.com/binary-authorization/docs](https://cloud.google.com/binary-authorization/docs)

Check out a demo of Binary Authorization, a Google Cloud Platform security feature. Binary Authorization is a deploy-time security control that ensures only trusted container images are deployed on Kubernetes Engine.

[https://www.youtube.com/watch?v=mi50OJq6wd0](https://www.youtube.com/watch?v=mi50OJq6wd0)


### Cloud Asset Inventory

Cloud Asset Inventory provides inventory services based on a time series database. This database keeps a five-week history of Google Cloud [asset](https://cloud.google.com/asset-inventory/docs/overview#assets) metadata.

[https://cloud.google.com/asset-inventory/docs/overview](https://cloud.google.com/asset-inventory/docs/overview)


### Cloud Data Loss Prevention

Welcome to Cloud Data Loss Prevention (DLP)! Cloud DLP provides access to a powerful sensitive data inspection, classification, and de-identification platform.

[https://cloud.google.com/dlp/docs](https://cloud.google.com/dlp/docs)

Learn how to automatically discover and redact sensitive data everywhere. Try the Data Loss Prevention: Qwik Start lab here:[ http://bit.ly/2QmSZsr](https://www.youtube.com/redirect?event=video_description&v=GArEb2e9jGk&q=http%3A%2F%2Fbit.ly%2F2QmSZsr&redir_token=QUFFLUhqbERxVzNuUE9wY3lHeHJDWGFuZkN4TkExNG9UUXxBQ3Jtc0trbGZ2dW5TYjJYd2FwQmFqZWlIek16QjdScG43R1hXekpkVU9sZTM5dFk1RjNJYkRRaFpEZ3lIdDhuRlVfQVltcVd2MF85aE1YUk9BMzAzOElNSW9qTndXejZURkxiY1hOdXRxTlEwTjJtVlRWTUY4cw%3D%3D)

[https://www.youtube.com/watch?v=GArEb2e9jGk](https://www.youtube.com/watch?v=GArEb2e9jGk)


### Cloud HSM

Cloud HSM is a cloud-hosted Hardware Security Module (HSM) service that allows you to host encryption keys and perform cryptographic operations in a cluster of [FIPS 140-2 Level 3](https://csrc.nist.gov/publications/detail/fips/140/2/final) certified HSMs. Google manages the HSM cluster for you, so you don't need to worry about clustering, scaling, or patching. Because Cloud HSM uses Cloud KMS as its front end, you can leverage all the conveniences and features that Cloud KMS provides.

[https://cloud.google.com/kms/docs/hsm](https://cloud.google.com/kms/docs/hsm)

[https://www.youtube.com/watch?v=DB6UfKFo3ds](https://www.youtube.com/watch?v=DB6UfKFo3ds)


### Security Command Center

Security Command Center is the canonical security and data risk database for Google Cloud. Security Command Center enables you to understand your security and data attack surface by providing asset inventory, discovery, search, and management.

[https://cloud.google.com/security-command-center/docs](https://cloud.google.com/security-command-center/docs)

[https://www.youtube.com/watch?v=k7ZEfAocMq4](https://www.youtube.com/watch?v=k7ZEfAocMq4)


### VPC Service Controls

With VPC Service Controls, administrators can define a security perimeter around resources of Google-managed services to control communication to and between those services.

[https://cloud.google.com/vpc-service-controls/docs](https://cloud.google.com/vpc-service-controls/docs)

VPC Service Controls enables you to establish security perimeters around sensitive data in Google Cloud Platform services such as Google Cloud Storage and BigQuery. 

[https://www.youtube.com/watch?v=EXwJFL24QzY](https://www.youtube.com/watch?v=EXwJFL24QzY)


### Incident Response and Management

The incident response problem space can be divided into three categories: people, process, and data management. Users have long had access to solid people-management solutions (on-call rotation schedulers, etc.) and Google’s SRE book outlines their Incident Management at Google (IMAG) process. In this presentation, attendees will learn the benefits of data management and how Google Cloud Platform (GCP) is providing technology to leverage the idea and accelerate users’ investigations. Attendees will see live demos of Stackdriver Incident Response and Management (IRM) Insights and the supporting GCP technology that makes the innovation possible.

[https://www.youtube.com/watch?v=VXqfbp_zE0c](https://www.youtube.com/watch?v=VXqfbp_zE0c)


### Phishing Protection

Phishing Protection is a phishing countermeasure platform that helps to detect phishing attacks against your users. The Phishing Protection Submission API also enables you to submit URLs suspected to be unsafe to [Safe Browsing](http://safebrowsing.google.com/). Any URLs that are confirmed to match the Safe Browsing Policies will be added to the Safe Browsing list, which is used by over three billion devices to show warnings when a user visits a known unsafe web resource. Common sources of these URLs are customer reports or internal phishing detection results.

[https://cloud.google.com/phishing-protection/docs](https://cloud.google.com/phishing-protection/docs)

A video to show you how security keys prevent phishing attacks by recognizing a domain name and using its hidden private key. 

[https://www.youtube.com/watch?v=c9EOETFnB74](https://www.youtube.com/watch?v=c9EOETFnB74)


### Cloud KMS

A cloud-hosted key management service that lets you manage symmetric and asymmetric cryptographic keys for your cloud services the same way you do on-premises. You can generate, use, rotate, and destroy AES256, RSA 2048, RSA 3072, RSA 4096, EC P256, and EC P384 cryptographic keys. Toggle between software- and hardware-protected encryption keys with the press of a button. Host encryption keys and perform cryptographic operations in FIPS 140-2 Level 3 certified HSMs. With this fully managed service, you can protect your most sensitive workloads without the need to worry about the operational overhead of managing an HSM cluster. Encrypt data in [BigQuery](https://cloud.google.com/bigquery) and [Compute Engine](https://cloud.google.com/compute) with encryption keys that are stored and managed in a third-party key management system that’s deployed outside Google’s infrastructure. External Key Manager allows you to maintain separation between your data at rest and your encryption keys while still leveraging the power of cloud for compute and analytics. Key Access Justifications works with [Cloud EKM](https://cloud.google.com/blog/products/identity-security/cloud-external-key-manager-now-in-beta) to greatly advance the control you have over your data. It’s the only product that gives you visibility into every request for an encryption key, a justification for that request, and a mechanism to approve or deny decryption in the context of that request. 

[https://cloud.google.com/security-key-management](https://cloud.google.com/security-key-management)

Learn about how Google automatically encrypts your data and how to take control of encryption by managing your own keys. 

[https://www.youtube.com/watch?v=38_dWxOHUN8](https://www.youtube.com/watch?v=38_dWxOHUN8)


### reCAPTCHA Enterprise

Google has been defending millions of sites with reCAPTCHA for almost a decade. reCAPTCHA Enterprise is an extension of that effort to help enterprises detect other types of fraudulent activity on their sites, like scraping, credential stuffing, and automated account creation. reCAPTCHA Enterprise offers enhanced detection with more granular scores, reason codes for risky events, and the ability to tune your site-specific model. reCAPTCHA Enterprise is a service that protects your site from spam and abuse. reCAPTCHA Enterprise builds on the existing reCAPTCHA API which uses advanced risk analysis techniques to tell humans and bots apart. reCAPTCHA Enterprise adds enhancements specifically designed to protect enterprise businesses, such as more granular scoring and returning reason codes with low scores to aid in analysis.

[https://cloud.google.com/recaptcha-enterprise/docs](https://cloud.google.com/recaptcha-enterprise/docs)

See how reCAPTCHA Enterprise can help protect your websites from fraud and abuse.

[https://www.youtube.com/watch?v=ic3Fj2B1LR4](https://www.youtube.com/watch?v=ic3Fj2B1LR4)


### Web Risk

Web Risk is a new enterprise security product that lets your client applications check URLs against Google's constantly updated lists of unsafe web resources.

[https://cloud.google.com/web-risk/docs](https://cloud.google.com/web-risk/docs)


### Identity & Security Topics

[https://cloud.google.com/blog/products/identity-security](https://cloud.google.com/blog/products/identity-security)


### Data Governance 


#### BigQuery Column-level security

[https://cloud.google.com/blog/products/data-analytics/data-governance-new-ways-to-securely-access-and-discover-data](https://cloud.google.com/blog/products/data-analytics/data-governance-new-ways-to-securely-access-and-discover-data)


### Qwiklabs


#### Cloud KMS

In this lab you'll learn how to use some advanced features of Google Cloud Security and Privacy APIs, including:



*   Setting up a secure Cloud Storage bucket
*   Managing keys and encrypted data using Key Management Storage
*   Viewing Cloud Storage audit logs

You'll take abridged data from the Enron Corpus, encrypt it and load it into Cloud Storage.

[Getting Started with Cloud KMS](https://www.qwiklabs.com/focuses/1713?catalog_rank=%7B%22rank%22%3A20%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&parent=catalog&search_id=7468061)


#### Security & Identity

Security is an uncompromising feature of Google Cloud services, and Google Cloud has developed specific tools for ensuring safety and identity across your projects. In this fundamental-level quest, you will get hands-on practice with Google Cloud’s Identity and Access Management (IAM) service, which is the go-to for managing user and virtual machine accounts.

[Security & Identity Fundamentals](https://www.qwiklabs.com/quests/40?catalog_rank=%7B%22rank%22%3A1%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&search_id=7482841)


#### IAM

In this fundamental-level quest, you will get hands-on practice with Google Cloud’s Identity and Access Management (IAM) service, which is the go-to for managing user and virtual machine accounts. You will get experience with network security by provisioning VPCs and VPNs, and learn what tools are available for security threat and data loss protections.

[Ensure Access & Identity in Google Cloud](https://www.qwiklabs.com/quests/150?catalog_rank=%7B%22rank%22%3A3%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&search_id=7482841)


## Infrastructure as Code


### Introduction

Provisioning compute resources has traditionally been hard to manage, not scalable, and prone to error, so what other techniques can you use to make sure you’re ready to meet demand? In this episode of Season of Scale, Stephanie Wong explains why you should adopt an Infrastructure as code (IaC) strategy, so you can automate the creation of your cloud resources, create templates, and store config files with the help of tools like Google Cloud Deployment Manager.

[https://cloud.google.com/solutions/infrastructure-as-code](https://cloud.google.com/solutions/infrastructure-as-code)


#### Google Cloud Deployment Manager

[https://www.youtube.com/watch?v=z-caqPtEw58](https://www.youtube.com/watch?v=z-caqPtEw58)


##### Cloud Deployment Quickstart

[https://cloud.google.com/deployment-manager/docs/quickstart](https://cloud.google.com/deployment-manager/docs/quickstart)


##### Deployments

[https://cloud.google.com/deployment-manager/docs/deployments](https://cloud.google.com/deployment-manager/docs/deployments)


##### Manifests

[https://cloud.google.com/deployment-manager/docs/deployments/viewing-manifest](https://cloud.google.com/deployment-manager/docs/deployments/viewing-manifest)


##### Cloud Deployment Manager Deploying Network Load Balanced Logbook 

[https://cloud.google.com/deployment-manager/docs/create-advanced-deployment](https://cloud.google.com/deployment-manager/docs/create-advanced-deployment)


##### Shard VPC with Cloud Deployment Manager

[https://cloud.google.com/solutions/shared-vpc-with-deployment-manager](https://cloud.google.com/solutions/shared-vpc-with-deployment-manager)


##### Solutions that use Cloud Deployment Manager

[https://cloud.google.com/docs/tutorials?sortBy=relevance#%22deployment%20manager%22](https://cloud.google.com/docs/tutorials?sortBy=relevance#%22deployment%20manager%22)


##### More examples

[https://github.com/GoogleCloudPlatform/deploymentmanager-samples/tree/master/examples/v2](https://github.com/GoogleCloudPlatform/deploymentmanager-samples/tree/master/examples/v2)


#### Cloud Foundation Toolkit

[https://cloud.google.com/foundation-toolkit/](https://cloud.google.com/foundation-toolkit/)


### Terraform 


#### Introduction

Terraform's infrastructure-as-code (IaC) approach supports [DevOps](https://cloud.google.com/devops) best practices for change management, letting you manage Terraform configuration files in source control to maintain an ideal provisioning state for testing and production environments.

[https://cloud.google.com/docs/terraform](https://cloud.google.com/docs/terraform)

Terraform is a tool from Hashicorp for building, changing, and versioning infrastructure safely and efficiently. Terraform can manage existing and popular service providers as well as custom in-house solutions.

[https://www.terraform.io/intro/index.html](https://www.terraform.io/intro/index.html)


#### Getting Started on GCP

[https://cloud.google.com/community/tutorials/getting-started-on-gcp-with-terraform](https://cloud.google.com/community/tutorials/getting-started-on-gcp-with-terraform)

Defining and managing your development, test, staging, and production environments using infra-as-code tools such as [Deployment Manager](https://cloud.google.com/deployment-manager) or [Terraform](https://www.terraform.io/) is a common practice. Ensuring that any changes you make to your environment config definitions are “safe” remains challenging, though.

[https://www.youtube.com/watch?v=3vfXQxWJazM](https://www.youtube.com/watch?v=3vfXQxWJazM)


##### Managing infrastructure as code with Terraform, Cloud Build, and GitOps

[https://cloud.google.com/solutions/managing-infrastructure-as-code](https://cloud.google.com/solutions/managing-infrastructure-as-code)


##### Hashicorp tutorials

[https://learn.hashicorp.com/collections/terraform/gcp-get-started#gcp](https://learn.hashicorp.com/collections/terraform/gcp-get-started#gcp)


##### Terraform Modules for GCP

[https://github.com/terraform-google-modules](https://github.com/terraform-google-modules)


##### Examples

[https://github.com/terraform-google-modules/docs-examples](https://github.com/terraform-google-modules/docs-examples)


#### Terraformer

Reverse of terraform.  

[https://github.com/GoogleCloudPlatform/terraformer](https://github.com/GoogleCloudPlatform/terraformer)


#### A list of URLs related to terraform

[https://github.com/shuaibiyy/awesome-terraform](https://github.com/shuaibiyy/awesome-terraform)


### Pulumi

[https://www.pulumi.com/docs/get-started/gcp/](https://www.pulumi.com/docs/get-started/gcp/)


### Ansible

An opinionated look at how ansible and terraform complement one another in a provisioner/configuration management separated view. A key takeaway is a simplified workflow for sysadmins/operators in cloud management that can be applied in multi-cloud/hybrid cloud scenarios.

[https://www.youtube.com/watch?v=utztQWTewWU](https://www.youtube.com/watch?v=utztQWTewWU)


### Qwiklabs


#### Terraform Quest

[https://www.qwiklabs.com/quests/44](https://www.qwiklabs.com/quests/44)


#### Terraform

In this Quest, the experienced user of Google Cloud will learn how to describe and launch cloud resources with Terraform, an open source tool that codifies APIs into declarative configuration files that can be shared amongst team members, treated as code, edited, reviewed, and versioned. In these nine hands-on labs, you will work with example templates and understand how to launch a range of configurations, from simple servers, through full load-balanced applications.

[Managing Cloud Infrastructure with Terraform](https://www.qwiklabs.com/quests/44?catalog_rank=%7B%22rank%22%3A1%2C%22num_filters%22%3A1%2C%22has_search%22%3Atrue%7D&search_id=7467726)


#### VM Migration

Google Cloud’s four step structured Cloud Migration Path Methodology provides a defined and repeatable path for users to follow when migrating and modernizing Virtual Machines. In this quest, you will get hands-on practice with Google’s current solution set for VM assessment, planning, migration, and modernization. You will start by analyzing your lab environment and building assessment reports with CloudPhysics and StratoZone, then build a landing zone within Google Cloud leveraging Terraform’s infrastructure-as-code templates, next you will manually transform a two-tier application into a cloud-native workload running on Kubernetes, and finally, transform a VM workload into Kubernetes with Migrate for Anthos and migrate a VM between cloud environments.

[VM Migration](https://www.qwiklabs.com/quests/87?catalog_rank=%7B%22rank%22%3A2%2C%22num_filters%22%3A1%2C%22has_search%22%3Atrue%7D&search_id=7467726)


## Google Maps Platform


### Introduction

Google Maps Platform includes Maps SDKs for Android and iOS, Maps Static API,

Maps JavaScript API, Street View Static API, Maps URLs and Maps Embed API. Routes APIs support Directions API, Distance Matrix API and Roads API.  Places SDK for Android and iOS add rich details for places. Places Library, Maps JavaScript API, Places API, Geocoding API, Geolocation API and Time Zone API provide rich location and time zone data.

[https://developers.google.com/maps/documentation/](https://developers.google.com/maps/documentation/)


### Solving business problems with Google Maps API

[https://www.youtube.com/watch?v=UzMEtXsMM08](https://www.youtube.com/watch?v=UzMEtXsMM08)


### Qwiklabs


#### Google Maps

In this quest you will use several tools available in Google Cloud to manipulate data and create a Google Map - map location details to find subway stations or a business; use geocoding and Apps Script to send an email of a map; visualize data on a customized map; and build a server-side proxy to create a map on a mobile device.

[Creating with Google Maps](https://www.qwiklabs.com/quests/103?catalog_rank=%7B%22rank%22%3A9%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&search_id=7467888)


## Google Workspace

AKA G-Suite


### Introduction

Similar to G Suite, all Google Workspace plans provide a custom email for your business and includes collaboration tools like Gmail, Calendar, Meet, Chat, Drive, Docs, Sheets, Slides, Forms, Sites, and more. 

[https://workspace.google.com/](https://workspace.google.com/)


### YouTube channel for Google Workspace

[https://www.youtube.com/channel/UCBmwzQnSoj9b6HzNmFrg_yw](https://www.youtube.com/channel/UCBmwzQnSoj9b6HzNmFrg_yw)


### Google Workspace Learning Center

[https://support.google.com/a/users#!/&topic=9296556](https://support.google.com/a/users#!/&topic=9296556)


### G Suite tutorial for beginners

[https://www.youtube.com/watch?v=wJ3S7kFFypU](https://www.youtube.com/watch?v=wJ3S7kFFypU)


### Introduction to G Suite Development tools

[https://www.youtube.com/watch?v=NqumcYgj5LI](https://www.youtube.com/watch?v=NqumcYgj5LI)


### G Suite REST APIs

[https://www.youtube.com/watch?v=ftxroBc7mi4](https://www.youtube.com/watch?v=ftxroBc7mi4)


### Qwiklabs


#### Essentials

G Suite is Google's Collaborative Applications platform, delivered from Google Cloud. In this introductory-level quest, you will get hands-on practice with G Suite’s core applications from a user perspective. Although there are many more applications and tool components to G Suite than are covered here, you will get experience with the primary apps: Gmail, Calendar, Sheets and a handful of others.

[G Suite Essentials](https://www.qwiklabs.com/quests/65?catalog_rank=%7B%22rank%22%3A1%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&search_id=7482904)


#### Integrations

This Quest of hands-on labs demonstrates the power of integrating Google Cloud services and tools with G Suite applications. With integration technologies like the Clasp Command Line environment, you will create and publish web apps and add-ons for G Suite products: Sheets, Docs, Forms, and Slides. In other labs you'll create direct connections to Google Cloud data sources using the BigQuery API, Sheets, and Slides to collect, analyze and present data.

[G Suite: Integrations](https://www.qwiklabs.com/quests/51?catalog_rank=%7B%22rank%22%3A2%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&search_id=7482904)


#### Certification Practice Lab

This practice lab helps you become familiar with the structure and types of questions used in the G Suite certification exam. The lab is helpful to anyone who is planning to take the exam.

[G Suite Certification: Practice Lab](https://www.qwiklabs.com/focuses/4051?catalog_rank=%7B%22rank%22%3A5%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&parent=catalog&search_id=7482904)


#### Gmail

Gmail is an email service developed by Google. Gmail stores your email safely in the cloud, allowing you to access it from any computer or device with a web browser. You can also quickly organize and find important email, as well as read and draft email without an internet connection.

[Gmail: Getting Started](https://www.qwiklabs.com/focuses/5825?catalog_rank=%7B%22rank%22%3A13%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&parent=catalog&search_id=7482915)


#### Shared Drives

Shared drives is a shared space where teams can easily store, search, and access their files anywhere, from any device. In Shared drive, files belong to the team. If members leave, the files stay exactly where they are so your team can continue to share information and get work done. In this lab you set up and use Shared drive.

[Shared Drives: Getting Started](https://www.qwiklabs.com/focuses/5829?catalog_rank=%7B%22rank%22%3A14%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&parent=catalog&search_id=7482915)


#### Meet

[Google Meet](https://apps.google.com/meet/) is a video conferencing application that lets you hold impromptu video meetings on the go, virtual training classes around the world, remote interviews, and much more. 

[Google Meet: Getting Started](https://www.qwiklabs.com/focuses/5831?catalog_rank=%7B%22rank%22%3A15%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&parent=catalog&search_id=7482915)


#### Google Drive

With Google Drive, you can store all your files in the cloud, including photos, Microsoft® Word® documents, Excel® spreadsheets, and more. You can also make changes to a Word file using Google Docs, or convert your Word files to Google Docs, Sheets, or Slides.

[Google Drive: Getting Started](https://www.qwiklabs.com/focuses/5827?catalog_rank=%7B%22rank%22%3A16%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&parent=catalog&search_id=7482915)


#### Sites

Google Sites is a website building platform for businesses and business teams. With Google Sites, you drag and drop content to easily build internal project hubs, team sites, public-facing websites, and more—all without designer, programmer, or IT help. In this lab, you explore how to use Google Sites to build and manage a website. You then share the site with people in your organization to collaborate on the content.

[Google Sites: Getting Started](https://www.qwiklabs.com/focuses/5830?catalog_rank=%7B%22rank%22%3A17%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&parent=catalog&search_id=7482915)


#### Sheets

Google Sheets is a cloud-based application that provides advanced, fast, online spreadsheets. Designed with collaboration and convenience in mind, you can analyze data with charts and filters, handle task lists, create project plans, and more with your team from any online device. All changes are saved automatically and in one place. Use Google Sheets to create, edit, and collaborate wherever you are.

[Google Sheets: Getting Started](https://www.qwiklabs.com/focuses/5828?catalog_rank=%7B%22rank%22%3A11%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&parent=catalog&search_id=7482915)


#### Calendar

Google Calendar is an online, integrated calendar designed for teams. You can quickly schedule meetings and events and get reminders about upcoming activities, so you always know what’s next. It’s easy to share your schedule with others and create multiple calendars that you and your team can use together.

[Google Calendar: Getting Started](https://www.qwiklabs.com/focuses/5826?catalog_rank=%7B%22rank%22%3A12%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&parent=catalog&search_id=7482915)

G Suite by Google Cloud is your go-to solution for productivity tools. Get more done with seamless collaboration tools, a simple management interface, and enterprise-level security and reliability. Easily add users, manage devices and configure security and settings so your data stays safe.


#### G Suite Administration

[G Suite Admin Getting Started - Personalization](https://www.qwiklabs.com/focuses/1724?catalog_rank=%7B%22rank%22%3A7%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&parent=catalog&search_id=7482904)


#### Hangouts Chat Bot

Hangouts Chat bots provide easy-to-use access points to your organization's data and services. Users can interact with bots conversationally within a chat experience.

[Hangouts Chat bot - Apps Script](https://www.qwiklabs.com/focuses/2165?catalog_rank=%7B%22rank%22%3A8%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&parent=catalog&search_id=7482904)


#### Big Data Analysis

This lab covers Google Cloud's [BigQuery](http://cloud.google.com/bigquery) API (as an Apps Script [advanced service](https://developers.google.com/apps-script/guides/services/advanced)) and the [built-in Apps Script services](https://developers.google.com/apps-script/guides/services) for [Google Sheets](http://gsuite.google.com/products/sheets) and [Google Slides](http://gsuite.google.com/products/slides).

[Big Data Analysis to a Slide Presentation](https://www.qwiklabs.com/focuses/3565?catalog_rank=%7B%22rank%22%3A9%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&parent=catalog&search_id=7482904)


#### Google Cloud Functions

In this lab, you build and deploy a few Cloud Functions connected to G Suite APIs and other Google Cloud Platform services.

[Empower Your Gmail Inbox with Google Cloud Functions](https://www.qwiklabs.com/focuses/5166?catalog_rank=%7B%22rank%22%3A10%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&parent=catalog&search_id=7482904)


## AppSheet


### Introduction

AppSheet Automation allows line-of-business employees to rapidly automate their critical business processes. The AI-powered solution anticipates your automation requirements, provides intelligent suggestions, and auto-constructs actions based on user intent.

[https://cloud.google.com/appsheet](https://cloud.google.com/appsheet)


### How to create a no-code App

[https://solutions.appsheet.com/how-to-create-an-app](https://solutions.appsheet.com/how-to-create-an-app)


### Sample Apps

[https://www.appsheet.com/SampleApps](https://www.appsheet.com/SampleApps)


### YouTube AppSheet Playlist

[https://www.youtube.com/watch?v=7Tzwu8mY-gI&list=PLZ81nepkT97KAehtQ_Y__bNJX3qZaStvt](https://www.youtube.com/watch?v=7Tzwu8mY-gI&list=PLZ81nepkT97KAehtQ_Y__bNJX3qZaStvt)


## Healthcare and Life Sciences


### Cloud Healthcare API

The Cloud Healthcare API provides industry-standard protocols and formats for ingesting, storing, analyzing, and integrating healthcare data with cloud-based applications.

The API supports the following applications:



*   Healthcare machine learning applications
*   Data-level integration of healthcare systems
*   Secure storage and retrieval of healthcare and life science data, including electronic protected health information (ePHI) and other forms of PII

For many applications, the Cloud Healthcare API can provide a cloud-based alternative to on-premises stacks implementing the following standards:



*   Digital Imaging and Communications in Medicine (DICOM)
*   Fast Healthcare Interoperability Resources (FHIR) DSTU2, STU3, and R4 standards
*   Health Level Seven Version 2.x (HL7v2)

The Cloud Healthcare API simplifies data integration with existing systems and allows developers to focus on differentiating features, such as UX and intelligence.

[https://cloud.google.com/healthcare/docs](https://cloud.google.com/healthcare/docs)

There is no shortage of opportunities for clinical decision support and cognitive assistance in healthcare. 

[https://www.youtube.com/watch?v=DH-JC9DfYdI](https://www.youtube.com/watch?v=DH-JC9DfYdI)


### Cloud Life Sciences

Cloud Life Sciences is a suite of services and tools for managing, processing, and transforming life sciences data. It also enables advanced insights and operational workflows using highly scalable and compliant infrastructure. Cloud Life Sciences includes features such as the Cloud Life Sciences API and extract-transform-load (ETL) tools, and more.

[https://cloud.google.com/life-sciences/docs](https://cloud.google.com/life-sciences/docs)


### Qwiklabs


#### ML Predictions

In this lab, you will create a prediction pipeline for FHIR resources using Cloud Healthcare API and AI Platform.

[Machine Learning Predictions with FHIR and Healthcare API](https://www.qwiklabs.com/focuses/6129?catalog_rank=%7B%22rank%22%3A18%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&parent=catalog&search_id=7468017)


## IoT


### Introduction

Learn how to create a Cloud IoT Core device registry and register a device. Try the Internet of Things: Qwik Start lab here:[ https://goo.gl/Wzgvaq](https://www.youtube.com/redirect?q=https%3A%2F%2Fgoo.gl%2FWzgvaq&redir_token=QUFFLUhqbU40UE5wbXFUUEtiSDRHT2hfY1dWbXIwdENXd3xBQ3Jtc0tueTJmREotMno2SHdtSi1xUVRJVGliZ21XNFRzd3VDWXppTWxxT1ZIcS0zc2NoZnBBZzJKWkx0akZybDRHTlg4cWF3T1RlWWN1OGQ5WWEtdVhCdjRVZ2FfME4zdXQ5ZFF0QnhHY0o3a2xfdmF6NUVwRQ%3D%3D&v=iRZzqpvARbc&event=video_description)

[https://www.youtube.com/watch?v=iRZzqpvARbc](https://www.youtube.com/watch?v=iRZzqpvARbc)


### IoT Core

Google Cloud Internet of Things (IoT) Core is a fully managed service for securely connecting and managing IoT devices, from a few to millions. Ingest data from connected devices and build rich applications that integrate with the other big data services of Google Cloud Platform.

[https://cloud.google.com/iot/docs](https://cloud.google.com/iot/docs)

Events of interest fire off continuously in the physical world, and data that is material to decision making can’t always wait for offline analysis. Internet-equipped sensors on any physical item imaginable make it possible to ingest data continuously into the cloud, directly from the source at massive scale. Learn why Cloud Platform is the best place to build IoT initiatives, taking advantage of Google’s heritage of web-scale processing, analytics, and machine intelligence.

[https://www.youtube.com/watch?v=51bq_Yhuof4](https://www.youtube.com/watch?v=51bq_Yhuof4)


### Qwiklabs


#### IoT in GCP

In this quest, you will learn about Google Cloud’s IoT Core service and its integration with other services like GCS, Dataprep, Stackdriver and Firestore. The labs in this quest use simulator code to mimic IOT devices and the learning here should empower you to implement the same streaming pipeline with real world IoT devices.

[IoT in the Google Cloud](https://www.qwiklabs.com/quests/49?catalog_rank=%7B%22rank%22%3A1%2C%22num_filters%22%3A1%2C%22has_search%22%3Atrue%7D&search_id=7467733)


#### Cloud Logging IoT

In this hands-on lab you will learn how to configure Cloud Functions to send IoT Core device application logs to Cloud Logging.

[Using Cloud Logging with IoT Core Devices](https://www.qwiklabs.com/focuses/2768?catalog_rank=%7B%22rank%22%3A18%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&parent=catalog&search_id=7468061)


## DevOps


### Introduction

Obtain a [competitive advantage](https://hbr.org/sponsored/2019/01/competitive-advantage-through-devops) through DevOps. [DevOps](https://cloud.google.com/devops/) is an organizational and cultural movement that aims to increase software delivery velocity, improve service reliability, and build shared ownership among software stakeholders. In this quest you will learn how to use Google Cloud to improve the speed, stability, availability, and security of your software delivery capability. [DevOps Research and Assessment](https://devops-research.com/) has joined Google Cloud. How does your team measure up? [Take this five multiple-choice question quiz](https://beta.devops-research.com/quickcheck.html) and find out! 

[DevOps Essentials](https://www.qwiklabs.com/quests/96?catalog_rank=%7B%22rank%22%3A3%2C%22num_filters%22%3A1%2C%22has_search%22%3Atrue%7D&search_id=7467726)


### Jenkins & GKE

Jenkins is one of the most popular CI systems in the world. It’s flexibility and ecosystem allow it to be used for almost any task.

[https://www.youtube.com/watch?v=IDoRWieTcMc](https://www.youtube.com/watch?v=IDoRWieTcMc)


### Spinnaker

Build a container based CI/CD pipeline leveraging Google Cloud Platform  tools along with open source tool Spinnaker for deployment. 

[https://www.youtube.com/watch?v=DQIu373gSKU](https://www.youtube.com/watch?v=DQIu373gSKU)


### Jib

Build optimized containers for your Java applications.

[https://www.youtube.com/watch?v=p36tv1YWIfU](https://www.youtube.com/watch?v=p36tv1YWIfU)


### Kubernetes CI/CD

This session demonstrates how using the best tools in the Kubernetes ecosystem, such as Jenkins X, Tekton, Docker, Helm, Skaffold, ChartMuseum, Knative, Prow and others can help you create a fully automated setup. 

[https://www.youtube.com/watch?v=jXPn36d5Tog](https://www.youtube.com/watch?v=jXPn36d5Tog)

Kubernetes had become the orchestrator of choice to deploy applications — but what about a developer’s day to day job? Building Kubernetes applications can require spending a lot of time on building containers, deploying them, and waiting to see changes. Developing applications on Kubernetes doesn’t have to be difficult, and this talk will show you how to leverage local development tools like Skaffold and Google Cloud Build to develop at 10x velocity. We’ll cover how Skaffold intelligently rebuilds and redeploys your application on every code change, all from the comfort of your favorite IDE. We’ll then go over how to use Skaffold and Google Cloud Build to easily deploy a robust CI/CD pipeline from GitHub to GKE, simplifying your local development experience from start to finish.

[https://www.youtube.com/watch?v=TYx0BTyFtmc](https://www.youtube.com/watch?v=TYx0BTyFtmc)


#### Security


##### StackRox

[https://www.stackrox.com/post/2020/11/stackrox-integrates-with-google-artifact-registry/](https://www.stackrox.com/post/2020/11/stackrox-integrates-with-google-artifact-registry/)


##### Binary Authorization Attestations with Voucher

[https://cloud.google.com/binary-authorization/docs/creating-attestations-voucher](https://cloud.google.com/binary-authorization/docs/creating-attestations-voucher)


### GitOps 

GitOps is a way to do application delivery. It works by using [Git](https://git-scm.com/) as a single source of truth for [declarative infrastructure and applications](https://en.wikipedia.org/wiki/Infrastructure_as_code), together with tools ensuring the _actual state_ of infrastructure and applications converges towards the _desired state_ declared in Git. With Git at the center of your delivery pipelines, developers can make pull requests to accelerate and simplify application deployments and operations tasks to your infrastructure or container-orchestration system (e.g. [Kubernetes](https://kubernetes.io/)).

[https://github.com/weaveworks/awesome-gitops](https://github.com/weaveworks/awesome-gitops)


#### Tutorial

This tutorial explains how to manage infrastructure as code with [Terraform](https://cloud.google.com/docs/terraform) and [Cloud Build](https://cloud.google.com/cloud-build) using the popular [GitOps](https://thenewstack.io/what-is-gitops-and-why-it-might-be-the-next-big-thing-for-devops/) methodology. The term GitOps was [first coined by Weaveworks](https://www.weave.works/blog/gitops-operations-by-pull-request), and its key concept is using a Git repository to store the environment state that you want. Terraform is a [HashiCorp](https://www.hashicorp.com/) open source tool that enables you to predictably create, change, and improve your cloud infrastructure by using code. In this tutorial, you use [Cloud Build](https://cloud.google.com/cloud-build), a Google Cloud continuous integration service, to automatically apply Terraform manifests to your environment.

[https://cloud.google.com/solutions/managing-infrastructure-as-code](https://cloud.google.com/solutions/managing-infrastructure-as-code)


#### Gitlab Gitops with Anthos

[https://www.youtube.com/watch?v=npc08ggdTOw](https://www.youtube.com/watch?v=npc08ggdTOw)


### ArgoCD

[https://www.youtube.com/watch?v=35Qimb_AZ8U](https://www.youtube.com/watch?v=35Qimb_AZ8U)


### Chaos Monkey

[https://netflix.github.io/chaosmonkey/](https://netflix.github.io/chaosmonkey/)


## Development, API & SDK


### Introduction

Google Cloud Application Programming Interfaces are the mechanism to interact with Google Cloud Services programmatically. 


### Cloud Endpoints

Endpoints is an API management system that helps you secure, monitor, analyze, and set quotas on your APIs using the same infrastructure Google uses for its own APIs. After you deploy your API to Endpoints, you can use the [Cloud Endpoints Portal](https://cloud.google.com/endpoints/docs/dev-portal-overview) to create a developer portal, a website that users of your API can access to view documentation and interact with your API.

[https://cloud.google.com/endpoints/docs](https://cloud.google.com/endpoints/docs)

Use Cloud Endpoints to deploy, test and  manage your API’s.

[https://www.youtube.com/watch?v=AgYImGHmvBA](https://www.youtube.com/watch?v=AgYImGHmvBA)


### Cloud API

Google Cloud APIs are a key part of Google Cloud Platform, allowing you to easily add the power of everything from storage access to machine-learning-based image analysis to your Cloud Platform applications.

[https://cloud.google.com/apis/docs/overview](https://cloud.google.com/apis/docs/overview)


### Artifact Registry

A universal package manager for all your build artifacts and dependencies. Fast, scalable, reliable and secure.

[https://cloud.google.com/artifacts/docs](https://cloud.google.com/artifacts/docs)

Container Registry has evolved into Artifact Registry - a platform that allows you to seamlessly manage container images, integrate with Cloud Build and third-party CI/CD systems. 

[https://www.youtube.com/watch?v=712Y0KpeHok](https://www.youtube.com/watch?v=712Y0KpeHok)


### Container Registry

Container Registry provides secure, private Docker image storage on Google Cloud Platform.

[https://cloud.google.com/container-registry/docs](https://cloud.google.com/container-registry/docs)


### Cloud Source Repositories

Cloud Source Repositories are fully featured, private [Git](https://git-scm.com/) repositories hosted on Google Cloud.

[https://cloud.google.com/source-repositories/docs](https://cloud.google.com/source-repositories/docs)


### Cloud Deployment Manager


#### Introduction

Google Cloud Deployment Manager is an infrastructure deployment service that automates the creation and management of Google Cloud resources. Write flexible template and configuration files and use them to create deployments that have a variety of Google Cloud services, such as Cloud Storage, Compute Engine, and Cloud SQL, configured to work together.

[https://cloud.google.com/deployment-manager/docs](https://cloud.google.com/deployment-manager/docs)


#### Tutorial

In this tutorial, you deploy an example logbook app that uses Node.js for its frontend and MySQL for its backend. 

[https://cloud.google.com/deployment-manager/docs/create-advanced-deployment](https://cloud.google.com/deployment-manager/docs/create-advanced-deployment)


### Codelabs

Google Developers Codelabs provide a guided, tutorial, hands-on coding experience. Most codelabs will step you through the process of building a small application, or adding a new feature to an existing application. They cover a wide range of topics such as Android Wear, Google Compute Engine, Project Tango, and Google APIs on iOS.

[https://codelabs.developers.google.com/](https://codelabs.developers.google.com/)


### Colab

Colaboratory, or "Colab" for short, allows you to write and execute Python in your browser.

Colab allows you to not only execute Jupyter Notebooks on the web, but also offers a free GPU, excellent collaboration features, built-in code snippets, and more.

[https://colab.research.google.com/](https://colab.research.google.com/)

A demo of Colab.

[https://www.youtube.com/watch?v=yEIc9z-Ad3k](https://www.youtube.com/watch?v=yEIc9z-Ad3k)


### Cloud Scheduler

Cloud Scheduler is a fully managed enterprise-grade cron job scheduler. It allows you to schedule virtually any job, including batch, big data jobs, cloud infrastructure operations, and more. You can automate everything, including retries in case of failure to reduce manual toil and intervention. Cloud Scheduler even acts as a single pane of glass, allowing you to manage all your automation tasks from one place.

[https://cloud.google.com/scheduler/docs/quickstart](https://cloud.google.com/scheduler/docs/quickstart)

Use Cloud Scheduler to run python scripts in the cloud periodically like cron jobs.

[https://www.youtube.com/watch?v=7Z1mgOxWTs8](https://www.youtube.com/watch?v=7Z1mgOxWTs8)


### Cloud Tasks

Cloud Tasks is a fully managed service that allows you to manage the execution, dispatch and delivery of a large number of distributed tasks. You can asynchronously perform work outside of a user request. Your tasks can be executed on App Engine or any arbitrary HTTP endpoint.

[https://cloud.google.com/tasks/docs](https://cloud.google.com/tasks/docs)

Understanding Cloud Tasks for Async Tasks.

Queues for background tasks.

[https://www.youtube.com/watch?v=Q_airdHCuV8](https://www.youtube.com/watch?v=Q_airdHCuV8)


### Cloud Code

Cloud Code provides IDE support for the full development cycle of Kubernetes and Cloud Run applications, from creating and customizing a new application from sample templates to running your finished application. Cloud Code also supports you along the way with run-ready samples, out-of-the-box configuration snippets, and a tailored debugging experience — making developing with Kubernetes and Cloud Run a whole lot easier!

[https://cloud.google.com/code/docs](https://cloud.google.com/code/docs)

Cloud Code provides an end-to-end workflow for developing, debugging, and deploying Cloud Run applications from within IDEs such as Visual Studio Code and IntelliJ. 

[https://www.youtube.com/watch?v=bOWsRGGO5xk](https://www.youtube.com/watch?v=bOWsRGGO5xk)

Using Cloud Code with Kubernetes.

[https://www.youtube.com/watch?v=KNd0mTxcQ_M](https://www.youtube.com/watch?v=KNd0mTxcQ_M)


### Cloud Build

Cloud Build is a service that executes your builds on Google Cloud Platform infrastructure. Cloud Build can import source code from Google Cloud Storage, Cloud Source Repositories, GitHub, or Bitbucket, execute a build to your specifications, and produce artifacts such as Docker containers or Java archives.

[https://cloud.google.com/cloud-build/docs](https://cloud.google.com/cloud-build/docs)

Google Cloud Build helps you create fast, consistent, and reliable workflows. 

[https://www.youtube.com/watch?v=w7dMHiEyGAs](https://www.youtube.com/watch?v=w7dMHiEyGAs)

A list of URLs related to Cloud Build.

[https://github.com/Timtech4u/awesome-cloudbuild](https://github.com/Timtech4u/awesome-cloudbuild)


### Qwiklabs


#### Exploring APIs

This quest will give you hands-on practice with a variety of GCP APIs, which you will learn through working with Google’s APIs Explorer, a tool that allows you to browse APIs and run their methods interactively. By learning how to transfer data between Cloud Storage buckets, deploy Compute Engine instances, configure Dataproc clusters and much more, Exploring APIs will show you how powerful APIs are and why they are used almost exclusively by proficient GCP users. Enroll in this quest today.

[Exploring APIs](https://www.qwiklabs.com/quests/54?catalog_rank=%7B%22rank%22%3A10%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&search_id=7467936)


#### App Engine API Explorer

[App Engine](https://cloud.google.com/appengine/) lets you deploy applications on a fully managed platform. You can scale your applications seamlessly without having to worry about managing the underlying infrastructure. With zero server management and zero configuration deployments, developers can focus only on building great applications without the management overhead.

In this lab you will deploy a simple hello world application to App Engine and make updates to its configuration using the App Engine Admin API through the APIs Explorer tool.

[APIs Explorer: App Engine](https://www.qwiklabs.com/focuses/3662?catalog_rank=%7B%22rank%22%3A16%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&parent=catalog&search_id=7467964)


## API Management, Apigee

Apigee is a Full-LifeCycle API Management tool.

[https://www.youtube.com/watch?v=-okdOGsitm8](https://www.youtube.com/watch?v=-okdOGsitm8)


### Apigee API Platform

With Apigee, you can build API proxies—RESTful, HTTP-based APIs that interact with your services. With easy-to-use APIs, developers can be more productive, increasing your speed to market.

[https://docs.apigee.com/](https://docs.apigee.com/)


### Apigee Developer Portal

Using the Drupal portal development tools, you can build a fully customizable developer portal. Drupal provides a rich set of functionality and all the CMS capabilities of Drupal with additional Apigee-developed Drupal modules. However, implementing a Drupal-based portal requires more time and effort.

[https://docs.apigee.com/api-platform/publish/developer-portal#integrated-portal](https://docs.apigee.com/api-platform/publish/developer-portal#integrated-portal)


### Apigee Sense

Apigee Sense protects your APIs from unwanted request traffic, including attacks from malicious clients. Apigee Sense analyzes API request traffic, identifying patterns that might represent unwanted requests.

[https://docs.apigee.com/sense/what-apigee-sense](https://docs.apigee.com/sense/what-apigee-sense)


### Apigee API Analytics

Edge API Analytics collects and calculates a wealth of information that flows through API proxies. You can visualize this data with graphs and charts in the Edge UI, or you can download the raw data for offline analysis using the Edge management APIs.

[https://docs.apigee.com/api-platform/analytics/analytics-services-overview](https://docs.apigee.com/api-platform/analytics/analytics-services-overview)


### Apigee API Monetization

As an API provider, you need an easy-to-use and flexible way to monetize your APIs so that you can generate revenue for the use of your APIs. Using monetization in Apigee Edge, you can create a variety of monetization plans that charge developers (or pay them through revenue sharing) for the use of your APIs.

[https://docs.apigee.com/api-platform/monetization/basics-monetization/](https://docs.apigee.com/api-platform/monetization/basics-monetization/)


### Apigee Hybrid

Apigee hybrid is a platform for developing and managing API proxies that features a hybrid deployment model. The hybrid model includes a management plane hosted by Apigee in the Cloud and a runtime plane that you install and manage on one of the [supported Kubernetes platforms](https://cloud.google.com/apigee/docs/hybrid/v1.3/install-before-begin#supported-platforms).

[https://docs.apigee.com/hybrid/what-is-hybrid](https://docs.apigee.com/hybrid/what-is-hybrid)


## Comparisons


### AWS vs. GCP 

Compare Google Cloud with AWS and highlight the similarities and differences between the two. 

[https://cloud.google.com/docs/compare/aws](https://cloud.google.com/docs/compare/aws) 


### DevOps vs. SRE

A video discussing differences and similarities between DevOps and SRE.

[https://www.youtube.com/watch?v=uTEL8Ff1Zvk](https://www.youtube.com/watch?v=uTEL8Ff1Zvk)

Some books on SRE from google.

[https://landing.google.com/sre/books/](https://landing.google.com/sre/books/)


## Accounts & Billing


### Concepts


#### Important Roles

[https://cloud.google.com/billing/docs/concepts#important_roles](https://cloud.google.com/billing/docs/concepts#important_roles)


#### Resource Hierarchy

[https://cloud.google.com/resource-manager/docs/cloud-platform-resource-hierarchy#resource-hierarchy-detail](https://cloud.google.com/resource-manager/docs/cloud-platform-resource-hierarchy#resource-hierarchy-detail)


#### Projects, Folders, Labels

[https://cloud.google.com/billing/docs/onboarding-checklist#projects-folders-labels](https://cloud.google.com/billing/docs/onboarding-checklist#projects-folders-labels)


#### Relationships between Resources

Relationships between organizations, projects, Cloud Billing accounts, and payments profiles

[https://cloud.google.com/billing/docs/concepts#relationships-between-resources](https://cloud.google.com/billing/docs/concepts#relationships-between-resources)


### Organizations

[https://cloud.google.com/resource-manager/docs/creating-managing-organization](https://cloud.google.com/resource-manager/docs/creating-managing-organization)


### Accounts

[https://cloud.google.com/billing/docs/how-to/manage-billing-account](https://cloud.google.com/billing/docs/how-to/manage-billing-account)


### Folders

[https://cloud.google.com/resource-manager/docs/creating-managing-folders](https://cloud.google.com/resource-manager/docs/creating-managing-folders)


### Billing Account & Payment Profile

[https://cloud.google.com/billing/docs/concepts#billing_account](https://cloud.google.com/billing/docs/concepts#billing_account)


### GCP Cloud Customer Onboarding Checklist

Google Cloud customers can be assisted in setting up their various Google Cloud resources to avoid common issues and enable best practices for access control and cost management. There are some design decisions and configuration options that help set you up for success in administering your cloud resources.

[https://cloud.google.com/billing/docs/onboarding-checklist](https://cloud.google.com/billing/docs/onboarding-checklist)


### Key Decisions

[https://cloud.google.com/billing/docs/onboarding-checklist#cloud-billing-accounts](https://cloud.google.com/billing/docs/onboarding-checklist#cloud-billing-accounts)


### Google Cloud Pricing Calculator

[https://cloud.google.com/products/calculator](https://cloud.google.com/products/calculator)

Managing GCP usage and cost trends is easier than you think. In this session, we'll show you how to quickly view your GCP costs, forecast your month-end bill, and provide an overview of some of the controls you can put in place to prevent budget overruns.

[https://www.youtube.com/watch?v=UocD6uY2-js](https://www.youtube.com/watch?v=UocD6uY2-js)


### Qwiklabs


#### Optimizing GCP Costs

Here you'll learn several ways to control and optimize your GCP costs, including setting up budgets and alerts, managing quota limits, and taking advantage of committed use discounts. In the hands-on labs, you’ll practice using various tools to control and optimize your GCP costs or to influence your technology teams to apply the cost optimization best practices.

[Optimizing Your GCP Costs](https://www.qwiklabs.com/quests/97?catalog_rank=%7B%22rank%22%3A4%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&search_id=7468028)


## Compliance

[GCP Compliance Offerings](https://cloud.google.com/security/compliance/offerings/#/)

[PCI Responsibility Matrix ](https://cloud.google.com/files/PCI_DSS_Shared_Responsibility_GCP_v32.pdf)

[GCP Security Controls](https://cloud.google.com/security/)

[Vault EaaS - Encryption As a Service](https://learn.hashicorp.com/tutorials/vault/eaas-transit)
