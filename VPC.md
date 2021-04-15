

# Introduction

Google Cloud Virtual Private Cloud (VPC) provides networking functionality to Compute Engine virtual machine (VM) instances, Google Kubernetes Engine (GKE) containers, and the App Engine flexible environment. VPC provides networking for your cloud-based services that is global, scalable, and flexible.

[https://cloud.google.com/vpc/docs](https://cloud.google.com/vpc/docs)


# Migrate from on-prem to cloud using VPC

[https://www.youtube.com/watch?v=cNb7xKyya5c](https://www.youtube.com/watch?v=cNb7xKyya5c)


# VPC Deep Dive

[https://www.youtube.com/watch?v=wmP6SQe5J7g](https://www.youtube.com/watch?v=wmP6SQe5J7g)

Google Cloud Virtual Private Cloud (VPC) Network Peering allows private connectivity across two VPC networks regardless of whether or not they belong to the same project or the same organization.

VPC networks use Linux's [VIRTIO network module](http://dl.acm.org/citation.cfm?id=1400097.1400108) to model Ethernet card and router functionality, but higher levels of the networking stack, such as ARP lookups, are handled using standard networking software.

[https://cloud.google.com/vpc/docs/advanced-vpc](https://cloud.google.com/vpc/docs/advanced-vpc)


# Shared VPC and VPC Peering

[Shared VPC](https://cloud.google.com/vpc/docs/shared-vpc) allows an  [organization](https://cloud.google.com/resource-manager/docs/cloud-platform-resource-hierarchy) to connect resources from multiple projects to a common [Virtual Private Cloud (VPC) network](https://cloud.google.com/vpc/docs/vpc), so that they can communicate with each other securely and efficiently using internal IPs from that network. When you use Shared VPC, you designate a project as a host project and attach one or more other service projects to it. The VPC networks in the host project are called Shared VPC networks. [Eligible resources](https://cloud.google.com/vpc/docs/shared-vpc#resources_that_can_be_attached_to_shared_vpc_networks_from_a_service_project) from service projects can use subnets in the Shared VPC network.

Shared VPC lets [organization administrators](https://cloud.google.com/resource-manager/docs/cloud-platform-resource-hierarchy#organizations) delegate administrative responsibilities, such as creating and managing instances, to [Service Project Admins](https://cloud.google.com/vpc/docs/shared-vpc#iam_in_shared_vpc) while maintaining centralized control over network resources like subnets, routes, and firewalls.

Google Cloud VPC Network Peering allows [internal IP address](https://cloud.google.com/vpc/docs/ip-addresses) connectivity across two Virtual Private Cloud (VPC) networks regardless of whether they belong to the same project or the same organization.

[VPC Network Peering](https://cloud.google.com/vpc/docs/vpc-peering) enables you to connect VPC networks so that workloads in different VPC networks can communicate internally. Traffic stays within Google's network and doesn't traverse the public internet.

[https://cloud.google.com/vpc/docs/vpc-peering](https://cloud.google.com/vpc/docs/vpc-peering)


# VPC network Sharing and Peering

Shared VPC allows you to export subnets from a [VPC network](https://cloud.google.com/vpc/docs/vpc) in a host project to other service projects in the same [organization](https://cloud.google.com/resource-manager/docs/creating-managing-organization). Instances in the service projects can have network connections in the shared subnets of the host project. 

[https://cloud.google.com/vpc/docs/how-to#vpc-network-sharing-and-peering](https://cloud.google.com/vpc/docs/how-to#vpc-network-sharing-and-peering)

