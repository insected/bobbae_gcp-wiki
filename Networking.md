

## Networking

Data Communication and [Computer Networking]( https://www.guru99.com/data-communication-computer-network-tutorial.html  ) provides the rules and regulations that allow computers with different operating systems, languages, cabling, and locations to share resources and communicate with each other. 



### Introduction

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


#### Networking 101

[https://www.youtube.com/watch?v=0hN-dyOV10c](https://www.youtube.com/watch?v=0hN-dyOV10c)

#### CompTIA Network+ full course

https://www.youtube.com/watch?v=qiQR5rTSshw&list=RDCMUC8butISFwT-Wl7EV0hUK0BQ

#### Networking End to End

[https://www.youtube.com/playlist?list=PLIivdWyY5sqJ0oXcnZYqOnuNRsLF9H48u](https://www.youtube.com/playlist?list=PLIivdWyY5sqJ0oXcnZYqOnuNRsLF9H48u)


#### Two Tier vs. Three Tier Architecture

[https://www.wwt.com/article/comparing-two-tier-three-tier-data-center-networks](https://www.wwt.com/article/comparing-two-tier-three-tier-data-center-networks)


 






### Network Options

You can choose from [Network Options](Network-Options).


#### Introduction

Cloud [CDN](https://en.wikipedia.org/wiki/Content_delivery_network) (Content Delivery Network) uses Google's globally distributed edge points of presence to cache external HTTP(S) load balanced content close to your users. Caching content at the edges of Google's network provides faster delivery of content to your users while reducing serving costs. 

There are [DNS](DNS) based CDNs.

The CDN provider typically determines the optimal server selection based on the source IP address of the DNS request (probably combined with other information). However, the source IP address conveyed to the [CDN](https://cloud.google.com/cdn/docs) provider is that of the DNS recursive server, rather than that of the client.




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

[Cloud NAT](https://cloud.google.com/nat/docs) provides fully managed, software-defined network address translation support for Google Cloud.



Moving your internal services to the cloud can bring you a handful of new, useful features, but one of the biggest challenges is protecting your internal endpoints. 

[https://www.youtube.com/watch?v=bmaarG0IkH8](https://www.youtube.com/watch?v=bmaarG0IkH8)


### Cloud Armor

Google [Cloud Armor](https://cloud.google.com/armor/docs) helps protect your infrastructure and applications from distributed denial-of-service (DDoS) attacks by using Google's global infrastructure and security systems.



Setting up Cloud Armor.

[https://www.youtube.com/watch?v=g_c2KLpnWck](https://www.youtube.com/watch?v=g_c2KLpnWck)


### Network Intelligence Center

[Network Intelligence Center](https://cloud.google.com/network-intelligence-center/docs) provides a single console for managing Google Cloud network visibility, monitoring, and troubleshooting.



Getting started with topology in network intelligence center.

[https://www.youtube.com/watch?v=ID7szIL9eew](https://www.youtube.com/watch?v=ID7szIL9eew)


### Network Service Tiers

With [Network Service Tiers](https://cloud.google.com/network-tiers), Google Cloud is the first major public cloud to offer a tiered cloud network. Select the right tier of network service for your requirements and budget.



Cost savings using different network tiers.

[https://www.youtube.com/watch?v=wsdgWGE-mwE](https://www.youtube.com/watch?v=wsdgWGE-mwE)


### Network Telemetry

[VPC](VPC) [Flow Logs](https://cloud.google.com/vpc/docs/using-flow-logs) records a sample of network flows sent from and received by VM instances, including instances used as GKE nodes. These logs can be used for network monitoring, forensics, real-time security analysis, and expense optimization.



Network and security telemetry is fundamental to operate your deployments in public clouds with confidence, providing the required visibility on the behavior of your network and Access control firewalls. 

[https://www.youtube.com/watch?v=as9mXNEcaDo](https://www.youtube.com/watch?v=as9mXNEcaDo)


### Traffic Director


[Traffic Director](Traffic-Director)  is GCP's fully managed traffic control plane for service mesh. With Traffic Director, you can easily deploy global load balancing across clusters and VM instances in multiple regions, offload health checking from service proxies, and configure sophisticated traffic control policies.


### Service Directory

[Service Directory](https://cloud.google.com/service-directory) helps reduce the complexity of management and operations by providing a single place to publish, discover, and connect services. It is a managed service that enhances service inventory management at scale so you don’t have to. Service Directory provides real-time service information, whether you have a few service endpoints or thousands. 



[https://www.youtube.com/watch?v=H9UoE_cWIEY](https://www.youtube.com/watch?v=H9UoE_cWIEY)


### Qwiklabs


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

