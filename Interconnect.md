

[Cloud Interconnect](https://cloud.google.com/network-connectivity/docs/interconnect)    extends your on-premises network to Google's network through a highly available, low latency connection. You can use Dedicated Interconnect to connect directly to Google or use Partner Interconnect to connect to Google through a supported service provider.



While migrating portions of your on-prem to the cloud, it’s important for your on-prem systems to communicate with your newly minted cloud resource.

[https://www.youtube.com/watch?v=cKaryf7qp9w](https://www.youtube.com/watch?v=cKaryf7qp9w)

## Google Cloud Interconnect Overview

The first step when establishing connectivity to Google Cloud is to set up a Virtual Private Cloud (VPC).

Google Cloud’s VPC is a private, managed virtual network that connects VM instances, Google Kubernetes Engine (GKE) clusters, and the Google App Engine flexible environment.



https://docs.packetfabric.com/cloud/google/overview/

## Dedicated Interconnect


<img src="https://docs.packetfabric.com/cloud/google/images/google_overview_dedicated.svg" width="600">

Dedicated Interconnect provides direct physical connections between your on-premises network and Google's network. Dedicated Interconnect enables you to transfer large amounts of data between networks, which can be more cost effective than purchasing additional bandwidth over the public Internet.

[https://cloud.google.com/network-connectivity/docs/interconnect](https://cloud.google.com/network-connectivity/docs/interconnect)

After you create a VLAN attachment, you need to configure your on-premises router to establish a BGP session with your Cloud Router. Use the VLAN ID, interface IP address, and peering IP address provided by the [VLAN attachment](https://cloud.google.com/network-connectivity/docs/interconnect/how-to/dedicated/creating-vlan-attachments) to configure your on-premises router.

[https://cloud.google.com/network-connectivity/docs/interconnect/how-to/dedicated/configuring-onprem-routers](https://cloud.google.com/network-connectivity/docs/interconnect/how-to/dedicated/configuring-onprem-routers)


## Partner Interconnect

<img src="https://docs.packetfabric.com/cloud/google/images/google_overview_hosted.svg" width="600">

Partner Interconnect provides connectivity between your on-premises network and your VPC network through a supported [service provider](https://cloud.google.com/network-connectivity/docs/interconnect/concepts/service-providers). A Partner Interconnect connection is useful if your data center is in a physical location that can't reach a Dedicated Interconnect colocation facility or if your data needs don't warrant an entire 10 Gbps connection.

[https://cloud.google.com/network-connectivity/docs/interconnect](https://cloud.google.com/network-connectivity/docs/interconnect)

An on-premises router in this context means a Layer 2 (L2) or Layer 3 (L3) device you configure to enable Partner Interconnect.

[https://cloud.google.com/network-connectivity/docs/interconnect/how-to/partner/configuring-onprem-routers](https://cloud.google.com/network-connectivity/docs/interconnect/how-to/partner/configuring-onprem-routers)

