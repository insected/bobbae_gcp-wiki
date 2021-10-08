[VMware]( http://vmware.com/  ) was the first commercially successful company to virtualize the x86 architecture.

VMware's most notable products are its [hypervisors](Hypervisor). VMware became well known for its first type 2 hypervisor known as GSX. This product has since evolved into two hypervisor product lines: VMware's type 1 hypervisors  running directly on hardware and their hosted type 2 hypervisors.

https://www.vmware.com/products.html

## Type 1 Hypervisors

These hypervisors run directly on the host's hardware to control the hardware and to manage guest operating systems. For this reason, they are sometimes called [bare-metal hypervisors](https://www.vmware.com/topics/glossary/content/bare-metal-hypervisor). 

### VMware ESXi

[VMware ESXi](https://en.wikipedia.org/wiki/VMware_ESXi) runs on bare metal unlike other VMware products. It includes its own kernel. In the original VMware ESX, a Linux kernel was started first and then used to load a variety of specialized components, including ESX which served as vmkernel which is a microkernel that runs on bare computer. The vmkernel handles CPU and memory directly using scan-before-execution (SBE) and system resource allocation table (SRAT). ESX is no longer used and ESXi is used instead, which does not include Linux kernel at all.

#### vCenter

[vCenter](https://en.m.wikipedia.org/wiki/VCenter) works with ESX to enable monitoring and management of multiple ESX, ESXi and GSX servers.

### Xen

[Xen](https://en.wikipedia.org/wiki/Xen) hypervisor handles memory management and CPU scheduling of all virtual machines.  The most privileged one is called `dom0` which has access to hardware. From the `dom0` the hypervisor can be managed to launch unprivileged virutal machines called `domU`. Xen offers five approaches to run the guest operating system: hardware virtual machines (HVM), HVM with PV drivers, paravirtualization with full hardware virtualization -- HVM with PVHVM drivers -- PVHVM, PV in an HVM container -- PVH and paravirtualization -- PV.

#### Paravirtualization

[Paravirtualization](https://en.wikipedia.org/wiki/Paravirtualization) is achieved by running a modified operating system which can leverage a special hypercall [ABI](https://en.wikipedia.org/wiki/Application_binary_interface) instead of certain architectural features for better performance.


### Microsoft Hyper-V

[Hyper-V](https://en.wikipedia.org/wiki/Hyper-V) implements isolation of virtual machines in terms of a partition. A partition is a logical unit of isolation, supported by the hypervisor, in which each guest operating system executes.

### z/VM

[z/VM](https://en.wikipedia.org/wiki/Z/VM) is IBM's based on original VM operating systems dating back to 1960s [CP/CMS](https://en.wikipedia.org/wiki/CP/CMS) and [System 360](https://en.wikipedia.org/wiki/IBM_System/360_Model_67).  z/VM runs on IBM's [Z](https://en.wikipedia.org/wiki/IBM_Z) family of computers.


## Type 2 Hypervisors

### VMware Workstation

[VMware Workstation](https://en.wikipedia.org/wiki/VMware_Workstation) is a hosted [hypervisor](hypervisor) that runs on Operating Systems.

### VMware Player

[VMWare Player](https://en.wikipedia.org/wiki/VMware_Workstation_Player) is a virtualization software that runs on Operating Systems and supplied free of charge for non-commercial use.


### QEMU

[QEMU](https://en.wikipedia.org/wiki/QEMU) is an open source [hypervisor](hypervisor) that emulates machine's processor through binary translation and software models of various hardware devices.

### VirtualBox

[VirtualBox](https://en.wikipedia.org/wiki/VirtualBox) is an open source hypervisor that can be installed on many Operating Systems.

## VMware Cloud

https://cloud.google.com/vmware-engine

https://www.vmware.com/products/vmc-on-aws.html
