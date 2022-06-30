
https://en.wikipedia.org/wiki/Computer_network

Data Communication and [Computer Networking]( https://www.guru99.com/data-communication-computer-network-tutorial.html  ) provides the rules and regulations that allow computers with different operating systems, languages, cabling, and locations to share resources and communicate with each other. 

https://book.systemsapproach.org/index.html

## Introduction

Google Cloud Platform includes [software-defined networking](https://developers.google.com/learn/topics/networking), hybrid connectivity, network performance optimization, [network security](Security), [service mesh](Service-Mesh) deployment, [NAT](Cloud-NAT), [load balancing](Load-Balancer), and [routing](Router).



GCP implements [software-defined network](  https://cloud.google.com/blog/products/networking/google-cloud-networking-in-depth-how-andromeda-2-2-enables-high-throughput-vms ) that provides [fast and reliable connections](  https://cloud.google.com/blog/products/networking/google-cloud-networking-in-depth-series-digest ) to users [around the world](https://cloud.google.com/about/locations).

Google Cloud customers enjoy significantly improved intra-zone network latency with the [Andromeda  software-defined network]( https://cloud.google.com/blog/products/gcp/andromeda-2-1-reduces-gcps-intra-zone-latency-by-40-percent  ) (SDN) stack that underpins all of Google Cloud.   [Snap](https://research.google/pubs/pub48630/) is a userspace networking system that supports Google’s rapidly evolving needs with flexible modules that implement a range of network functions, including edge packet switching, virtualization for our cloud platform, traffic shaping policy enforcement, and a high-performance reliable messaging and RDMA-like service. 



Google's own [Jupiter network fabrics](  https://research.google/pubs/pub43837/ )   can deliver more than 1 Petabit/sec of total bisection bandwidth. To put this in perspective, such [capacity](https://cloudplatform.googleblog.com/2015/06/A-Look-Inside-Googles-Data-Center-Networks.html?m=1) would be enough for 100,000 servers to exchange information at 10Gb/s each, enough to read the entire scanned contents of the Library of Congress in less than 1/10th of a second.

From data centers to subsea cables, GCP connects customers in [different regions](https://www.blog.google/products/google-cloud/expanding-our-global-infrastructure-new-regions-and-subsea-cables/) around the world.

https://cloud.google.com/blog/products/infrastructure/googles-dunant-subsea-cable-is-now-ready-for-service

<!--
<img src="https://storage.googleapis.com/gweb-uniblog-publish-prod/images/infrastructure-3.max-1000x1000.png" width="700">

Google built a superior [cloud network](https://cloud.google.com/docs/compare/data-centers/networking) as a result of the well-provisioned direct paths between its cloud and end-users.

<img src="https://storage.googleapis.com/gweb-uniblog-publish-prod/images/infrastructure-1.max-1000x1000.png" width="500">
-->

https://cloud.google.com/blog/topics/developers-practitioners/googles-subsea-fiber-optics-explained

https://youtu.be/KayF1osXrOk


https://cloud.google.com/blog/products/infrastructure/google-network-infrastructure-investments

## GCP Network stack
https://cloud.google.com/blog/products/networking/networking-spotlight-2022

## GCP networking 101
https://github.com/jesuispy/networking-101-gcp-sheet

## GCP Network Options


GCP provides various [Network Service Options](Network-Options).

## GCP Network Analyzer

https://cloud.google.com/network-intelligence-center/docs/network-analyzer/overview

## GCP IP and DNS

### IP Addresses

https://cloud.google.com/compute/docs/ip-addresses

https://cloud.google.com/blog/topics/developers-practitioners/ip-addressing-options-google-cloud-networking-basics

### Internal DNS

https://cloud.google.com/compute/docs/internal-dns

## General Networking 101

[https://www.youtube.com/watch?v=0hN-dyOV10c](https://www.youtube.com/watch?v=0hN-dyOV10c)

### OSI Model

The [Open Systems Interconnection model]( https://en.wikipedia.org/wiki/OSI_model  ) (OSI model) is a [conceptual model]( https://www.freecodecamp.org/news/osi-model-computer-networking-for-beginners/  ) that characterises and standardises the communication functions of a telecommunication or computing system without regard to its underlying internal structure and technology. 


Recommendation X.200 describes seven layers, labelled 1 to 7.





### TCP/IP

The [Internet protocol suite]( https://en.wikipedia.org/wiki/Internet_protocol_suite  ), commonly known as TCP/IP, is the set of communications protocols used in the Internet and similar computer networks. The current foundational protocols in the suite are the Transmission Control Protocol (TCP) and the Internet Protocol (IP).




### Protocol Wars

https://wikipedia.org/wiki/Protocol_Wars

### CIDR

[Classless Inter-Domain Routing](https://en.wikipedia.org/wiki/Classless_Inter-Domain_Routing   ) is a method for allocating IP addresses and for IP routing. The Internet Engineering Task Force introduced CIDR in 1993 to replace the previous classful network addressing architecture on the Internet. Its goal was to slow the growth of routing tables on routers across the Internet, and to help slow the rapid exhaustion of IPv4 addresses.

https://www.digitalocean.com/community/tutorials/understanding-ip-addresses-subnets-and-cidr-notation-for-networking

### Routing

[IP routing](https://en.wikipedia.org/wiki/IP_routing   ) deals with routes of Internet Protocol (IP) packets within and across IP networks. 

https://en.wikipedia.org/wiki/Routing_table


### DNS

The [Domain Name System](DNS) (DNS) is a hierarchical and decentralized naming system for the Internet or a private network. It [translates domain names to the numerical IP addresses]( https://en.wikipedia.org/wiki/Domain_Name_System  ).



### Ethernet

[Ethernet](  https://en.wikipedia.org/wiki/Ethernet ) is a family of wired computer networking technologies commonly used in local area networks (LAN), metropolitan area networks (MAN), and wide area networks (WAN).



### Network Switch

A [network switch]( https://en.wikipedia.org/wiki/Network_switch  ) (also called switching hub, bridging hub, and, by the IEEE, MAC bridge) is networking hardware that connects devices on a computer network by using packet switching to receive and forward data to the destination device.



#### Multi-layer Switch

A [multilayer switch](  https://en.wikipedia.org/wiki/Multilayer_switch ) (MLS) is a computer networking device that switches on OSI layer 2 like an ordinary network switch and provides extra functions on higher OSI layers.




#### Open vSwitch

[Open vSwitch]( https://en.wikipedia.org/wiki/Open_vSwitch   ), sometimes abbreviated as OVS, is an open-source implementation of a distributed virtual multilayer switch. 


#### Open Compute Project Whitebox Switches

https://www.opencompute.org/wiki/Networking/SpecsAndDesigns

### Network Router

A [router]( https://en.wikipedia.org/wiki/Router_(computing)  ) is a networking device that forwards data packets between computer networks. Routers perform the traffic directing functions on the Internet. 


#### Brouter

A [bridge router or brouter](https://en.m.wikipedia.org/wiki/Bridge_router) is a network device that works as a bridge and as a router. 

#### Switch vs Router

https://www.guru99.com/router-vs-switch-difference.html

### Routing Protocols

A [routing protocol](  https://en.wikipedia.org/wiki/Routing_protocol ) specifies how routers communicate with each other to distribute information that enables them to select routes between nodes on a computer network. 



### Subnetwork

A [subnetwork or subnet]( https://en.wikipedia.org/wiki/Subnetwork  ) is a logical subdivision of an IP network. The practice of dividing a network into two or more networks is called subnetting.


## Network Learning Resources

### CompTIA Network+ full course

https://www.youtube.com/watch?v=qiQR5rTSshw&list=RDCMUC8butISFwT-Wl7EV0hUK0BQ

### Networking End to End

[https://www.youtube.com/playlist?list=PLIivdWyY5sqJ0oXcnZYqOnuNRsLF9H48u](https://www.youtube.com/playlist?list=PLIivdWyY5sqJ0oXcnZYqOnuNRsLF9H48u)


### Two-Tier vs. Three Tier Architecture

#### Networking point of view

[https://www.wwt.com/article/comparing-two-tier-three-tier-data-center-networks](https://www.wwt.com/article/comparing-two-tier-three-tier-data-center-networks)

#### Database point of view

https://www.softwaretestingclass.com/what-is-difference-between-two-tier-and-three-tier-architecture/

## Designing your network infrastructure
https://cloud.google.com/architecture/framework/system-design/networking

## Securing your network
https://cloud.google.com/architecture/framework/security/network-security


## Optimizing networking cost
https://cloud.google.com/architecture/framework/cost-optimization/networking

## Network Connectivity Center
https://cloud.google.com/network-connectivity-center

### Site to cloud
https://cloud.google.com/network-connectivity/docs/network-connectivity-center/concepts/site-to-cloud

#### Automatic exchange of routes between on-premises and multiple VPCs

https://cloud.google.com/blog/products/networking/google-cloud-networking-in-depth-simplify-routing-between-your-vpcs-with-vpc-peering

#### Transit network
https://cloud.google.com/vpc/docs/vpc-peering#transit-network

#### Router virtual appliance
https://cloud.google.com/network-connectivity/docs/network-connectivity-center/partners
#### Cloud Router
https://cloud.google.com/network-connectivity/docs/router

### Site to site


https://cloud.google.com/network-connectivity/docs/network-connectivity-center/concepts/data-transfer

#### Voice trading in the cloud
https://cloud.google.com/blog/products/networking/modernizing-private-wires-for-voice-trading-with-the-cloud

### VPC to VPC
https://cloud.google.com/architecture/best-practices-vpc-design#connecting_multiple_networks

#### VPC Peering
https://cloud.google.com/vpc/docs/vpc-peering

#### Hybrid Connectivity
https://cloud.google.com/hybrid-connectivity

#### Firewall policies
https://cloud.google.com/vpc/docs/firewalls

#### Transit VPC
https://cloud.google.com/vpc/docs/vpc-peering#transit-network

#### Firewall topology to connect VPCs together
https://cloud.google.com/network-connectivity/docs/network-connectivity-center/concepts/firewall-topology


## Network Features

### CDN

Cloud [CDN](CDN) (Content Delivery Network) uses Google's globally distributed edge points of presence to cache external HTTP(S) load balanced content close to your users. Caching content at the edges of Google's network provides faster delivery of content to your users while reducing serving costs. 

https://www.sciencedirect.com/science/article/pii/S2352864817300731



### Using CDN and Load Balancing

[https://www.youtube.com/watch?v=NedNhOg_TgA](https://www.youtube.com/watch?v=NedNhOg_TgA)


### Setting up Cloud CDN with backend storage bucket


Cloud CDN leverages Google Cloud global external HTTP(S) load balancers to provide routing, health checking, and Anycast IP support. 

[https://cloud.google.com/cdn/docs/setting-up-cdn-with-bucket](https://cloud.google.com/cdn/docs/setting-up-cdn-with-bucket)

### VPN

[VPN](VPN) extends a private network across a public network and enables users to send and receive data across shared or public networks as if their computing devices were directly connected to the private network.

https://en.wikipedia.org/wiki/Virtual_private_network


#### GCP Cloud VPN

https://cloud.google.com/network-connectivity/docs/vpn/concepts/overview


## VLAN

A [virtual LAN](VLAN) (VLAN) is any broadcast domain that is partitioned and isolated in a computer network at the data link layer (OSI layer 2).

https://cloud.google.com/network-connectivity/docs/interconnect/how-to/dedicated/creating-vlan-attachments

## BGP

[Border Gateway Protocol](BGP) is a standardized exterior gateway protocol designed to exchange routing and reachability information among autonomous systems (AS) on the Internet. BGP is classified as a path-vector routing protocol, and it makes routing decisions based on paths, network policies, or rule sets configured by a network administrator.


https://en.wikipedia.org/wiki/Border_Gateway_Protocol


https://cloud.google.com/network-connectivity/docs/router/how-to/configuring-bgp

### Path vector, Distance vector, Link state and Hybrid

https://cloud.google.com/vpc/docs/routes

https://www.packetcoders.io/routing-protocols-compared-distance-vector-path-vector-link-state-and-hybrid/

https://www.techtarget.com/searchnetworking/definition/split-horizon

https://www.geeksforgeeks.org/difference-between-static-and-dynamic-routing/

## MPLS


Multiprotocol Label Switching (MPLS) is a routing technique in telecommunications networks that directs data from one node to the next based on short path labels rather than long network addresses.

MPLS supports a range of access technologies, including [T1/E1](https://en.wikipedia.org/wiki/Digital_Signal_1), [ATM](https://en.wikipedia.org/wiki/Asynchronous_Transfer_Mode), [Frame Relay](https://en.wikipedia.org/wiki/Frame_Relay), and [DSL](https://en.wikipedia.org/wiki/Digital_subscriber_line).

https://en.wikipedia.org/wiki/Multiprotocol_Label_Switching

https://cloud.google.com/network-connectivity/docs/interconnect/support/faq


### Virtual switches and isolation

https://dl.acm.org/doi/pdf/10.1145/3229616.3229618

https://cloud.google.com/vpc

## Hybrid Connectivity

[https://cloud.google.com/hybrid-connectivity](https://cloud.google.com/hybrid-connectivity)

### Cloud Interconnect

Enterprise-grade connections to your Google VPC via  [interconnect](Interconnect) directly to a Google location with [Dedicated Interconnect](https://cloud.google.com/network-connectivity/docs/interconnect/concepts/dedicated-overview), or flexible bandwidth options with [Partner Interconnect](https://cloud.google.com/network-connectivity/docs/interconnect/concepts/partner-overview).

https://cloud.google.com/network-connectivity/docs/interconnect

https://cloud.google.com/network-connectivity/docs/how-to/choose-product#cloud-interconnect


### Cloud VPN

Connect your on-premises or other public cloud networks to your Google VPC securely over the internet through IPsec VPN.

https://cloud.google.com/network-connectivity/docs/vpn


### Cloud Interconnect

[Interconnect](Interconnect) extends your on-premises network to Google's network through a highly available, low latency connection. 

### Peering with Google

If you can meet Google's requirements, connect directly with Direct Peering, or choose a partner with Carrier Peering.

https://jayendrapatil.com/google-cloud-peering/

#### Direct Peering

Direct Peering enables you to establish a direct peering connection between your business network and Google's edge network and exchange high-throughput cloud traffic.


https://cloud.google.com/network-connectivity/docs/direct-peering

#### Carrier Peering 

Carrier Peering enables you to access Google applications, such as Google Workspace, by using a service provider to obtain enterprise-grade network services that connect your infrastructure to Google.


https://cloud.google.com/network-connectivity/docs/carrier-peering



#### VLAN and Interconnect

https://cloud.google.com/network-connectivity/docs/interconnect/support/faq#interconnect-attachments

#### BGP and MPLS

https://cloud.google.com/network-connectivity/docs/interconnect/support/faq#self-mpls-vpn

## Network Connectivity Center

https://cloud.google.com/network-connectivity/docs/network-connectivity-center/concepts/overview

https://cloud.google.com/blog/products/networking/google-cloud-network-connectivity-center-networking-partnerships

### Hubs
https://cloud.google.com/network-connectivity/docs/network-connectivity-center/concepts/overview#hubs

### Spokes
https://cloud.google.com/network-connectivity/docs/network-connectivity-center/concepts/overview#supported-spoke-resources

## Cloud Load Balancing

[Load Balancer](Load-Balancer) distributes user traffic across multiple instances of your applications. By spreading the load, load balancing reduces the risk that your applications experience performance issues.

### Assembling and managing distributed applications using Google Cloud Networking solutions

https://cloud.google.com/blog/products/networking/networking-spotlight-2022

## Cloud NAT

[Cloud NAT](https://cloud.google.com/nat/docs) provides fully managed, software-defined network address translation support for Google Cloud.



Moving your internal services to the cloud can bring you a handful of new, useful features, but one of the biggest challenges is protecting your internal endpoints. 

[https://www.youtube.com/watch?v=bmaarG0IkH8](https://www.youtube.com/watch?v=bmaarG0IkH8)


## Cloud Armor

Google [Cloud Armor](https://cloud.google.com/armor/docs) helps protect your infrastructure and applications from distributed denial-of-service (DDoS) attacks by using Google's global infrastructure and security systems.



Setting up Cloud Armor.

[https://www.youtube.com/watch?v=g_c2KLpnWck](https://www.youtube.com/watch?v=g_c2KLpnWck)


## Network Intelligence Center

[Network Intelligence Center](https://cloud.google.com/network-intelligence-center/docs) provides a single console for managing Google Cloud network visibility, monitoring, and troubleshooting.

https://cloud.google.com/network-intelligence-center

Getting started with topology in network intelligence center.

[https://www.youtube.com/watch?v=ID7szIL9eew](https://www.youtube.com/watch?v=ID7szIL9eew)

### Firewall Insights

https://cloud.google.com/network-intelligence-center/docs/firewall-insights/concepts/overview






### Enabling NetOps with GCP Network Topology

https://medium.com/google-cloud/enabling-netops-with-gcp-network-topology-39bd49a66a98

## Network Service Tiers


[Network Service Tiers](https://cloud.google.com/network-tiers/) lets you optimize connectivity between systems on the internet and your Google Cloud instances. Premium Tier delivers traffic on Google's premium backbone, while Standard Tier uses regular ISP networks.


[https://www.youtube.com/watch?v=wsdgWGE-mwE](https://www.youtube.com/watch?v=wsdgWGE-mwE)


## Network Telemetry

[VPC](VPC) [Flow Logs](https://cloud.google.com/vpc/docs/using-flow-logs) records a sample of network flows sent from and received by VM instances, including instances used as GKE nodes. These logs can be used for network monitoring, forensics, real-time security analysis, and expense optimization.




[https://www.youtube.com/watch?v=as9mXNEcaDo](https://www.youtube.com/watch?v=as9mXNEcaDo)


## Traffic Director


[Traffic Director](Traffic-Director)  is GCP's fully managed traffic control plane for service mesh. With Traffic Director, you can easily deploy global load balancing across clusters and VM instances in multiple regions, offload health checking from service proxies and configure sophisticated traffic control policies.


## Service Directory

[Service Directory](https://cloud.google.com/service-directory) is a managed service that helps reduce the complexity of management and operations by providing a single place to publish, discover, and connect services. 


[https://www.youtube.com/watch?v=H9UoE_cWIEY](https://www.youtube.com/watch?v=H9UoE_cWIEY)




## Network Security

Network [Security](Security) consists of the policies, processes, and practices adopted to prevent, detect and monitor unauthorized access, misuse, modification, or denial of a computer network and network-accessible resources.

https://en.wikipedia.org/wiki/Network_security

## LAN

A [local area network](https://en.wikipedia.org/wiki/Local_area_network
) (LAN) is a computer network that interconnects computers within a limited area such as a residence, school, laboratory, university campus, or office building. By contrast, a wide area network (WAN) not only covers a larger geographic distance but also generally involves leased telecommunication circuits.

[Ethernet](https://en.wikipedia.org/wiki/Ethernet) and [Wi-Fi](https://en.wikipedia.org/wiki/Wi-Fi) are the two most common technologies in use for local area networks. Other LAN technologies include [ARCNET](https://en.wikipedia.org/wiki/ARCNET), [Token Ring](https://en.wikipedia.org/wiki/Token_Ring), [FDDI](https://en.wikipedia.org/wiki/Fiber_Distributed_Data_Interface) and [AppleTalk](https://en.wikipedia.org/wiki/AppleTalk).


https://en.wikipedia.org/wiki/Local_area_network


## WAN

A [wide area network](https://en.wikipedia.org/wiki/Wide_area_network
) (WAN) is a telecommunications network that extends over a large geographic area for the primary purpose of computer networking. Wide area networks are often established with leased telecommunication circuits.


https://en.wikipedia.org/wiki/Wide_area_network

## NAT

[Network address translation](https://en.wikipedia.org/wiki/Network_address_translation
) (NAT) is a method of mapping an IP address space into another by modifying network address information in the IP header of packets while they are in transit across a traffic routing device. 


https://en.wikipedia.org/wiki/Network_address_translation


## Firewall

A [firewall](https://cloud.google.com/vpc/docs/using-firewalls
) is a network security system that monitors and controls the incoming and outgoing network traffic based on predetermined security rules. 

A firewall rule can contain either IPv4 or IPv6 ranges, but not both.

https://cloud.google.com/vpc/docs/using-firewalls

### Netfilter

https://en.wikipedia.org/wiki/Netfilter


## Underlay network

The Underlay network is closer to the physical layer. It includes switches, routers, VLANs, and so on. It is the basis on which overlay networks are built.

https://networkingnerd.net/tag/underlay-network/

## Overlay network

Overlay network refers to the virtual network layer. It is designed to be highly scalable than the underlying network. For example, while VLANs in the underlying network support only 4096 identifiers, VxLAN can reach up to 16 million ones.


https://book.systemsapproach.org/applications/overlays.html


## Kubernetes CNI

A [CNI](Kubernetes-Networking#cni) is a link between the container runtime (like Docker or rkt) and the network plugin. A CNI is a set of rules and Go libraries that aid in container/network-plugin integration.

All of the CNIs can be deployed by running a pod or a Daemonset that launches and manages their daemons. Let’s have a look now at the most well-known Kubernetes networking solutions.

## Networking Technology 

### IOT Networking

There are [networking technologies for IoT](IoT-Networking)  that allow communications between devices.

### Cellular IoT networks

https://www.iotforall.com/cellular-iot-explained-nb-iot-vs-lte-m

### Time Synchronization 

https://www.masterclock.com/support/library/gps-network-time-synchronization

### NTP

https://wikipedia.org/wiki/Network_Time_Protocol


### PTP

https://wikipedia.org/wiki/Precision_Time_Protocol



### Clock synchronization in distributed systems

https://www.geeksforgeeks.org/synchronization-in-distributed-systems/

### Vector clock

https://wikipedia.org/wiki/Vector_clock

### True time

https://cloud.google.com/spanner/docs/true-time-external-consistency

### Timewarp

https://learnyousomeerlang.com/time

### Plesiochronous

A [plesiochronous system](https://en.wikipedia.org/wiki/Plesiochronous_system) is one where different parts of the system are almost, but not perfectly synchronized. 

### Isochronous Real-time 

https://profinetuniversity.com/profinet-basics/isochronous-real-time-irt-communication/


### TDM

https://en.m.wikipedia.org/wiki/Time-division_multiplexing

### FDM

https://en.m.wikipedia.org/wiki/Frequency-division_multiplexing


### WDM

https://en.m.wikipedia.org/wiki/Wavelength-division_multiplexing

### Statistical Multiplexing 

https://en.m.wikipedia.org/wiki/Statistical_time-division_multiplexing

### TDMA

https://en.m.wikipedia.org/wiki/Time-division_multiple_access


### Packet Switching 

https://en.m.wikipedia.org/wiki/Packet_switching

### Circuit Switching 

https://en.m.wikipedia.org/wiki/Circuit_switching

## NetDevOps

https://github.com/bobbae/gcp/wiki/DevOps#netdevops

## Secure voice trading in the cloud
https://cloud.google.com/blog/products/networking/modernizing-private-wires-for-voice-trading-with-the-cloud

## Qwiklabs


[Networking in the Google Cloud](https://www.qwiklabs.com/quests/31?catalog_rank=%7B%22rank%22%3A4%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&search_id=7467791)


[Build and Secure Networks in Google Cloud](https://www.qwiklabs.com/quests/128?catalog_rank=%7B%22rank%22%3A1%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&search_id=7467791)



[Network Performance and Optimization](https://www.qwiklabs.com/quests/46?catalog_rank=%7B%22rank%22%3A2%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&search_id=7467791)



[VPC Networking Fundamentals](https://www.qwiklabs.com/focuses/1229?catalog_rank=%7B%22rank%22%3A11%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&parent=catalog&search_id=7467802)


[VPC Network Peering](https://www.qwiklabs.com/focuses/964?catalog_rank=%7B%22rank%22%3A10%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&parent=catalog&search_id=7467800)


[Network Performance and Optimization](https://www.qwiklabs.com/quests/46?catalog_rank=%7B%22rank%22%3A3%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&search_id=7468028)


[VPC Flow Logs - Analyzing Network Traffic](https://www.qwiklabs.com/focuses/1236?catalog_rank=%7B%22rank%22%3A12%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&parent=catalog&search_id=7467802)


[Multiple VPC Networks](https://www.qwiklabs.com/focuses/1230?catalog_rank=%7B%22rank%22%3A13%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&parent=catalog&search_id=7467802)


[VPC Networks - Controlling Access](https://www.qwiklabs.com/focuses/1231?catalog_rank=%7B%22rank%22%3A15%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&parent=catalog&search_id=7467802)



[Using VPC Network Peering](https://www.qwiklabs.com/focuses/1249?catalog_rank=%7B%22rank%22%3A16%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&parent=catalog&search_id=7467802)


[VPC Networking: Cloud HA-VPN](https://www.qwiklabs.com/focuses/6270?catalog_rank=%7B%22rank%22%3A18%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&parent=catalog&search_id=7467802)


[Dynamic VPN Gateways - Cloud Routers ](https://www.qwiklabs.com/focuses/1233?parent=catalog)


[Service Directory: Qwik Start](https://www.qwiklabs.com/focuses/12412?catalog_rank=%7B%22rank%22%3A19%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&parent=catalog&search_id=7468061)

