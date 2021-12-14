[Cloud Router](https://cloud.google.com/network-connectivity/docs/router) is a Cloud service that programs custom dynamic routes and scales with your network traffic. Cloud Router works with both legacy networks and Virtual Private Cloud (VPC) networks.

Cloud Router is a fully distributed and managed service that programs custom dynamic routes and scales with the network traffic. 

[Cloud Router](https://cloud.google.com/network-connectivity/docs/router)  enables you to dynamically exchange routes between your Virtual Private Cloud (VPC) and on-premises networks by using [Border Gateway Protocol (BGP)](https://www.wikipedia.org/wiki/Border_Gateway_Protocol). 

For example, if you use a Cloud [VPN](VPN) tunnel to connect your networks, you can [use Cloud Router to establish a BGP session with your on-premises router over your Cloud VPN tunnel](https://medium.com/google-cloud/dynamic-routing-with-cloud-router-9ff5c362d833  ). Cloud Router automatically learns new subnets in your [VPC](VPC) network and announces them to your on-premises network.





## BGP



Border Gateway Protocol (BGP) is a standardized exterior gateway protocol designed to [exchange routing and reachability information](https://www.youtube.com/watch?v=_Z29ZzKeZHc) among autonomous systems (AS) on the Internet. 

[BGP]( https://engineering.fb.com/2021/05/13/data-center-engineering/bgp/   ) is classified as a path-vector routing protocol, and it makes routing decisions based on paths, network policies, or rule-sets configured by a network administrator.


[Cloud Router uses Border Gateway Protocol](https://cloud.google.com/network-connectivity/docs/router/how-to/configuring-bgp) (BGP) to exchange routes between your Virtual Private Cloud (VPC) network and your on-premises network.  This is great for setting up VPN between the cloud and on-prem, as topology changes automatically propagate with no manual intervention and higher redundancy for your systems.

On Cloud Router, you configure an interface and a [BGP](https://en.wikipedia.org/wiki/Border_Gateway_Protocol) peer for your on-premises router. The interface and BGP peer configuration together form a BGP session.





## Dynamic Routing

The biggest pitfall with static routes is that they aren’t fault-tolerant. Any change to the routing infrastructure, like a failed VM or re-architecture, would mean manual intervention. 

If routers are purely static, they have no way of choosing a better route if a link becomes unavailable. They have no way to intelligently share information between one another to advertise alternative routes. Simply stated, static routes are great for stable networks that don’t change.

<!--
<img src="https://miro.medium.com/max/5400/1*yZclHkU5wb-xTGj8fhb24w.png" width="500">
-->


Instead of a static routing table, dynamic routers advertise their routes to other routers, meaning they exchange information. 

It allows routers on the network to make intelligent decisions on which path is best to get data to a subnet/destination. 

A dynamic routing table is created, maintained, and updated by a routing protocol (like BGP) running on the router. This lets the router dynamically choose a different (or better) path when there is a change to the routing infrastructure, like when a link fails. 

It’s like how Google Maps recalculates a new optimal path when your current route becomes flooded with traffic or an accident occurs. 

Cloud Routers make determinations based on several criteria, including network quality, link up/down, traffic congestion, etc. 

The key benefit here is redundancy. If one path on the network disappears, dynamic routing will adjust routes around that path without manual intervention.

You can learn more about [Dynamic routing with Cloud Router](https://medium.com/google-cloud/dynamic-routing-with-cloud-router-9ff5c362d833) and view this [video](https://www.youtube.com/watch?v=K_xb_j46YOk).


Dynamic routing does have [risks that should be considered](  https://www.wired.com/story/bgp-routing-manrs-google-fix/  ).
