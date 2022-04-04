A [virtual machine](https://en.wikipedia.org/wiki/Virtual_machine) (VM) is an [emulation](https://en.wikipedia.org/wiki/Emulator) of a computer system. Virtual machines are based on [computer architectures](https://en.wikipedia.org/wiki/Computer_architectures) and provide the functionality of a physical computer. Their implementations may involve specialized hardware, software, or a combination. A VM is a kind of [hypervisor](hypervisor). The [distinction](https://en.wikipedia.org/wiki/Hypervisor#Classification) between [Type-1 and Type-2](https://medium.com/teamresellerclub/type-1-and-type-2-hypervisors-what-makes-them-different-6a1755d6ae2c) hypervisor can sometimes be not clear. 
 
[https://www.youtube.com/watch?v=VtXNIy_noWg](https://www.youtube.com/watch?v=VtXNIy_noWg)

## GCE

Google Compute Engine is computing and hosting service that lets you create and run virtual machines on Google infrastructure.

### Create and start VMs
https://cloud.google.com/compute/docs/instances/create-start-instance

### HPC-ready VMs
https://cloud.google.com/compute/docs/instances/create-hpc-vm

### Instance templates
https://cloud.google.com/compute/docs/instances/create-vm-from-instance-template

### Sole-tenant VMs
https://cloud.google.com/compute/docs/nodes/sole-tenant-nodes

### Nested virtualization
https://cloud.google.com/compute/docs/instances/nested-virtualization/overview

### Virtual displays
https://cloud.google.com/compute/docs/instances/enable-instance-virtual-display

### VM Disks

https://cloud.google.com/compute/docs/disks

#### Boot disks
https://cloud.google.com/compute/docs/disks/detach-reattach-boot-disk



### VM Migration
https://cloud.google.com/compute/docs/import

### Securly connecting to VMs

https://cloud.google.com/solutions/connecting-securely

### Google Compute Engine and KVM

[Google Compute Engine](Compute) uses KVM as the hypervisor.
The [KVM](https://en.wikipedia.org/wiki/Kernel-based_Virtual_Machine) may be categorized as both Type-1 and Type-2.


### Suspending VMs

https://cloud.google.com/compute/docs/instances/suspend-resume-instance
 

### Machine images
https://cloud.google.com/compute/docs/machine-images

### Back up disks

#### Snapshot
https://cloud.google.com/compute/docs/disks/snapshots

#### Restoring from backup
https://cloud.google.com/compute/docs/machine-images/create-instance-from-machine-image

### Cloud-native vs VM

https://cloud.google.com/blog/topics/developers-practitioners/vms-and-their-relevance-cloud-native-future-conversation

### Virtual Random Number Generator
https://cloud.google.com/compute/docs/instances/enabling-virtio-rng

### Autoscaling groups of instances
https://cloud.google.com/compute/docs/autoscaler

### NTP
https://cloud.google.com/compute/docs/instances/configure-ntp

### VM Instance lifecycle
https://cloud.google.com/compute/docs/instances/instance-life-cycle

### Managed VM instances
https://cloud.google.com/compute/docs/instance-groups/working-with-managed-instances

### Google Cloud metadata server

Google Cloud runs a local metadata server alongside each instance at 169.254.169.254.

https://cloud.google.com/vpc/docs/firewalls#gcp-metadata-server

### Connecting to instances that do not have external IP addresses

https://cloud.google.com/compute/docs/instances/connecting-advanced#sshbetweeninstances

### Tau VMs

https://cloud.google.com/blog/products/compute/google-cloud-introduces-tau-vms

### Spot VMs

https://cloud.google.com/kubernetes-engine/docs/concepts/spot-vms

#### Run Fault-tolerant workload on Spot VMs

https://cloud.google.com/blog/products/compute/google-cloud-spot-vm

## Virtual Machine related topics

### Intel VT-x and AMD SVM


https://www.anandtech.com/show/2480/9


### Firecracker microVM

https://firecracker-microvm.github.io/

### Containers
https://www.ibm.com/cloud/blog/containers-vs-vms

### UniK and unikernels

https://github.com/solo-io/unik


## Examples


https://cloud.google.com/compute/docs/tutorials

### Running Apache server on GCE VM

https://cloud.google.com/compute/docs/tutorials/basic-webserver-apache

### Running Discord bot on GCE VM

https://cloud.google.com/blog/topics/developers-practitioners/build-and-run-discord-bot-top-google-cloud

### Migration Amazon Linux instances using Migrate for Compute Engine

https://taneli-leppa.medium.com/migrating-amazon-linux-instances-using-migrate-for-compute-engine-b2392c97cda6