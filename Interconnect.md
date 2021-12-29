

[Cloud Interconnect](https://cloud.google.com/network-connectivity/docs/interconnect)    extends your [on-premises network to Google's network](https://www.google.com/url?sa=t&source=web&rct=j&url=https://m.youtube.com/watch%3Fv%3DZMHXxHaCAeE&ved=2ahUKEwjkxcbgp7DwAhUUKn0KHSOfAHUQxa8BegQIBhAE&usg=AOvVaw3ZbaIFoh-HX2gY56RKcCEC) through a [highly available, low latency connection](https://www.google.com/url?sa=t&source=web&rct=j&url=https://m.youtube.com/watch%3Fv%3DqsDfazSdoKo&ved=2ahUKEwibotPjp7DwAhU4JDQIHYj6ACY4ChDFrwF6BAgKEAQ&usg=AOvVaw2--dDU-IoK1iHy_sGEW9lY).

You can use [Dedicated Interconnect](https://www.youtube.com/watch?v=cKaryf7qp9w) to connect directly to Google or use [Partner Interconnect](https://cloud.google.com/network-connectivity/docs/interconnect/concepts/partner-overview) to connect to Google through a [supported service provider](https://cloud.google.com/network-connectivity/docs/interconnect/concepts/service-providers).



While migrating portions of your on-prem to the cloud, it’s important for your on-prem systems to communicate with your newly minted cloud resource.

## Network Connectivity Center

https://cloud.google.com/network-connectivity-center


https://cloud.google.com/blog/products/networking/google-cloud-network-connectivity-center-networking-partnerships


## Google Cloud Interconnect Overview

The first step when establishing connectivity to Google Cloud is to set up a Virtual Private Cloud (VPC).

Google Cloud’s VPC is a private, managed virtual network that connects VM instances, Google Kubernetes Engine (GKE) clusters, and the Google App Engine flexible environment.





## Dedicated Interconnect




Dedicated Interconnect [provides direct physical connections](https://docs.packetfabric.com/cloud/google/overview/)  between your on-premises network and Google's network. Dedicated Interconnect enables you to transfer large amounts of data between networks, which can be more cost effective than purchasing additional bandwidth over the public Internet.



After you create a VLAN attachment, you need to configure your on-premises router to establish a BGP session with your [Cloud Router](https://cloud.google.com/network-connectivity/docs/interconnect/how-to/dedicated/configuring-onprem-routers). Use the VLAN ID, interface IP address, and peering IP address provided by the [VLAN attachment](https://cloud.google.com/network-connectivity/docs/interconnect/how-to/dedicated/creating-vlan-attachments) to configure your on-premises router.




## Partner Interconnect




[Partner Interconnect](https://cloud.google.com/network-connectivity/docs/interconnect/concepts/partner-overview) provides connectivity between your on-premises network and your VPC network through a supported [service provider](https://cloud.google.com/network-connectivity/docs/interconnect/concepts/service-providers). 

A [Partner Interconnect connection](https://cloud.google.com/network-connectivity/docs/interconnect/how-to/partner/provisioning-overview)     is useful if your data center is in a physical location that can't reach a Dedicated Interconnect colocation facility or if your data needs don't warrant an entire 10 Gbps connection.



An on-premises router in this context means a [Layer 2 (L2) or Layer 3 (L3)](https://cloud.google.com/network-connectivity/docs/interconnect/concepts/partner-overview#connectivity-type)  [device](https://cloud.google.com/network-connectivity/docs/interconnect/how-to/partner/configuring-onprem-routers) you configure to enable Partner Interconnect.


To provision a Partner Interconnect connection with a [service provider](https://cloud.google.com/network-connectivity/docs/interconnect/concepts/service-providers), you start by connecting your on-premises network to a supported service provider. Work with the service provider to establish connectivity.

Next, you create a VLAN attachment for a Partner Interconnect connection in your Google Cloud project, which generates a unique pairing key that you use to request a connection from your service provider. You also need to provide other information such as the connection location and capacity.

After the service provider configures your VLAN attachment, you activate your connection to start using it. Depending on your connection, either you or your service provider then establishes a Border Gateway Protocol (BGP) session.
