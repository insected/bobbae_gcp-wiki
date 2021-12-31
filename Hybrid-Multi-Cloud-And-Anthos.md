

[Anthos](Anthos) is a modern application management platform that provides a consistent development and operations experience for cloud and on-premises environments. 



## Multi Cloud

Enterprises require multi-cloud solutions for their critical workloads. This strategy requires them to build workloads that are portable across architectures.

https://cloud.netapp.com/blog/gcp-cvo-blg-google-anthos-the-first-true-multi-cloud-platform

## Edge computing

https://cloud.google.com/blog/topics/hybrid-cloud/edge-computing-architectural-challenges-and-pitfalls


## Anthos vs AWS Outposts vs Azure Stack

The [AWS Outposts](https://aws.amazon.com/outposts/), Anthos and [Azure Stack](https://azure.microsoft.com/en-us/overview/azure-stack/) have different goals and characteristics. Each has [a unique approach](https://www.bizety.com/2020/06/28/aws-outposts-google-anthos-gke-and-azure-on-prem-overview/) to solving
the hybrid multi cloud issues.



### AWS Outposts

[AWS Outposts](https://aws.amazon.com/outposts/) is a  managed service that offers the same AWS infrastructure, AWS services, APIs, and tools to virtually any datacenter, co-location space, or on-premises facility for a  consistent hybrid experience. 

Outposts is available as a 42U rack that can scale from [1 rack to 96 racks](  https://aws.amazon.com/outposts/1u-2u/ ) to create pools of compute and storage capacity. 

### Azure Stack


[Azure Stack](https://azure.microsoft.com/en-us/overview/azure-stack/) allows you to extend Azure services and capabilities from the datacenter to [edge locations and remote offices](https://docs.microsoft.com/en-us/azure-stack/hci/concepts/system-requirements).

#### Azure Stack Hub

https://azure.microsoft.com/en-us/products/azure-stack/hub/

### How is Anthos approach different than AWS Output or Azure Stack

https://www.computerworld.com/article/3428108/the-major-hybrid-cloud-options-compared-aws-outposts-vs-azure-stack-vs-google-anthos.html


#### Azure Stack approach

[Azure Stack](https://azure.microsoft.com/en-us/overview/azure-stack/) is Azure cloud brought into an organization's own data center.  Azure Stack is running  Hyper-V, Windows networking and storage on hardware from HPE, DELL, Cisco, Huawei and Lenovo. You can license Azure Stack and purchase your own hardware to install onto it.


#### AWS Outposts approach

[AWS](AWS) delivers pre-configured hardware and software to the customer data center or co-location space.  You can run [VMware Cloud on AWS](https://www.vmware.com/products/vmc-on-aws.html) or run compute and storage on-premises using native AWS APIs used in the AWS cloud. Users can configure outposts with EC2 instances and EBS. It supports EKS, EMR, RDS, SageMaker and AWS MSK.

#### Oracle Cloud at Customer approach

In Oracle's approach, SaaS, CRM, ERP and HCM products are brought into customer's own data centers. Oracle provides converged Oracle hardware, software and management services to run applications using customer's data center, networking and power.


#### Anthos approach

[Anthos](Anthos) is a combination of GKE on-prem and Anthos Config Management console.  It is hardware agnostic and can be run on existing servers or with VMWare, Dell, HPE, Intel and Lenovo racks.  This approach relies on Kubernetes as a kind of portability layer over multiple clouds, as Anthos can run on AWS and Azure.   It has similarities to [Tanzu](https://tanzu.vmware.com/tanzu) and [Openshift](https://www.redhat.com/en/technologies/cloud-computing/openshift).

## OCP

The [Open Compute Project](https://www.opencompute.org/) (OCP) is a collaborative community focused on redesigning hardware technology to efficiently support the growing demands on compute infrastructure. 




## Collie

[Collie](https://github.com/meshcloud/collie-cli) helps you get an overview over multiple cloud accounts.

## Kubernetes based multi cloud

https://medium.datadriveninvestor.com/a-multi-cloud-and-multi-cluster-architecture-with-kubernetes-cb3abe554948

### Kubernetes portability

https://diginomica.com/kubernetes-and-misconception-multi-cloud-portability

### D2IQ DKP

https://d2iq.com/kubernetes-platform

### Kosmos

https://blog.scaleway.com/k8s-multi-cloud/

### Platform 9

https://platform9.com/

### Rancher

https://rancher.com/

### Openshift

https://openshift.com
