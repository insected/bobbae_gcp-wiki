


[GCP compute stack](  https://cloud.google.com/products/compute )  contains, Google [Compute Engine](https://cloud.google.com/compute) (GCE), [Google Kubernetes Engine](   GKE) (formerly Container Engine) (GKE), [Google App Engine](App-Engine) (GAE) and [Google Cloud Functions](  https://cloud.google.com/functions) (GCF). [There are  hosting options](  https://cloud.google.com/hosting-options ) that address different requirements. 







<img src="https://cloudx-bricks-prod-bucket.storage.googleapis.com/d5c9cad33f729dc110d8b907db5a695ca9cf6b0f4b692f44f0f2c0e276d78369.svg" width="800">

## From Data Center Professional Point of view

Typically, [data centers use server virtualization](  https://cloud.google.com/docs/compare/data-centers/compute ), in which multiple virtual Unix/Linux or Windows servers can be run on a single physical machine. These [virtual machines](VM) are created, provisioned, and managed through a software suite such as VMware [vSphere](https://www.vmware.com/products/vsphere-hypervisor.html) or [XenCenter](https://docs.citrix.com/en-us/xencenter.html).

[Compute Engine](   https://youtu.be/KBeyQHoAcrQ ) uses this model as well, combining server virtualization and related management tools into an integrated suite. On Compute Engine, virtual machines are called [virtual machine](  VM ) (VM) instances.




### Compute Engine

[Compute Engine](  https://cloud.google.com/compute/docs  ) lets you create and run virtual machines on Google infrastructure. [Compute Engine offers scale](  https://cloud.google.com/compute/docs/tutorials  ), performance, and value that lets you easily launch large compute clusters on [Google's infrastructure](  https://en.wikipedia.org/wiki/Google_Compute_Engine ). 



## Quickstart using a Linux VM

https://cloud.google.com/compute/docs/quickstart-linux


## How to create a VM on GCP

[https://www.youtube.com/watch?v=1FpMe8na64A](https://www.youtube.com/watch?v=1FpMe8na64A)

https://cloud.google.com/compute/docs/instances/create-start-instance

### Preemptible VM


A preemptible instance is an instance you can create and run at a much lower price than normal instances. However, Compute Engine might stop (preempt) these instances if it requires access to those resources for other tasks. Preemptible instances will always stop after 24 hours. 

https://cloud.google.com/compute/docs/instances/create-start-preemptible-instance


## Creating machine images

[https://cloud.google.com/compute/docs/machine-images/create-machine-images](https://cloud.google.com/compute/docs/machine-images/create-machine-images)


## Adding & Resizing Persistent Disks.

[https://cloud.google.com/compute/docs/disks/add-persistent-disk](https://cloud.google.com/compute/docs/disks/add-persistent-disk)

### Creating customized boot disks

https://cloud.google.com/compute/docs/disks/create-root-persistent-disks

### Detach and reattach boot disks

https://cloud.google.com/compute/docs/disks/detach-reattach-boot-disk


### Slurm-GCP

https://cloud.google.com/compute/docs/instances/create-intel-select-solution-hpc-clusters#create_intel_select_solution_verified_clusters_using_slurm-gcp

https://github.com/schedmd/slurm-gcp/tree/intel-select

## Public & Custom Images

[https://cloud.google.com/compute/docs/images/](https://cloud.google.com/compute/docs/images/)


##### Instance Templates & Groups

[https://cloud.google.com/compute/docs/instance-templates](https://cloud.google.com/compute/docs/instance-templates)


##### Compute Engine AIM roles and permissions

[https://cloud.google.com/compute/docs/access/iam](https://cloud.google.com/compute/docs/access/iam)


##### SSH connections to Linux VMs

[https://cloud.google.com/compute/docs/instances/ssh](https://cloud.google.com/compute/docs/instances/ssh)


## Securely connecting to VMs

[https://cloud.google.com/solutions/connecting-securely](https://cloud.google.com/solutions/connecting-securely)


## Operating System Details

[https://cloud.google.com/compute/docs/images/os-details](https://cloud.google.com/compute/docs/images/os-details)


## Managing SSH keys

[https://cloud.google.com/compute/docs/instances/adding-removing-ssh-keys](https://cloud.google.com/compute/docs/instances/adding-removing-ssh-keys)

### SSH protocol and public key authentication method

https://www.ssh.com/academy/ssh/public-key-authentication

### PKI

https://www.ssh.com/academy/pki

### Creating snapshots

[https://cloud.google.com/compute/docs/disks/create-snapshots](https://cloud.google.com/compute/docs/disks/create-snapshots)


## Best Practices

[https://cloud.google.com/compute/docs/disks/snapshot-best-practices](https://cloud.google.com/compute/docs/disks/snapshot-best-practices)


## Linux Command Cheat Sheet

[https://www.linuxtrainingacademy.com/linux-commands-cheat-sheet/](https://www.linuxtrainingacademy.com/linux-commands-cheat-sheet/)


## Firewall Rules

Each [firewall](  https://cloud.google.com/vpc/docs/firewalls ) rule applies to incoming (ingress) or outgoing (egress) connection, not both. [Firewall rules](   https://www.youtube.com/watch?v=HTVV9YzGw5k ) only support IPv4 connections. Each firewall rule's action is either allow or deny . When you create a firewall rule, you must select a VPC network.






### Using Network tags

[https://cloud.google.com/vpc/docs/add-remove-network-tags](https://cloud.google.com/vpc/docs/add-remove-network-tags)


#### Machine Types

A [machine type](  https://cloud.google.com/compute/docs/machine-types ) is a set of virtualized hardware resources available to a virtual machine (VM) instance, including the system memory size, virtual CPU (vCPU) count, and persistent disk limits. In Compute Engine, machine types are grouped and curated by families for different workloads. You can choose from general-purpose, memory-optimized, and compute-optimized families. You must choose a machine type when you [create an instance](https://cloud.google.com/compute/docs/instances/creating-and-starting-an-instance?hl=tr). You can select from a number of predefined machine types in each machine type family. If the predefined machine types do not meet your needs, you can create your own [custom machine types](https://cloud.google.com/compute/docs/machine-types?hl=tr#custom_machine_types). To compare machine type performance, see [CPU platforms](https://cloud.google.com/compute/docs/cpu-platforms?hl=tr).



The E2 machines are lower-cost general purpose, N2, N2D, N1 are also general purpose but balanced price / performance, M2, M1 are memory optimized and C2 are compute optimized.


## Windows VM Instances


### Creating Windows Server Failover Clustering

[https://cloud.google.com/compute/docs/tutorials/running-windows-server-failover-clustering](https://cloud.google.com/compute/docs/tutorials/running-windows-server-failover-clustering)


### Creating Disaster Recovery Plan for SQL Server

[https://cloud.google.com/solutions/sql-server-disaster-recovery-plan-compute-engine](https://cloud.google.com/solutions/sql-server-disaster-recovery-plan-compute-engine)


### Performing an automated in-place upgrade

[https://cloud.google.com/compute/docs/tutorials/performing-an-automated-in-place-upgrade-windows-server](https://cloud.google.com/compute/docs/tutorials/performing-an-automated-in-place-upgrade-windows-server)


### Where to run my code? Deciding between GCE, GKE, App Engine

https://www.youtube.com/watch?v=2tLXKCgqwLY


## Qwiklabs


[Getting Started: Create and Manage Cloud Resources](https://www.qwiklabs.com/quests/120?catalog_rank=%7B%22rank%22%3A4%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&search_id=7467866)


[Hosting a Web App on Google Cloud Using Compute Engine](https://www.qwiklabs.com/focuses/11952?catalog_rank=%7B%22rank%22%3A26%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&parent=catalog&search_id=7467972)


[Build a Website on Google Cloud](https://www.qwiklabs.com/quests/115?catalog_rank=%7B%22rank%22%3A1%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&search_id=7467892)


[VM Migration: Planning](https://www.qwiklabs.com/focuses/6899?catalog_rank=%7B%22rank%22%3A5%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&parent=catalog&search_id=7467835)

[VM Migration: Assessment](https://www.qwiklabs.com/focuses/6896?catalog_rank=%7B%22rank%22%3A8%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&parent=catalog&search_id=7467835)


[Cloud Development](https://www.qwiklabs.com/quests/67?catalog_rank=%7B%22rank%22%3A6%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&search_id=7467936)

