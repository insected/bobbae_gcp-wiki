

## Networking

https://www.guru99.com/data-communication-computer-network-tutorial.html

### Introduction

Google Cloud Platform includes software-defined networking, hybrid connectivity, network performance optimization, network security, service mesh deployment, NAT, load balancing, and routing.

[https://developers.google.com/learn/topics/networking](https://developers.google.com/learn/topics/networking)

Google Cloud Platform has recently added new regions in Seoul, Salt Lake City, Las Vegas and Jakarta. GCP implements software-defined network that provides fast and reliable connections to users around the world.

[https://cloud.google.com/about/locations](https://cloud.google.com/about/locations)


Google spent $30 billion improving the infrastructure over the years. From data centers to subsea cables, GCP connects customers in different regions around the world.

[https://www.blog.google/products/google-cloud/expanding-our-global-infrastructure-new-regions-and-subsea-cables/](https://www.blog.google/products/google-cloud/expanding-our-global-infrastructure-new-regions-and-subsea-cables/)

<img src="https://storage.googleapis.com/gweb-uniblog-publish-prod/images/infrastructure-3.max-1000x1000.png" width="700">

In a traditional data center, you manage a complex network setup composed of racks of servers, storage devices, multiple layers of switches, routers, load balancers, firewall devices, and more. In addition to these hardware components, you must set up, maintain, and monitor the network's underlying software, as well as detailed device configurations for your environment. And the managerial overhead doesn't end there: you also have to worry about the security and availability of your network, and you must plan out the upgrades and expansions of your network—a lengthy and time-consuming process.

https://cloud.google.com/docs/compare/data-centers/networking

Google built a superior cloud network as a result of the well-provisioned direct paths between its cloud and end-users.

<img src="https://storage.googleapis.com/gweb-uniblog-publish-prod/images/infrastructure-1.max-1000x1000.png" width="500">


#### Networking 101

[https://www.youtube.com/watch?v=0hN-dyOV10c](https://www.youtube.com/watch?v=0hN-dyOV10c)

#### CompTIA Network+ full course

https://www.youtube.com/watch?v=qiQR5rTSshw&list=RDCMUC8butISFwT-Wl7EV0hUK0BQ

#### Networking End to End

[https://www.youtube.com/playlist?list=PLIivdWyY5sqJ0oXcnZYqOnuNRsLF9H48u](https://www.youtube.com/playlist?list=PLIivdWyY5sqJ0oXcnZYqOnuNRsLF9H48u)


#### Two Tier vs. Three Tier Architecture

[https://www.wwt.com/article/comparing-two-tier-three-tier-data-center-networks](https://www.wwt.com/article/comparing-two-tier-three-tier-data-center-networks)


#### Jupiter 

[Jupiter](https://cloud.google.com/blog/products/networking/google-cloud-networking-in-depth-series-digest)  fabrics can deliver more than 1 Petabit/sec of total bisection bandwidth. To put this in perspective, such capacity would be enough for 100,000 servers to exchange information at 10Gb/s each, enough to read the entire scanned contents of the Library of Congress in less than 1/10th of a second.

[https://cloudplatform.googleblog.com/2015/06/A-Look-Inside-Googles-Data-Center-Networks.html](https://cloudplatform.googleblog.com/2015/06/A-Look-Inside-Googles-Data-Center-Networks.html?m=1)


### Network Options

[Network Options](Network-Options)


#### Introduction

Cloud [CDN](https://en.wikipedia.org/wiki/Content_delivery_network) (Content Delivery Network) uses Google's globally distributed edge points of presence to cache external HTTP(S) load balanced content close to your users. Caching content at the edges of Google's network provides faster delivery of content to your users while reducing serving costs. 

There are [DNS](DNS) based CDNs.

The CDN provider typically determines the optimal server selection based on the source IP address of the DNS request (probably combined with other information). However, the source IP address conveyed to the CDN provider is that of the DNS recursive server, rather than that of the client.

[https://cloud.google.com/cdn/docs](https://cloud.google.com/cdn/docs)


#### Using CDN and Load Balancing

[https://www.youtube.com/watch?v=NedNhOg_TgA](https://www.youtube.com/watch?v=NedNhOg_TgA)


#### Setting up Cloud CDN with backend storage bucket

[https://cloud.google.com/cdn/docs/setting-up-cdn-with-bucket](https://cloud.google.com/cdn/docs/setting-up-cdn-with-bucket)


### Hybrid Connectivity

[https://cloud.google.com/hybrid-connectivity](https://cloud.google.com/hybrid-connectivity)


### Cloud Interconnect

[Interconnect](Interconnect) extends your on-premises network to Google's network through a highly available, low latency connection. 





### Cloud Load Balancing

[Load Balancer](Load-Balancer) distributes user traffic across multiple instances of your applications. By spreading the load, load balancing reduces the risk that your applications experience performance issues.

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

[VPC](VPC) Flow Logs records a sample of network flows sent from and received by VM instances, including instances used as GKE nodes. These logs can be used for network monitoring, forensics, real-time security analysis, and expense optimization.

[https://cloud.google.com/vpc/docs/using-flow-logs](https://cloud.google.com/vpc/docs/using-flow-logs)

Network and security telemetry is fundamental to operate your deployments in public clouds with confidence, providing the required visibility on the behavior of your network and Access control firewalls. 

[https://www.youtube.com/watch?v=as9mXNEcaDo](https://www.youtube.com/watch?v=as9mXNEcaDo)


### Traffic Director


[Traffic Director](Traffic-Director)  is GCP's fully managed traffic control plane for service mesh. With Traffic Director, you can easily deploy global load balancing across clusters and VM instances in multiple regions, offload health checking from service proxies, and configure sophisticated traffic control policies.


### Service Directory

Service Directory helps reduce the complexity of management and operations by providing a single place to publish, discover, and connect services. It is a managed service that enhances service inventory management at scale so you don’t have to. Service Directory provides real-time service information, whether you have a few service endpoints or thousands. 

[https://cloud.google.com/service-directory](https://cloud.google.com/service-directory)

[https://www.youtube.com/watch?v=H9UoE_cWIEY](https://www.youtube.com/watch?v=H9UoE_cWIEY)


### Qwiklabs


#### Networking

Networking is a principle theme of cloud computing. It’s the underlying structure of Google Cloud, and it’s what connects all your resources and services to one another. This fundamental-level quest will cover essential Google Cloud networking services and will give you hands-on practice with specialized tools for developing mature networks. 

[Networking in the Google Cloud](https://www.qwiklabs.com/quests/31?catalog_rank=%7B%22rank%22%3A4%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&search_id=7467791)


#### Secure Networks

[Build and Secure Networks in Google Cloud](https://www.qwiklabs.com/quests/128?catalog_rank=%7B%22rank%22%3A1%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&search_id=7467791)


#### Network Performance

This quest is composed of labs that cover real-life use cases and it will teach you best practices for overcoming common networking bottlenecks. From getting hands-on practice with testing and improving network performance, to integrating high-throughput [VPNs](VPN) and networking tiers, Network Performance and Optimization is an essential quest for GCP developers who are looking to double down on application speed and robustness.


[Network Performance and Optimization](https://www.qwiklabs.com/quests/46?catalog_rank=%7B%22rank%22%3A2%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&search_id=7467791)


#### [VPC](VPC) Networking Fundamentals

Google Cloud Virtual Private Cloud (VPC) provides networking functionality to Compute Engine virtual machine (VM) instances, Kubernetes Engine containers and App Engine Flex. In other words, without a VPC network you cannot create VM instances, containers or App Engine applications. Therefore, each Google Cloud project has a default network to get you started.

You can think of a [VPC](VPC) network the same way you would think of a physical network, except that it is virtualized within Google Cloud. A VPC network is a global resource which consists of a list of regional virtual subnetworks (subnets) in data centers, all connected by a global wide area network (WAN). VPC networks are logically isolated from each other in Google Cloud.

[VPC Networking Fundamentals](https://www.qwiklabs.com/focuses/1229?catalog_rank=%7B%22rank%22%3A11%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&parent=catalog&search_id=7467802)


#### VPC Network Peering

VPC Network [Peering](Peering) allows you to build SaaS (Software-as-a-Service) ecosystems in Google Cloud, making services available privately across different VPC networks within and across organizations, allowing workloads to communicate in private space.

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

In this lab, you configure Cloud [Routers](Router) using the Console. The Cloud Routers will implement VPN gateways configured with BGP. BGP provides dynamic network discovery and eliminates the need to configure or maintain static routes. When successful you will be able to ping the internal IP of the VM in a newly discovered subnetwork via an auto-populated route.

[Dynamic VPN Gateways - Cloud Routers ](https://www.qwiklabs.com/focuses/1233?parent=catalog)


#### Service Directory

Service Directory provides real-time service information, whether you have a few service endpoints or thousands. This helps ensure that your applications only resolve the most updated information of their resources, increasing the reachability of your services. With Service Directory, you can easily understand all your services across multi-cloud environments. This includes workloads running in Compute Engine VMs, Google Kubernetes Engine (GKE), as well as external services running on-prem and third-party clouds. It improves application reachability by maintaining the endpoint information for all your services.

[Service Directory: Qwik Start](https://www.qwiklabs.com/focuses/12412?catalog_rank=%7B%22rank%22%3A19%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&parent=catalog&search_id=7468061)

