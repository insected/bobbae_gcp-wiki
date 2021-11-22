
Google Cloud [Virtual Private Cloud](https://cloud.google.com/vpc/docs) (VPC) provides networking functionality to Compute Engine virtual machine (VM) instances, Google Kubernetes Engine (GKE) containers, and the App Engine flexible environment. 

VPC provides networking for your cloud-based services that is global, scalable, and flexible.



[https://www.youtube.com/watch?v=wmP6SQe5J7g](https://www.youtube.com/watch?v=wmP6SQe5J7g)

Google Cloud Virtual Private Cloud (VPC) Network Peering allows private connectivity across two VPC networks regardless of whether or not they belong to the same project or the same organization.

[VPC networks](https://cloud.google.com/vpc/docs/advanced-vpc) use Linux's [VIRTIO network module](http://dl.acm.org/citation.cfm?id=1400097.1400108) to model Ethernet card and router functionality, but higher levels of the networking stack, such as ARP lookups, are handled using standard networking software.

A Virtual Private Cloud (VPC) network is a virtual version of a physical network, [implemented inside of Google's production network, using Andromeda](https://cloud.google.com/vpc/docs/vpc).

Cloud Platform firewalls, routing, and forwarding rules all leverage the underlying internal [Andromeda]( https://cloud.google.com/blog/products/gcp/enter-andromeda-zone-google-cloud-platforms-latest-networking-stack) APIs and infrastructure.



## Migrate from on-prem to cloud using VPC

[https://www.youtube.com/watch?v=cNb7xKyya5c](https://www.youtube.com/watch?v=cNb7xKyya5c)



## Shared VPC and VPC Peering

[Shared VPC](https://cloud.google.com/vpc/docs/shared-vpc) allows an  [organization](https://cloud.google.com/resource-manager/docs/cloud-platform-resource-hierarchy) to connect resources from multiple projects to a common [Virtual Private Cloud (VPC) network](https://cloud.google.com/vpc/docs/vpc), so that they can communicate with each other securely and efficiently using internal IPs from that network. When you use Shared VPC, you designate a project as a host project and attach one or more other service projects to it. 

The VPC networks in the host project are called Shared VPC networks. [Eligible resources](https://cloud.google.com/vpc/docs/shared-vpc#resources_that_can_be_attached_to_shared_vpc_networks_from_a_service_project) from service projects can use subnets in the Shared VPC network.

Shared VPC lets [organization administrators](https://cloud.google.com/resource-manager/docs/cloud-platform-resource-hierarchy#organizations) delegate administrative responsibilities, such as creating and managing instances, to [Service Project Admins](https://cloud.google.com/vpc/docs/shared-vpc#iam_in_shared_vpc) while maintaining centralized control over network resources like subnets, routes, and firewalls.

Google Cloud VPC Network Peering allows [internal IP address](https://cloud.google.com/vpc/docs/ip-addresses) connectivity across two Virtual Private Cloud (VPC) networks regardless of whether they belong to the same project or the same organization.

[VPC Network Peering](https://cloud.google.com/vpc/docs/vpc-peering) enables you to connect VPC networks so that workloads in different VPC networks can communicate internally. Traffic stays within Google's network and doesn't traverse the public internet.



https://medium.com/google-cloud/everything-you-always-wanted-to-know-about-vpc-peering-but-were-afraid-to-ask-2b26267ba7d9

## VPC network Sharing and Peering

[Shared VPC](https://cloud.google.com/vpc/docs/how-to#vpc-network-sharing-and-peering) allows you to export subnets from a [VPC network](https://cloud.google.com/vpc/docs/vpc) in a host project to other service projects in the same [organization](https://cloud.google.com/resource-manager/docs/creating-managing-organization). Instances in the service projects can have network connections in the shared subnets of the host project. 

## VPC Service Controls


[VPC Service Controls](https://cloud.google.com/vpc-service-controls) improves your ability to mitigate the risk of data exfiltration from Google Cloud services such as Cloud Storage and BigQuery. You can use VPC Service Controls to create perimeters that protect the resources and data of services that you explicitly specify.

https://blog.scalesec.com/vpc-service-controls-in-plain-english-a5ce9779393e

VPC Service Controls provides an extra layer of security defense for Google Cloud services that is independent of Identity and Access Management (IAM). While [IAM](IAM) enables granular identity-based access control, VPC Service Controls enables broader context-based perimeter security, including controlling data egress across the perimeter. We recommend using both VPC Service Controls and IAM for defense in depth.


https://cloud.google.com/vpc-service-controls/docs/overview

## Private Google Access

VM instances that only have internal IP addresses (no external IP addresses) can use Private Google Access. They can reach the external IP addresses of Google APIs and services. The source IP address of the packet can be the primary internal IP address of the network interface or an address in an alias IP range that is assigned to the interface. If you disable Private Google Access, the VM instances can no longer reach Google APIs and services; they can only send traffic within the VPC network.

https://cloud.google.com/vpc/docs/private-google-access

### Private Service Connect 

https://faun.pub/private-service-connect-to-connect-privately-with-google-apis-and-services-e91da2f26a7a

https://cloud.google.com/vpc/docs/private-service-connect

https://medium.com/google-cloud/exposing-the-client-behind-psc-2471a851ae23
