

## Compute

### Introduction 

GCP compute stack that contains, Google Compute Engine (GCE), Google Kubernetes Engine (formerly Container Engine) (GKE), Google App Engine (GAE) and Google Cloud Functions (GCF).

[https://cloud.google.com/products/compute](https://cloud.google.com/products/compute)

[https://cloud.google.com/hosting-options](https://cloud.google.com/hosting-options)

[[https://cloudx-bricks-prod-bucket.storage.googleapis.com/2d5d0c50a9b20c435977d09ce20c29e6e926f626f198c5a14670f43924a74402.svg]]


#### From Data Center Professional Point of view

Typically, data centers use server virtualization, in which multiple virtual Unix/Linux or Windows servers can be run on a single physical machine. These virtual machines are created, provisioned, and managed through a software suite such as VMware vSphere or XenCenter.

Compute Engine uses this model as well, combining server virtualization and related management tools into an integrated suite. On Compute Engine, virtual machines are called virtual machine (VM) instances

https://cloud.google.com/docs/compare/data-centers/compute


### Compute Engine

Compute Engine lets you create and run virtual machines on Google infrastructure. Compute Engine offers scale, performance, and value that lets you easily launch large compute clusters on Google's infrastructure. There are no upfront investments, and you can run thousands of virtual CPUs on a system that offers quick, consistent performance.

[https://cloud.google.com/compute/docs](https://cloud.google.com/compute/docs)

[https://cloud.google.com/compute/docs/tutorials](https://cloud.google.com/compute/docs/tutorials)


#### VM

A virtual machine (VM) is an [emulation](https://en.wikipedia.org/wiki/Emulator) of a computer system. Virtual machines are based on [computer architectures](https://en.wikipedia.org/wiki/Computer_architectures) and provide functionality of a physical computer. Their implementations may involve specialized hardware, software, or a combination. A VM is a kind of [hypervisor](https://en.wikipedia.org/wiki/Hypervisor). The [distinction](https://en.wikipedia.org/wiki/Hypervisor#Classification) between Type-1 and Type-2 hypervisor can sometimes be not clear. For example, [KVM](https://en.wikipedia.org/wiki/Kernel-based_Virtual_Machine) may be categorized as both.  It is possible to run [nested VM](https://cloud.google.com/compute/docs/instances/enable-nested-virtualization-vm-instances) instances in GCP.

[https://www.youtube.com/watch?v=VtXNIy_noWg](https://www.youtube.com/watch?v=VtXNIy_noWg)


##### How to create a VM on GCP

[https://www.youtube.com/watch?v=1FpMe8na64A](https://www.youtube.com/watch?v=1FpMe8na64A)


##### Creating machine images

[https://cloud.google.com/compute/docs/machine-images/create-machine-images](https://cloud.google.com/compute/docs/machine-images/create-machine-images)


##### Adding & Resizing Persistent Disks.

[https://cloud.google.com/compute/docs/disks/add-persistent-disk](https://cloud.google.com/compute/docs/disks/add-persistent-disk)


##### Public & Custom Images

[https://cloud.google.com/compute/docs/images/](https://cloud.google.com/compute/docs/images/)


##### Instance Templates & Groups

[https://cloud.google.com/compute/docs/instance-templates](https://cloud.google.com/compute/docs/instance-templates)


##### Compute Engine AIM roles and permissions

[https://cloud.google.com/compute/docs/access/iam](https://cloud.google.com/compute/docs/access/iam)


##### SSH connections to Linux VMs

[https://cloud.google.com/compute/docs/instances/ssh](https://cloud.google.com/compute/docs/instances/ssh)


##### Securely connecting to VMs

[https://cloud.google.com/solutions/connecting-securely](https://cloud.google.com/solutions/connecting-securely)


##### Operating System Details

[https://cloud.google.com/compute/docs/images/os-details](https://cloud.google.com/compute/docs/images/os-details)


##### Managing SSH keys

[https://cloud.google.com/compute/docs/instances/adding-removing-ssh-keys](https://cloud.google.com/compute/docs/instances/adding-removing-ssh-keys)


#### Snapshots


##### Creating snapshots

[https://cloud.google.com/compute/docs/disks/create-snapshots](https://cloud.google.com/compute/docs/disks/create-snapshots)


##### Best Practices

[https://cloud.google.com/compute/docs/disks/snapshot-best-practices](https://cloud.google.com/compute/docs/disks/snapshot-best-practices)


#### Linux Command Cheat Sheet

[https://www.linuxtrainingacademy.com/linux-commands-cheat-sheet/](https://www.linuxtrainingacademy.com/linux-commands-cheat-sheet/)


#### Firewall Rules

Each firewall rule applies to incoming (ingress) or outgoing (egress) connection, not both. Firewall rules only support IPv4 connections. Each firewall rule's action is either allow or deny . When you create a firewall rule, you must select a VPC network.

[https://cloud.google.com/vpc/docs/firewalls](https://cloud.google.com/vpc/docs/firewalls)

[https://www.youtube.com/watch?v=HTVV9YzGw5k](https://www.youtube.com/watch?v=HTVV9YzGw5k)


##### Using Network tags

[https://cloud.google.com/vpc/docs/add-remove-network-tags](https://cloud.google.com/vpc/docs/add-remove-network-tags)


#### Machine Types

A machine type is a set of virtualized hardware resources available to a virtual machine (VM) instance, including the system memory size, virtual CPU (vCPU) count, and persistent disk limits. In Compute Engine, machine types are grouped and curated by families for different workloads. You can choose from general-purpose, memory-optimized, and compute-optimized families. You must choose a machine type when you [create an instance](https://cloud.google.com/compute/docs/instances/creating-and-starting-an-instance?hl=tr). You can select from a number of predefined machine types in each machine type family. If the predefined machine types do not meet your needs, you can create your own [custom machine types](https://cloud.google.com/compute/docs/machine-types?hl=tr#custom_machine_types). To compare machine type performance, see [CPU platforms](https://cloud.google.com/compute/docs/cpu-platforms?hl=tr).

[https://cloud.google.com/compute/docs/machine-types](https://cloud.google.com/compute/docs/machine-types?hl=tr)

The E2 machines are lower-cost general purpose, N2, N2D, N1 are also general purpose but balanced price / performance, M2, M1 are memory optimized and C2 are compute optimized.


#### Windows


##### Creating Windows Server Failover Clustering

[https://cloud.google.com/compute/docs/tutorials/running-windows-server-failover-clustering](https://cloud.google.com/compute/docs/tutorials/running-windows-server-failover-clustering)


##### Creating Disaster Recovery Plan for SQL Server

[https://cloud.google.com/solutions/sql-server-disaster-recovery-plan-compute-engine](https://cloud.google.com/solutions/sql-server-disaster-recovery-plan-compute-engine)


##### Performing an automated in-place upgrade

[https://cloud.google.com/compute/docs/tutorials/performing-an-automated-in-place-upgrade-windows-server](https://cloud.google.com/compute/docs/tutorials/performing-an-automated-in-place-upgrade-windows-server)


#### Qwiklabs


##### Getting Started

In this introductory-level Quest, you will get hands-on practice with Google Cloud’s fundamental tools and services. Getting Started: Create and Manage Cloud Resources is the recommended first Quest for the Google Cloud learner - you will come in with little or no prior cloud knowledge, and come out with practical experience that you can apply to your first Google Cloud project. From writing Cloud Shell commands and deploying your first virtual machine, to running applications on Kubernetes Engine or with load balancing, Getting Started: Create and Manage Cloud Resources is a prime introduction to the basic features of Google Cloud. 

[Getting Started: Create and Manage Cloud Resources](https://www.qwiklabs.com/quests/120?catalog_rank=%7B%22rank%22%3A4%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&search_id=7467866)


##### Hosting a Web App on GCP

There are many ways to deploy web sites within Google Cloud with each solution offering different features, capabilities, and levels of control. Compute Engine offers a deep level of control over the infrastructure used to run a web site, but also requires a little more operational management compared to solutions like Google Kubernetes Engines (GKE), App Engine, or others. With Compute Engine, you have fine-grained control of aspects of the infrastructure, including the virtual machines, load balancers, and more. In this lab you will deploy a sample application, the "Fancy Store" ecommerce website, to show how a website can be deployed and scaled easily with Compute Engine.

[Hosting a Web App on Google Cloud Using Compute Engine](https://www.qwiklabs.com/focuses/11952?catalog_rank=%7B%22rank%22%3A26%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&parent=catalog&search_id=7467972)


##### Build a Website on GCP

In this quest you will learn about the 4 Google Cloud website architectures available to ensure that your website is available and scalable. This quest is based on the video series [Get Cooking in Cloud](https://www.youtube.com/watch?v=pxp7uYUjH_M).

[Build a Website on Google Cloud](https://www.qwiklabs.com/quests/115?catalog_rank=%7B%22rank%22%3A1%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&search_id=7467892)


##### Planning VM migration

This lab focuses on the “Plan” phase and how to deploy your basic infrastructure on GCP. [Terraform](https://www.terraform.io/) is a popular open-source tool for defining and provisioning infrastructure (Infrastructure as Code). In this lab, you'll leverage pre-built Infrastructure as Code templates to setup a cloud network, configure access, and deploy your first application—all in a secure and automated fashion.

[VM Migration: Planning](https://www.qwiklabs.com/focuses/6899?catalog_rank=%7B%22rank%22%3A5%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&parent=catalog&search_id=7467835)


##### VM Migration Assessment

This lab focuses on the “Assess” phase using [CloudPhysics](https://www.cloudphysics.com/).

[VM Migration: Assessment](https://www.qwiklabs.com/focuses/6896?catalog_rank=%7B%22rank%22%3A8%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&parent=catalog&search_id=7467835)


##### Cloud Development 

The hands-on labs in this Quest are structured to give experienced app developers hands-on practice with the state-of-the-art developing applications in Google Cloud. The topics align with the [Google Cloud Certified Professional Cloud Developer](https://cloud.google.com/certification/cloud-developer) Certification. These labs follow the sequence of activities needed to create and deploy an app in GCP from beginning to end. Labs in the sequence with application code are presented in two language flavors, Java and Python. 

[Cloud Development](https://www.qwiklabs.com/quests/67?catalog_rank=%7B%22rank%22%3A6%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&search_id=7467936)

