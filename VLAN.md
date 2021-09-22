[VLANs](  https://wikipedia.org/wiki/Virtual_LAN ) allow network administrators to group hosts under the same switch or between different switches.

The protocol most commonly used today to support VLANs is [IEEE 802.1Q]( https://wikipedia.org/wiki/IEEE_802.1Q   ).

VLANs work by [applying tags](https://www.firewall.cx/networking-topics/vlan-networks/219-vlan-tagging.html) to network frames and handling these tags in networking systems – creating the appearance and functionality of network traffic that is physically on a single network but acts as if it is split between separate networks. In this way, VLANs can [keep network applications separate](https://en.m.wikipedia.org/wiki/VLAN_Trunking_Protocol) despite being connected to the same physical network, and without requiring multiple sets of cabling and networking devices to be deployed.


## Virtual Networking 


[Network Virtualization](  https://www.vmware.com/topics/glossary/content/network-virtualization ) is a process of logically grouping physical networks and making them operate as single or multiple independent networks called Virtual Networks.

For example, [VMware NSX Data Center](    https://docs.vmware.com/en/VMware-NSX-Data-Center-for-vSphere/index.html  ) is a network virtualization platform that delivers networking and security components like firewalling, switching, and routing that are defined and consumed in software.

Linux also has rich virtual networking capabilities that are used as basis for hosting VMs and containers, as well as cloud environments.  


https://man7.org/linux/man-pages/man8/ip-link.8.html


https://developers.redhat.com/blog/2018/10/22/introduction-to-linux-interfaces-for-virtual-networking

https://liuhangbin.netlify.app/post/virtual-ifaces

https://lloydrochester.com/post/unix/virtual_networking_device_types/

### NFV, VNF, SDN

https://cloudify.co/blog/mobile-world-congress-nfv-sdn-network-orchestration-automation/

## OVS

[Open vSwitch](https://www.openvswitch.org/), sometimes abbreviated as OVS, is an open-source implementation of a distributed virtual multilayer switch. The main purpose of Open vSwitch is to provide a switching stack for hardware virtualization environments, while supporting multiple protocols and standards used in computer networks.

It is designed to enable massive network automation through programmatic extension, while still supporting standard management interfaces and protocols (e.g. NetFlow, sFlow, IPFIX, RSPAN, CLI, LACP, 802.1ag).  In addition, it is designed to support distribution across multiple physical servers similar to VMware's vNetwork distributed vswitch or Cisco's Nexus 1000V. 


## Bridge

A Linux bridge behaves like a network switch. It forwards packets between interfaces that are connected to it. It's usually used for forwarding packets on routers, on gateways, or between VMs and network namespaces on a host. It also supports STP, VLAN filter, and multicast snooping.

https://wiki.linuxfoundation.org/networking/bridge

## Bonding

The Linux bonding driver provides a method for aggregating multiple network interfaces into a single logical "bonded" interface. The behavior of the bonded interface depends on the mode; generally speaking, modes provide either hot standby or load balancing services.

https://wiki.linuxfoundation.org/networking/bridge

## Team device

Similar a bonded interface, the purpose of a team device is to provide a mechanism to group multiple NICs (ports) into one logical one (teamdev) at the L2 layer.

https://access.redhat.com/documentation/en-us/red_hat_enterprise_linux/7/html/networking_guide/sec-comparison_of_network_teaming_to_bonding

## VLAN

A VLAN, aka virtual LAN, separates broadcast domains by adding tags to network packets. 

https://techhub.hpe.com/eginfolib/networking/docs/switches/5820x-5800/5998-7387r_l2-lan_cg/content/441756596.htm

## VXLAN

VXLAN (Virtual eXtensible Local Area Network) is a tunneling protocol designed to solve the problem of limited VLAN IDs (4,096) in IEEE 802.1q. It is described by [IETF RFC 7348](https://datatracker.ietf.org/doc/html/rfc7348).

https://networkdirection.net/articles/routingandswitching/vxlanoverview/vxlanframes/

## MACVLAN


With VLAN, you can create multiple interfaces on top of a single one and filter packages based on a VLAN tag. With MACVLAN, you can create multiple interfaces with different Layer 2 (that is, Ethernet MAC) addresses on top of a single one.

Before MACVLAN, if you wanted to connect to physical network from a VM or namespace, you would have needed to create TAP/VETH devices and attach one side to a bridge and attach a physical interface to the bridge on the host at the same time, as shown below.

https://hicu.be/bridge-vs-macvlan

## IPVLAN

IPVLAN is similar to MACVLAN with the difference being that the endpoints have the same MAC address.

https://hicu.be/macvlan-vs-ipvlan


## MACVTAP/IPVTAP

MACVTAP/IPVTAP is a new device driver meant to simplify virtualized bridged networking. When a MACVTAP/IPVTAP instance is created on top of a physical interface, the kernel also creates a character device/dev/tapX to be used just like a TUN/TAP device, which can be directly used by KVM/QEMU.

https://linuxnatives.net/2012/virtualized-bridged-networking-with-macvtap

https://liuhangbin.netlify.app/post/virtual-ifaces/#macvtapipvtap

## MACSec

MACsec (Media Access Control Security) is an IEEE standard for security in wired Ethernet LANs. Similar to IPsec, as a layer 2 specification, MACsec can protect not only IP traffic but also ARP, neighbor discovery, and DHCP. 

https://developers.redhat.com/blog/2016/10/14/macsec-a-different-solution-to-encrypt-network-traffic


## VETH

The VETH (virtual Ethernet) device is a local Ethernet tunnel. 

https://developers.redhat.com/blog/2018/10/22/introduction-to-linux-interfaces-for-virtual-networking

## VCAN

Similar to the network loopback devices, the VCAN (virtual CAN) driver offers a virtual local [CAN (Controller Area Network)](https://en.wikipedia.org/wiki/CAN_bus) interface, so users can send/receive CAN messages via a VCAN interface. CAN is mostly used in the automotive field nowadays.

## VXCAN

Similar to the VETH driver, a VXCAN (Virtual CAN tunnel) implements a local CAN traffic tunnel between two VCAN network devices. When you create a VXCAN instance, two VXCAN devices are created as a pair. When one end receives the packet, the packet appears on the device's pair and vice versa. VXCAN can be used for cross-namespace communication.

