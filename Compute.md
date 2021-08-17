


[GCP compute stack](  https://cloud.google.com/products/compute )  contains, Google [Compute Engine](https://cloud.google.com/compute) (GCE), [Google Kubernetes Engine](   GKE) (formerly Container Engine) (GKE), [Google App Engine](App-Engine) (GAE) and [Google Cloud Functions](  https://cloud.google.com/functions) (GCF). 


There are  many [hosting options](  https://cloud.google.com/hosting-options ) that address different requirements. 





## Concepts

https://cloud.google.com/compute/docs/concepts

## Regions and Zones

https://cloud.google.com/compute/docs/regions-zones

## Google Compute Engine How-to guides

https://cloud.google.com/compute/docs/how-to

## Reserving Zonal Resources

https://cloud.google.com/compute/docs/instances/reservations-overview

## Machine Types

A [machine type](  https://cloud.google.com/compute/docs/machine-types ) is a set of virtualized hardware resources available to a virtual machine (VM) instance, including the system memory size, virtual CPU (vCPU) count, and persistent disk limits. In Compute Engine, machine types are grouped and curated by families for different workloads. You can choose from general-purpose, memory-optimized, and compute-optimized families. You must choose a machine type when you [create an instance](https://cloud.google.com/compute/docs/instances/creating-and-starting-an-instance?hl=tr). You can select from a number of predefined machine types in each machine type family. If the predefined machine types do not meet your needs, you can create your own [custom machine types](https://cloud.google.com/compute/docs/machine-types?hl=tr#custom_machine_types). To compare machine type performance, see [CPU platforms](https://cloud.google.com/compute/docs/cpu-platforms?hl=tr).



The E2 machines are lower-cost general purpose, N2, N2D, N1 are also general purpose but balanced price / performance, M2, M1 are memory optimized and C2 are compute optimized.
## From Data Center Professional Point of view

Typically, [data centers use server virtualization](  https://cloud.google.com/docs/compare/data-centers/compute ), in which multiple virtual Unix/Linux or Windows servers can be run on a single physical machine. These [virtual machines](VM) are created, provisioned, and managed through a software suite such as VMware [vSphere](https://www.vmware.com/products/vsphere-hypervisor.html) or [XenCenter](https://docs.citrix.com/en-us/xencenter.html).

[Compute Engine](   https://youtu.be/KBeyQHoAcrQ ) uses this model as well, combining server virtualization and related management tools into an integrated suite. On Compute Engine, virtual machines are called [virtual machine](  VM ) (VM) instances.


## Machine Images

https://cloud.google.com/compute/docs/machine-images


## Quickstart using a Linux VM

https://cloud.google.com/compute/docs/quickstart-linux


## How to create a VM on GCP

[https://www.youtube.com/watch?v=1FpMe8na64A](https://www.youtube.com/watch?v=1FpMe8na64A)

https://cloud.google.com/compute/docs/instances/create-start-instance



## Backing up persistent disks using snapshots

https://cloud.google.com/compute/docs/disks/create-snapshots

## Create and Manage custom images

https://cloud.google.com/compute/docs/images/create-delete-deprecate-private-images

## Instance Templates

https://cloud.google.com/compute/docs/instance-templates/create-instance-templates

## Audit Logging

https://cloud.google.com/compute/docs/logging/audit-logging

## Naming Resources

https://cloud.google.com/compute/docs/naming-resources

## Labels

https://cloud.google.com/compute/docs/labeling-resources

## Managing Access to Resources

https://cloud.google.com/compute/docs/access/managing-access-to-resources

## Best Practices

https://cloud.google.com/compute/docs/tutorials/robustsystems


## Sole tenant nodes

Sole-tenancy lets you have exclusive access to a sole-tenant node, which is a physical Compute Engine server that is dedicated to hosting only your project's VMs. Use sole-tenant nodes to keep your VMs physically separated from VMs in other projects, or to group your VMs together on the same host hardware.

https://cloud.google.com/compute/docs/nodes/provisioning-sole-tenant-vms

## Preemptible VM


A preemptible instance is an instance you can create and run at a much lower price than normal instances. However, Compute Engine might stop (preempt) these instances if it requires access to those resources for other tasks. Preemptible instances will always stop after 24 hours. 

https://cloud.google.com/compute/docs/instances/create-start-preemptible-instance

## Reservations

Reservations provide a very high level of assurance in obtaining capacity for Compute Engine zonal resources. For example, use reservations to help ensure that your project has resources for future increases in demand, including: planned or unplanned spikes, migrating a large number of virtual machine (VM) instances, backup and disaster recovery, or planned growth and buffer.

https://cloud.google.com/compute/docs/instances/reservations-overview

## Creating machine images

[https://cloud.google.com/compute/docs/machine-images/create-machine-images](https://cloud.google.com/compute/docs/machine-images/create-machine-images)


## Adding & Resizing Persistent Disks.

[https://cloud.google.com/compute/docs/disks/add-persistent-disk](https://cloud.google.com/compute/docs/disks/add-persistent-disk)

## Creating customized boot disks

https://cloud.google.com/compute/docs/disks/create-root-persistent-disks

## Detach and reattach boot disks

https://cloud.google.com/compute/docs/disks/detach-reattach-boot-disk

## Importing and Exporting VM images

You can share virtual machine (VM) instances, virtual disk files, and machine images from other cloud environments or from your on-premises environment by importing and exporting images from Cloud Storage. 

https://cloud.google.com/compute/docs/import/requirements-export-import-images

## Slurm-GCP

[Slurm](https://slurm.schedmd.com/overview.html) is an open source, fault-tolerant, and highly scalable cluster management and job scheduling system for large and small Linux clusters.

https://cloud.google.com/compute/docs/instances/create-intel-select-solution-hpc-clusters#create_intel_select_solution_verified_clusters_using_slurm-gcp





## Public & Custom Images

[https://cloud.google.com/compute/docs/images/](https://cloud.google.com/compute/docs/images/)



## Instance Groups

A managed instance group (MIG) is a group of virtual machine (VM) instances that you control as a single entity. MIGs support features such as autohealing, load balancing, autoscaling, auto-updating, and stateful workloads.

https://cloud.google.com/compute/docs/instance-groups/creating-groups-of-managed-instances

## Regional MIGs

You can create regional MIGs or zonal MIGs. Regional MIGs provide higher availability compared to zonal MIGs because the instances in a regional MIG are spread across multiple zones in a single region. This document provides information about creating either zonal or regional MIGs. However, regional MIGs have additional options and considerations.

https://cloud.google.com/compute/docs/instance-groups/regional-migs


## Instance Templates & Groups

[https://cloud.google.com/compute/docs/instance-templates](https://cloud.google.com/compute/docs/instance-templates)


## Compute Engine AIM roles and permissions

[https://cloud.google.com/compute/docs/access/iam](https://cloud.google.com/compute/docs/access/iam)

## Operating System Details

[https://cloud.google.com/compute/docs/images/os-details](https://cloud.google.com/compute/docs/images/os-details)


## Securely connecting to VMs

[https://cloud.google.com/solutions/connecting-securely](https://cloud.google.com/solutions/connecting-securely)


## SSH connections to Linux VMs

[https://cloud.google.com/compute/docs/instances/ssh](https://cloud.google.com/compute/docs/instances/ssh)




## Managing SSH keys

[https://cloud.google.com/compute/docs/instances/adding-removing-ssh-keys](https://cloud.google.com/compute/docs/instances/adding-removing-ssh-keys)

## SSH protocol and public key authentication method

https://www.ssh.com/academy/ssh/public-key-authentication

## PKI

https://www.ssh.com/academy/pki


## Creating snapshots

[https://cloud.google.com/compute/docs/disks/create-snapshots](https://cloud.google.com/compute/docs/disks/create-snapshots)


## Best Practices

[https://cloud.google.com/compute/docs/disks/snapshot-best-practices](https://cloud.google.com/compute/docs/disks/snapshot-best-practices)


## Linux Command Cheat Sheet

[https://www.linuxtrainingacademy.com/linux-commands-cheat-sheet/](https://www.linuxtrainingacademy.com/linux-commands-cheat-sheet/)


## Firewall Rules

Each [firewall](  https://cloud.google.com/vpc/docs/firewalls ) rule applies to incoming (ingress) or outgoing (egress) connection, not both. [Firewall rules](   https://www.youtube.com/watch?v=HTVV9YzGw5k ) only support IPv4 connections. Each firewall rule's action is either allow or deny . When you create a firewall rule, you must select a VPC network.






## Using Network tags

[https://cloud.google.com/vpc/docs/add-remove-network-tags](https://cloud.google.com/vpc/docs/add-remove-network-tags)






## TPU Types and Zones


Tensor Processing Units (TPUs) are Google’s custom-developed application-specific integrated circuits (ASICs) used to accelerate machine learning workloads. TPUs are designed from the ground up with the benefit of Google’s deep experience and leadership in machine learning.

https://cloud.google.com/tpu/docs/tpus

Available Zones:

https://cloud.google.com/tpu/docs/types-zones


## GPU

Compute Engine provides graphics processing units (GPUs) that you can add to your virtual machine (VM) instances. You can use these GPUs to accelerate specific workloads on your instances such as machine learning and data processing.

https://cloud.google.com/compute/docs/gpus

Compute Engine provides NVIDIA® GPUs for your instances in passthrough mode so that your virtual machine instances have direct control over the GPUs and their associated memory.


## GPU regions and zones


https://cloud.google.com/compute/docs/gpus/gpu-regions-zones


## Creating VMs with attached GPUs

https://cloud.google.com/compute/docs/gpus/create-vm-with-gpus

## Running TensorFlow inference workloads with TensorRT5 and NVIDIA T4 GPU


https://cloud.google.com/compute/docs/tutorials/ml-inference-t4


## Windows VM Instances


## Creating Windows Server Failover Clustering

[https://cloud.google.com/compute/docs/tutorials/running-windows-server-failover-clustering](https://cloud.google.com/compute/docs/tutorials/running-windows-server-failover-clustering)


## Creating Disaster Recovery Plan for SQL Server

[https://cloud.google.com/solutions/sql-server-disaster-recovery-plan-compute-engine](https://cloud.google.com/solutions/sql-server-disaster-recovery-plan-compute-engine)


## Performing an automated in-place upgrade

[https://cloud.google.com/compute/docs/tutorials/performing-an-automated-in-place-upgrade-windows-server](https://cloud.google.com/compute/docs/tutorials/performing-an-automated-in-place-upgrade-windows-server)



## Where to run my code? Deciding between GCE, GKE, App Engine

https://www.youtube.com/watch?v=2tLXKCgqwLY




VM Manager helps drive efficiency through automation and reduces the operational burden of maintaining these VM fleets.

VM Manager supports projects in [VPC Service Controls](https://cloud.google.com/vpc-service-controls/docs/supported-products#table_vm_manager) service perimeters.

https://cloud.google.com/compute/docs/vm-manager

## IP Addresses

https://cloud.google.com/compute/docs/ip-addresses

## Internal DNS

https://cloud.google.com/compute/docs/internal-dns

## Auto Healing

https://cloud.google.com/compute/docs/tutorials/high-availability-autohealing

## Running a basic Web server Tutorial

https://cloud.google.com/compute/docs/tutorials/basic-webserver-apache



## Google Data Centers

https://www.google.com/about/datacenters/

## GCP Locations

https://www.google.com/about/datacenters/locations/


## Open Compute Project

Open source hardware design for data centers.


https://www.opencompute.org/products

## Tutorials

https://cloud.google.com/compute/docs/tutorials


## Qwiklabs


[Getting Started: Create and Manage Cloud Resources](https://www.qwiklabs.com/quests/120?catalog_rank=%7B%22rank%22%3A4%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&search_id=7467866)


[Hosting a Web App on Google Cloud Using Compute Engine](https://www.qwiklabs.com/focuses/11952?catalog_rank=%7B%22rank%22%3A26%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&parent=catalog&search_id=7467972)


[Build a Website on Google Cloud](https://www.qwiklabs.com/quests/115?catalog_rank=%7B%22rank%22%3A1%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&search_id=7467892)


[VM Migration: Planning](https://www.qwiklabs.com/focuses/6899?catalog_rank=%7B%22rank%22%3A5%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&parent=catalog&search_id=7467835)

[VM Migration: Assessment](https://www.qwiklabs.com/focuses/6896?catalog_rank=%7B%22rank%22%3A8%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&parent=catalog&search_id=7467835)


[Cloud Development](https://www.qwiklabs.com/quests/67?catalog_rank=%7B%22rank%22%3A6%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&search_id=7467936)

