


Data Communication and [Computer Networking]( https://www.guru99.com/data-communication-computer-network-tutorial.html  ) provides the rules and regulations that allow computers with different operating systems, languages, cabling, and locations to share resources and communicate with each other. 



## Introduction

Google Cloud Platform includes [software-defined networking](https://developers.google.com/learn/topics/networking), hybrid connectivity, network performance optimization, network security, service mesh deployment, NAT, load balancing, and routing.



GCP implements [software-defined network](  https://cloud.google.com/docs/compare/data-centers/networking ) that provides [fast and reliable connections](  https://cloud.google.com/blog/products/networking/google-cloud-networking-in-depth-series-digest ) to users [around the world](https://cloud.google.com/about/locations).

Google Cloud customers enjoy significantly improved intra-zone network latency with the [Andromeda  software-defined network]( https://cloud.google.com/blog/products/gcp/andromeda-2-1-reduces-gcps-intra-zone-latency-by-40-percent  ) (SDN) stack that underpins all of Google Cloud.




Google's own [Jupiter network fabrics](  https://research.google/pubs/pub43837/ )   can deliver more than 1 Petabit/sec of total bisection bandwidth. To put this in perspective, such [capacity](https://cloudplatform.googleblog.com/2015/06/A-Look-Inside-Googles-Data-Center-Networks.html?m=1) would be enough for 100,000 servers to exchange information at 10Gb/s each, enough to read the entire scanned contents of the Library of Congress in less than 1/10th of a second.

From data centers to subsea cables, GCP connects customers in [different regions](https://www.blog.google/products/google-cloud/expanding-our-global-infrastructure-new-regions-and-subsea-cables/) around the world.



<img src="https://storage.googleapis.com/gweb-uniblog-publish-prod/images/infrastructure-3.max-1000x1000.png" width="700">

In a traditional data center, you manage a complex network setup composed of racks of servers, storage devices, multiple layers of switches, routers, load balancers, firewall devices, and more. 

In addition to these hardware components, you must set up, maintain, and monitor the network's underlying software, as well as detailed device configurations for your environment. And the managerial overhead doesn't end there: you also have to worry about the security and availability of your network, and you must plan out the upgrades and expansions of your network—a lengthy and time-consuming process.



Google built a superior [cloud network](https://cloud.google.com/docs/compare/data-centers/networking) as a result of the well-provisioned direct paths between its cloud and end-users.

<img src="https://storage.googleapis.com/gweb-uniblog-publish-prod/images/infrastructure-1.max-1000x1000.png" width="500">


## Networking 101

[https://www.youtube.com/watch?v=0hN-dyOV10c](https://www.youtube.com/watch?v=0hN-dyOV10c)

### OSI Model

The Open Systems Interconnection model (OSI model) is a conceptual model that characterises and standardises the communication functions of a telecommunication or computing system without regard to its underlying internal structure and technology. Its goal is the interoperability of diverse communication systems with standard communication protocols.


The recommendation X.200 describes seven layers, labelled 1 to 7.

https://en.wikipedia.org/wiki/OSI_model


### TCP/IP

The Internet protocol suite, commonly known as TCP/IP, is the set of communications protocols used in the Internet and similar computer networks. The current foundational protocols in the suite are the Transmission Control Protocol (TCP) and the Internet Protocol (IP).


https://en.wikipedia.org/wiki/Internet_protocol_suite


### CIDR

Classless Inter-Domain Routing (CIDR /ˈsaɪdər, ˈsɪ-/) is a method for allocating IP addresses and for IP routing. The Internet Engineering Task Force introduced CIDR in 1993 to replace the previous classful network addressing architecture on the Internet. Its goal was to slow the growth of routing tables on routers across the Internet, and to help slow the rapid exhaustion of IPv4 addresses.

https://en.wikipedia.org/wiki/Classless_Inter-Domain_Routing

### Routing

IP routing is the field of routing methodologies of Internet Protocol (IP) packets within and across IP networks. This involves not only protocols and technologies but includes the policies of the worldwide organization and configuration of Internet infrastructure. In each IP network node, IP routing involves the determination of a suitable path for a network packet from a source to its destination in an IP network. The process uses static configuration rules or dynamically obtained status information to select specific packet forwarding methods to direct traffic to the next available intermediate network node one hop closer to the desired final destination, a total path potentially spanning multiple computer networks.

https://en.wikipedia.org/wiki/IP_routing

### DNS

The [Domain Name System](DNS) (DNS) is a hierarchical and decentralized naming system for computers, services, or other resources connected to the Internet or a private network. It associates various information with domain names assigned to each of the participating entities. Most prominently, it translates more readily memorized domain names to the numerical IP addresses needed for locating and identifying computer services and devices with the underlying network protocols. By providing a worldwide, distributed directory service, the Domain Name System has been an essential component of the functionality of the Internet since 1985.

https://en.wikipedia.org/wiki/Domain_Name_System

### Ethernet

Ethernet (/ˈiːθərnɛt/) is a family of wired computer networking technologies commonly used in local area networks (LAN), metropolitan area networks (MAN) and wide area networks (WAN).

https://en.wikipedia.org/wiki/Ethernet

### Network Switch

A network switch (also called switching hub, bridging hub, and, by the IEEE, MAC bridge[1]) is networking hardware that connects devices on a computer network by using packet switching to receive and forward data to the destination device.

https://en.wikipedia.org/wiki/Network_switch

### Network Router

A router[a] is a networking device that forwards data packets between computer networks. Routers perform the traffic directing functions on the Internet. Data sent through the internet, such as a web page or email, is in the form of data packets. A packet is typically forwarded from one router to another router through the networks that constitute an internetwork (e.g. the Internet) until it reaches its destination node.

https://en.wikipedia.org/wiki/Router_(computing)

### Routing Protocols

A routing protocol specifies how routers communicate with each other to distribute information that enables them to select routes between nodes on a computer network. Routers perform the traffic directing functions on the Internet; data packets are forwarded through the networks of the internet from router to router until they reach their destination computer. Routing algorithms determine the specific choice of route. Each router has a prior knowledge only of networks attached to it directly. A routing protocol shares this information first among immediate neighbors, and then throughout the network. This way, routers gain knowledge of the topology of the network. The ability of routing protocols to dynamically adjust to changing conditions such as disabled connections and components and route data around obstructions is what gives the Internet its fault tolerance and high availability.

https://en.wikipedia.org/wiki/Routing_protocol

### Subnetwork

A subnetwork or subnet is a logical subdivision of an IP network.[1]:1,16 The practice of dividing a network into two or more networks is called subnetting.

Computers that belong to the same subnet are addressed with an identical most-significant bit-group in their IP addresses. This results in the logical division of an IP address into two fields: the network number or routing prefix and the rest field or host identifier. The rest field is an identifier for a specific host or network interface.

https://en.wikipedia.org/wiki/Subnetwork

## CompTIA Network+ full course

https://www.youtube.com/watch?v=qiQR5rTSshw&list=RDCMUC8butISFwT-Wl7EV0hUK0BQ

## Networking End to End

[https://www.youtube.com/playlist?list=PLIivdWyY5sqJ0oXcnZYqOnuNRsLF9H48u](https://www.youtube.com/playlist?list=PLIivdWyY5sqJ0oXcnZYqOnuNRsLF9H48u)


## Two Tier vs. Three Tier Architecture

### Networking point of view

[https://www.wwt.com/article/comparing-two-tier-three-tier-data-center-networks](https://www.wwt.com/article/comparing-two-tier-three-tier-data-center-networks)

### Database point of view

https://www.softwaretestingclass.com/what-is-difference-between-two-tier-and-three-tier-architecture/
 






## GCP Network Options

Google's connectivity solutions enable you to connect your networks to Google in the following ways:

- To Google Cloud, which enables you to access your Virtual Private Cloud (VPC) networks and Compute Engine virtual machine (VM) instances from your on-premises networks or from another cloud provider.

- To connect your sites together through a Network Connectivity Center hub located in Google Cloud.

- To Google Workspace and supported Google APIs, which lets you access only these products and services.

- To CDN providers, which enables you to choose supported content delivery providers that establish Direct Peering links with Google's edge network. Choosing a provider enables you to send traffic from your VPC networks to that provider.



You can choose from [Network Options](Network-Options).


## CDN

Cloud [CDN](CDN) (Content Delivery Network) uses Google's globally distributed edge points of presence to cache external HTTP(S) load balanced content close to your users. Caching content at the edges of Google's network provides faster delivery of content to your users while reducing serving costs. 

There are [DNS](DNS) based CDNs.

The CDN provider typically determines the optimal server selection based on the source IP address of the DNS request (probably combined with other information). However, the source IP address conveyed to the [CDN](https://cloud.google.com/cdn/docs) provider is that of the DNS recursive server, rather than that of the client.

https://www.iotforall.com/cellular-iot-explained-nb-iot-vs-lte-m


### Using CDN and Load Balancing

[https://www.youtube.com/watch?v=NedNhOg_TgA](https://www.youtube.com/watch?v=NedNhOg_TgA)


### Setting up Cloud CDN with backend storage bucket


Cloud CDN leverages Google Cloud global external HTTP(S) load balancers to provide routing, health checking, and Anycast IP support. Because global external HTTP(S) load balancers can have multiple backend instance types— Compute Engine VM instances, Google Kubernetes Engine Pods, Cloud Storage buckets, or external backends outside of Google Cloud—you can choose which backends (origins) to enable Cloud CDN for.

[https://cloud.google.com/cdn/docs/setting-up-cdn-with-bucket](https://cloud.google.com/cdn/docs/setting-up-cdn-with-bucket)

## VPN

[VPN](VPN) extends a private network across a public network and enables users to send and receive data across shared or public networks as if their computing devices were directly connected to the private network.

https://en.wikipedia.org/wiki/Virtual_private_network

## VLAN

A [virtual LAN](VLAN) (VLAN) is any broadcast domain that is partitioned and isolated in a computer network at the data link layer (OSI layer 2).

## BGP

Border Gateway Protocol (BGP) is a standardized exterior gateway protocol designed to exchange routing and reachability information among autonomous systems (AS) on the Internet. BGP is classified as a path-vector routing protocol, and it makes routing decisions based on paths, network policies, or rule-sets configured by a network administrator.


https://en.wikipedia.org/wiki/Border_Gateway_Protocol

## MPLS


Multiprotocol Label Switching (MPLS) is a routing technique in telecommunications networks that directs data from one node to the next based on short path labels rather than long network addresses, thus avoiding complex lookups in a routing table and speeding traffic flows. The labels identify virtual links (paths) between distant nodes rather than endpoints. MPLS can encapsulate packets of various network protocols, hence the "multiprotocol" reference on its name. MPLS supports a range of access technologies, including [T1/E1](https://en.wikipedia.org/wiki/Digital_Signal_1), [ATM](https://en.wikipedia.org/wiki/Asynchronous_Transfer_Mode), [Frame Relay](https://en.wikipedia.org/wiki/Frame_Relay), and [DSL](https://en.wikipedia.org/wiki/Digital_subscriber_line).

https://en.wikipedia.org/wiki/Multiprotocol_Label_Switching


## Hybrid Connectivity

[https://cloud.google.com/hybrid-connectivity](https://cloud.google.com/hybrid-connectivity)

### Cloud Interconnect

Enterprise-grade connections to your Google VPC backed by industry-leading SLAs. Choose a 10 Gbps or 100 Gbps pipe and connect directly to a Google location with Dedicated Interconnect, or flexible bandwidth options (50 Mbps to 10 Gbps) with Partner Interconnect.


https://cloud.google.com/network-connectivity/docs/interconnect

### Cloud VPN

Connect your on-premises or other public cloud networks to your Google VPC securely over the internet through IPsec VPN at a low cost for your data bandwidth needs up to 3.0 Gbps. High availability VPN offers the best SLA in the industry, with a guaranteed uptime of 99.99%.


https://cloud.google.com/network-connectivity/docs/vpn


### Cloud Interconnect

[Interconnect](Interconnect) extends your on-premises network to Google's network through a highly available, low latency connection. 

### Peering with Google

Access Google and Google Cloud features over VPN or the internet, while cutting egress fees. If you can meet Google's requirements, connect directly with Direct Peering, or choose a partner with Carrier Peering.

#### Direct Peering

Direct Peering enables you to establish a direct peering connection between your business network and Google's edge network and exchange high-throughput cloud traffic.

This capability is available at any of more than 100 locations in 33 countries around the world. For more information about Google's edge locations, see Google's peering site.

https://cloud.google.com/network-connectivity/docs/direct-peering

#### Carrier Peering 

Carrier Peering enables you to access Google applications, such as Google Workspace, by using a service provider to obtain enterprise-grade network services that connect your infrastructure to Google.

When connecting to Google through a service provider, you can get connections with higher availability and lower latency, using one or more links. Work with your service provider to get the connection that you need.

https://cloud.google.com/network-connectivity/docs/carrier-peering


#### Partner Interconnect

Partner Interconnect provides connectivity between your on-premises network and your Virtual Private Cloud (VPC) network through a supported service provider. A Partner Interconnect connection is useful if your data center is in a physical location that can't reach a Dedicated Interconnect colocation facility, or your data needs don't warrant an entire 10-Gbps connection.



https://cloud.google.com/network-connectivity/docs/interconnect/concepts/partner-overview


#### VLAN and Interconnect

https://cloud.google.com/network-connectivity/docs/interconnect/support/faq#interconnect-attachments

#### BGP and MPLS

https://cloud.google.com/network-connectivity/docs/interconnect/support/faq#self-mpls-vpn


## Cloud Load Balancing

[Load Balancer](Load-Balancer) distributes user traffic across multiple instances of your applications. By spreading the load, load balancing reduces the risk that your applications experience performance issues.

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



Getting started with topology in network intelligence center.

[https://www.youtube.com/watch?v=ID7szIL9eew](https://www.youtube.com/watch?v=ID7szIL9eew)


## Network Service Tiers

With [Network Service Tiers](https://cloud.google.com/network-tiers), Google Cloud is the first major public cloud to offer a tiered cloud network. Select the right tier of network service for your requirements and budget.



Cost savings using different network tiers.

[https://www.youtube.com/watch?v=wsdgWGE-mwE](https://www.youtube.com/watch?v=wsdgWGE-mwE)


## Network Telemetry

[VPC](VPC) [Flow Logs](https://cloud.google.com/vpc/docs/using-flow-logs) records a sample of network flows sent from and received by VM instances, including instances used as GKE nodes. These logs can be used for network monitoring, forensics, real-time security analysis, and expense optimization.



Network and security telemetry is fundamental to operate your deployments in public clouds with confidence, providing the required visibility on the behavior of your network and Access control firewalls. 

[https://www.youtube.com/watch?v=as9mXNEcaDo](https://www.youtube.com/watch?v=as9mXNEcaDo)


## Traffic Director


[Traffic Director](Traffic-Director)  is GCP's fully managed traffic control plane for service mesh. With Traffic Director, you can easily deploy global load balancing across clusters and VM instances in multiple regions, offload health checking from service proxies, and configure sophisticated traffic control policies.


## Service Directory

[Service Directory](https://cloud.google.com/service-directory) helps reduce the complexity of management and operations by providing a single place to publish, discover, and connect services. It is a managed service that enhances service inventory management at scale so you don’t have to. Service Directory provides real-time service information, whether you have a few service endpoints or thousands. 



[https://www.youtube.com/watch?v=H9UoE_cWIEY](https://www.youtube.com/watch?v=H9UoE_cWIEY)




## Network Security

Network [Security](Security) consists of the policies, processes and practices adopted to prevent, detect and monitor unauthorized access, misuse, modification, or denial of a computer network and network-accessible resources.

https://en.wikipedia.org/wiki/Network_security

## LAN

A local area network (LAN) is a computer network that interconnects computers within a limited area such as a residence, school, laboratory, university campus or office building. By contrast, a wide area network (WAN) not only covers a larger geographic distance, but also generally involves leased telecommunication circuits.

Ethernet and Wi-Fi are the two most common technologies in use for local area networks. Historical network technologies include [ARCNET](https://en.wikipedia.org/wiki/ARCNET), [Token Ring](https://en.wikipedia.org/wiki/Token_Ring), and [AppleTalk](https://en.wikipedia.org/wiki/AppleTalk).


https://en.wikipedia.org/wiki/Local_area_network


## WAN

A wide area network (WAN) is a telecommunications network that extends over a large geographic area for the primary purpose of computer networking. Wide area networks are often established with leased telecommunication circuits.

Businesses, as well as schools and government entities, use wide area networks to relay data to staff, students, clients, buyers and suppliers from various locations across the world. In essence, this mode of telecommunication allows a business to effectively carry out its daily function regardless of location. The Internet may be considered a WAN.


https://en.wikipedia.org/wiki/Wide_area_network

## NAT

Network address translation (NAT) is a method of mapping an IP address space into another by modifying network address information in the IP header of packets while they are in transit across a traffic routing device. 

The technique was originally used to avoid the need to assign a new address to every host when a network was moved, or when the upstream Internet service provider was replaced, but could not route the networks address space. It has become a popular and essential tool in conserving global address space in the face of IPv4 address exhaustion. One Internet-routable IP address of a NAT gateway can be used for an entire private network.

https://en.wikipedia.org/wiki/Network_address_translation


## Firewall

A firewall is a network security system that monitors and controls incoming and outgoing network traffic based on predetermined security rules. A firewall typically establishes a barrier between a trusted network and an untrusted network, such as the Internet.


GCP Firewall rules are defined at the network level, and only apply to the network where they are created; however, the name you choose for each of them must be unique to the project.

A firewall rule can contain either IPv4 or IPv6 ranges, but not both.

https://cloud.google.com/vpc/docs/using-firewalls

## Underlay network

Underlay network is closer to the physical layer. It includes switches, routers, VLANs and so on. It is the basis on which overlay networks are built. It tends to be less scalable due to technical limitations. However, since it’s closer to the actual hardware, it is slightly faster than an overlay.

## Overlay network

Overlay network refers to the virtual network layer. It is designed to be highly scalable than the underlying network. For example, while VLANs in the underlying network support only 4096 identifiers, VxLAN can reach up to 16 million ones.

## Kubernetes Networking

[Kubernetes Networking](Kubernetes-Networking) supports both networking models, so you can base your model of choice on other factors than whether or not the cluster can handle it.

## Kubernetes CNI

A [CNI](Kubernetes-Networking#cni) is simply a link between the container runtime (like Docker or rkt) and the network plugin. The network plugin is nothing but the executable that handles the actual connection of the container to or from the network, according to a set of rules defined by the CNI. So, to put it simply, a CNI is a set of rules and Go libraries that aid in container/network-plugin integration.

All of the CNIs can be deployed by simply running a pod or a daemonset that launches and manages their daemons. Let’s have a look now at the most well-known Kubernetes networking solutions.


## IOT Networking

### 802.15.4

IEEE 802.15.4 is a technical standard which defines the operation of low-rate wireless personal area networks (LR-WPANs). It specifies the physical layer and media access control for LR-WPANs, and is maintained by the IEEE 802.15 working group, which defined the standard in 2003.


https://standards.ieee.org/standard/802_15_4-2020.html

### ZigBee 

ZigBee is a 2.4 GHz mesh local area network (LAN) protocol. It was originally designed for building automation and control—so things like wireless thermostats and lighting systems often use ZigBee.


https://zigbeealliance.org/solution/zigbee/


### LoRaWAN 

LoRaWAN is a media access control (MAC) layer protocol designed for large-scale public networks with a single operator. It is built using Semtech’s LoRa modulation as the underlying PHY, but it is important to note that LoRa and LoRaWAN are two seperate things that are often (mistakenly) conflated. 


https://lora-alliance.org/

### GPRS 

General Packet Radio Service (GPRS) is a packet oriented mobile data standard on the 2G and 3G cellular communication network's global system for mobile communications (GSM). GPRS was established by European Telecommunications Standards Institute (ETSI) in response to the earlier CDPD and i-mode packet-switched cellular technologies. It is now maintained by the 3rd Generation Partnership Project (3GPP).

https://www.twilio.com/docs/glossary/what-general-packet-radio-service-gprs


### 3G & 4G

3G was the first “high speed” cellular network, and is a name that refers to a number of technologies that meet IMT-2000 standards. 4G is the generation of cellular standards that followed 3G, and is what most people use today for mobile cellular data. You can use 3G and 4G for IoT devices, but the application needs a constant power source or must be able to be recharged regularly.

### LTE Cat 0, 1, & 3

With LTE classes, the lower the speed, the lower the amount of power they use. LTE Cat 1 and 0 are typically more suitable for IoT devices. (You can learn more about them in this Radio-Electronics article.)

### LTE-M1

This is the first cellular wireless protocol that was build from the ground up for IoT devices. That being said, it isn’t available yet, so how it performs remains to be seen.

With LTE,  it’s worth understanding that carriers typically don’t have to modify hardware for their basestations; upgrades can be done entirely through software. This really helps with infrastructure costs, because companies won’t necessarily need new cellular basestations, just new endpoint hardware.


### NB-IoT

NB-IoT, or Narrowband IoT, is another way to tackle cellular M2M for low power devices. It is based on a DSSS modulation similar to the old Neul version of Weightless-W. Huawei, Ericsson, and Qualcomm are active proponents of this protocol and are involved in putting it together.

### GSM

The Global System for Mobile Communications (GSM) is a standard developed by the European Telecommunications Standards Institute (ETSI) to describe the protocols for second-generation (2G) digital cellular networks used by mobile devices such as mobile phones and tablets. It was first deployed in Finland in December 1991.

https://en.wikipedia.org/wiki/GSM

### 5G


5G is the fifth generation technology standard for broadband cellular networks, which cellular phone companies began deploying worldwide in 2019, and is the planned successor to the 4G networks which provide connectivity to most current cellphones. 5G networks are predicted to have more than 1.7 billion subscribers worldwide by 2025, according to the GSM Association.

https://en.wikipedia.org/wiki/5G

### Cellular IoT Overview

https://www.iotforall.com/cellular-iot-explained-nb-iot-vs-lte-m

### MQTT 

An MQTT (Message Queuing Telemetry Transport) is a lightweight IoT data protocol. It features a publisher-subscriber messaging model and allows for simple data flow between different devices.

MQTT’s main selling point is its architecture. Its genetic make-up is basic and lightweight and, therefore, it’s able to provide low power consumption for devices. It also works on top of a TCP/IP protocol.

IoT data protocols were designed to tackle unreliable communication networks. This became a need in the IoT world due to the increasing number of small, cheap, and lower-power objects that have appeared in the network over the past few years.

https://en.wikipedia.org/wiki/MQTT

### CoAP

A CoAp (Constrained Application Protocol) is an application layer protocol. It’s designed to address the needs of HTTP-based IoT systems. HTTP stands for Hypertext Transfer Protocol, and it’s the foundation of data communication for the World Wide Web.

While the existing structure of the internet is freely available and usable by any IoT device, it’s often too heavy and power-consuming for most IoT applications. This has led to many within the IoT community dismissing HTTP as a protocol not suitable for IoT.

https://en.wikipedia.org/wiki/Constrained_Application_Protocol


### AMQP 

An Advanced Message Queuing Protocol (AMQP) is an open standard application layer protocol used for transactional messages between servers.

AMQP is an open standard application layer protocol for message-oriented middleware. The defining features of AMQP are message orientation, queuing, routing (including point-to-point and publish-and-subscribe), reliability and security.

AMQP mandates the behavior of the messaging provider and client to the extent that implementations from different vendors are interoperable, in the same way as SMTP, HTTP, FTP, etc. have created interoperable systems. Previous standardizations of middleware have happened at the API level (e.g. JMS) and were focused on standardizing programmer interaction with different middleware implementations, rather than on providing interoperability between multiple implementations.

AMQP was originated in 2003 by John O'Hara at JPMorgan Chase in London. AMQP was conceived as a co-operative open effort. The initial design was by JPMorgan Chase from mid-2004 to mid-2006 and it contracted iMatix Corporation to develop a C broker and protocol documentation. In 2005 JPMorgan Chase approached other firms to form a working group that included Cisco Systems, IONA Technologies, iMatix, Red Hat, and Transaction Workflow Innovation Standards Team (TWIST). In the same year JPMorgan Chase partnered with Red Hat to create Apache Qpid, initially in Java and soon after C++. Independently, [RabbitMQ](https://en.wikipedia.org/wiki/RabbitMQ) was developed in [Erlang](https://en.wikipedia.org/wiki/Erlang_(programming_language)) by Rabbit Technologies, followed later by the Microsoft and StormMQ implementations.



### DDS 


DDS (Data Distribution Service) is another scalable IoT protocol that enables high-quality communication in IoT. Similar to the MQTT, DDS also works to a publisher-subscriber model.

It can be deployed in multiple settings, from the cloud to very small devices. This makes it perfect for real-time and embedded systems. Moreover, unlike MQTT, the DDS protocol allows for interoperable data exchange that is independent of the hardware and the software platform.

## Industrial Networking

### Modbus

Modbus is a granddaddy of industrial communication protocols. Modbus is Modicon plus fieldbus.

Modbus, a serial communication protocol developed by Modicon in 1979. It is developed by  Modicon for PLC in industrial applications, now it an open protocol. It is used over serial and Ethernet cable.

https://instrumentationtools.com/compare-modbus-fieldbus-and-profibus/


### Profibus


Profibus (usually styled as PROFIBUS, as a portmanteau for Process Field Bus) is a standard for fieldbus communication in automation technology and was first promoted in 1989 by BMBF (German department of education and research) and then used by Siemens. It should not be confused with the Profinet standard for Industrial Ethernet. Profibus is openly published as part of IEC 61158.

https://en.wikipedia.org/wiki/Profibus


### CANBus

A Controller Area Network (CAN bus) is a robust vehicle bus standard designed to allow microcontrollers and devices to communicate with each other's applications without a host computer. It is a message-based protocol, designed originally for multiplex electrical wiring within automobiles to save on copper, but it can also be used in many other contexts. For each device, the data in a frame is transmitted sequentially but in such a way that if more than one device transmits at the same time, the highest priority device can continue while the others back off. Frames are received by all devices, including by the transmitting device.

https://en.wikipedia.org/wiki/CAN_bus


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

