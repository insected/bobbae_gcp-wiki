[Border Gateway Protocol](https://en.wikipedia.org/wiki/Border_Gateway_Protocol) version 4 (BGP4) is an exterior gateway protocol that performs inter-autonomous system (AS) or inter-domain routing. It peers to other BGP-speaking systems over TCP to exchange network reachability and routing information. BGP primarily performs two types of routing: inter-AS routing, and intra-AS routing. BGP peers belonging to different autonomous systems use the inter-AS routing, referred as Exterior BGP (eBGP). On the other hand, within an AS BGP can be used to maintain a consistent view of network topology, to provide optimal routing, or to scale the network.


## BGP4+ 


The implementation of IPv6 supports multiprotocol BGP (MBGP) extensions that allow Border Gateway Protocol version 4 plus (BGP4+) to distribute routing information. BGP4+ supports all of the same features and functionality as IPv4 BGP (BGP4).

The extended BGP is commonly known as BGP4+. The specific use of BGP4+ by IPv6 is documented in [RFC2545]. We will use BGP4+ to refer to BGP4+ as deployed in the IPv6 network. We will also use the terms BGP4+ and BGP interchangeably for the remainder of this topic.

http://what-when-how.com/ipv6-advanced-protocols-implementation/introduction-to-bgp4-ipv6-unicast-routing-protocols-part-1/

### Kubernetes and BGP

https://www.asykim.com/blog/kubernetes-traffic-engineering-with-bgp

## VRRPv2 

Virtual Router Redundancy Protocol (VRRP) is an election protocol that provides redundancy to routers within a Local Area Network (LAN).

VRRP was designed to eliminate a single point of failure in a static default-route environment by dynamically assigning virtual IP routers to participating hosts. A virtual router is a collection of physical routers whose interfaces must belong to the same IP subnet. A virtual router ID (VRID) is assigned to each virtual router, but there is no restriction against reusing a VRID with a different address mapping on different LANs.

https://en.wikipedia.org/wiki/Virtual_Router_Redundancy_Protocol

## VRRPv3

VRRPv3 implements support for IPv6 addresses for networks using IPv6, and it also supports IPv4 addresses for dual-stack networks configured with VRRP or VRRP-E. VRRPv3 is compliant with RFC 5798. The benefit of implementing VRRPv3 is faster switchover to backup devices than can be achieved using standard IPv6 neighbor discovery mechanisms. With VRRPv3, a backup router can become a master router in a few seconds with less overhead traffic and no interaction with the hosts.

https://datatracker.ietf.org/doc/html/rfc5798

## OSPF

Open Shortest Path First (OSPF) is a routing protocol for Internet Protocol (IP) networks. It uses a link state routing (LSR) algorithm and falls into the group of interior gateway protocols (IGPs), operating within a single autonomous system (AS). 

https://en.wikipedia.org/wiki/Open_Shortest_Path_First

OSPF works on [Dijkstra algorithm](https://en.wikipedia.org/wiki/Dijkstra%27s_algorithm).

## RIP

RIP (Routing Information Protocol), is an example of distance vector routing for local networks. RIP works to deliver the whole routing table to all active interfaces every 30 seconds. In RIP protocol, hop count is the only metrics to decide the best path to a remote network. 

https://en.wikipedia.org/wiki/Routing_Information_Protocol

## Router firmware

https://en.wikipedia.org/wiki/List_of_router_firmware_projects
