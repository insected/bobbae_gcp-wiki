

[Anthos](Anthos) is a modern application management platform that provides a consistent development and operations experience for cloud and on-premises environments. 



## Multi Cloud

Enterprises require multi-cloud solutions for their critical workloads. This strategy requires them to build workloads that are portable across architectures.

https://cloud.netapp.com/blog/gcp-cvo-blg-google-anthos-the-first-true-multi-cloud-platform

## Anthos vs AWS Outpost vs Azure Stack

The [AWS Outpost](https://aws.amazon.com/outposts/), Anthos and [Azure Stack](https://azure.microsoft.com/en-us/overview/azure-stack/) have different goals and characteristics. Each has a unique approach to solving
the hybrid multi cloud issues.

https://www.bizety.com/2020/06/28/aws-outposts-google-anthos-gke-and-azure-on-prem-overview/

### AWS Outpost

AWS Outpost is a fully managed service that offers the same AWS infrastructure, AWS services, APIs, and tools to virtually any datacenter, co-location space, or on-premises facility for a truly consistent hybrid experience. 

AWS compute, storage, database, and other services run locally on Outposts, and you can access the full range of AWS services available in the Region to build, manage, and scale your on-premises applications using familiar AWS services and tools.

Outposts is available as a 42U rack that can scale from 1 rack to 96 racks to create pools of compute and storage capacity. 

https://aws.amazon.com/outposts/1u-2u/

### Azure Stack


Azure Stack allows you to extend Azure services and capabilities to your environment of choice—from the datacenter to edge locations and remote offices—with Azure Stack. Build, deploy, and run hybrid and edge computing apps consistently across your IT ecosystem, with flexibility for diverse workloads.

#### Azure Stack Edge

Get rapid insights with an Azure managed appliance using compute and hardware-accelerated machine learning at edge locations for your Internet of Things (IoT) and AI workloads.


#### Azure Stack HCI


Refresh your virtualization host using a hybrid and hyperconverged solution integrated with Azure.

https://docs.microsoft.com/en-us/azure-stack/hci/concepts/system-requirements

#### Azure Stack Hub

Run your own private, autonomous cloud—connected or disconnected with cloud-native apps using consistent Azure services on-premises.

### Discuss the diverse approaches

How is Anthos approach different than AWS Output or Azure Stack.

https://www.computerworld.com/article/3428108/the-major-hybrid-cloud-options-compared-aws-outposts-vs-azure-stack-vs-google-anthos.html


### Azure Stack approach

Azure Stack is Microsoft's Azure cloud brought into an organization's own data center.  Azure Stack is running Microsoft Hyper-V, Windows and Microsoft networking and storage.   Azure Stack can run on qualified hardware from HPE, DELL, Cisco, Huawei and Lenovo. You can license Azure Stack and purchase your own hardware to install onto it.


### AWS Outpost approach

AWS delivers pre-configured hardware and software to the customer data center or co-location space.  You can run VMware Cloud on AWS or run compute and storage on-premises using native AWS APIs used in the AWS cloud. Users can configure outpost with EC2 instances and EBS. It supports EKS, EMR, RDS, SageMaker and AWS MSK.

### Oracle Cloud at Customer approach

In Oracle's approach, SaaS, CRM, ERP and HCM products are brought into customer's own data centers. Oracle provides converged Oracle hardware, software and management services to run applications using customer's data center, networking and power.


### Anthos approach

Anthos is a combination of GKE on-prem and Anthos Config Management console.  It is hardware agnostic and can be run on existing servers or with VMWare, Dell, HPE, Intel and Lenovo racks.  This approach relies on Kubernetes as a kind of portability layer over multiple clouds, as Anthos can run on AWS and Azure.


## OCP

The [Open Compute Project](https://www.opencompute.org/) (OCP) is a collaborative community focused on redesigning hardware technology to efficiently support the growing demands on compute infrastructure. 




## Collie

[Collie](https://github.com/meshcloud/collie-cli) helps you get an overview over multiple cloud accounts.



