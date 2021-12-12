[VLANs](  https://wikipedia.org/wiki/Virtual_LAN ) allow network administrators to group hosts under the same switch or between different switches.

The protocol most commonly used today to support VLANs is [IEEE 802.1Q]( https://wikipedia.org/wiki/IEEE_802.1Q   ).

VLANs work by [applying tags](https://www.firewall.cx/networking-topics/vlan-networks/219-vlan-tagging.html) to network frames and handling these tags in networking systems – creating the appearance and functionality of network traffic that is physically on a single network but acts as if it is split between separate networks. In this way, VLANs can [keep network applications separate](https://en.m.wikipedia.org/wiki/VLAN_Trunking_Protocol) despite being connected to the same physical network, and without requiring multiple sets of cabling and networking devices to be deployed.


## Virtual Networking 


[Network Virtualization](  https://www.vmware.com/topics/glossary/content/network-virtualization ) is a process of logically grouping physical networks and making them operate as single or multiple independent networks called Virtual Networks.

For example, [VMware NSX Data Center](    https://docs.vmware.com/en/VMware-NSX-Data-Center-for-vSphere/index.html  ) is a network virtualization platform that delivers networking and security components like firewalling, switching, and routing that are defined and consumed in software.

Linux also has [network utilities](https://man7.org/linux/man-pages/man8/ip-link.8.html
) and  [rich virtual networking capabilities](https://developers.redhat.com/blog/2018/10/22/introduction-to-linux-interfaces-for-virtual-networking
) that are used as [basis](https://developers.redhat.com/blog/2018/10/22/introduction-to-linux-interfaces-for-virtual-networking
) for [hosting VMs and containers](https://liuhangbin.netlify.app/post/virtual-ifaces
), as well as [cloud environments](https://lloydrochester.com/post/unix/virtual_networking_device_types/
).  







### NFV, VNF, SDN

#### Comparison of NFV, VNF, SDN

https://cloudify.co/blog/mobile-world-congress-nfv-sdn-network-orchestration-automation/

#### NFV

[Network Function Virtualization](https://en.wikipedia.org/wiki/Network_function_virtualization) is an approach by Telecom companies for deployment, management and scaling of network functions. NFV allows for decoupling and virtualization of existing OSS or legacy hardware to make them software driven and use standardized hardware. NFV is about overarching concept as a framework for running SDN functions.

#### VNF

[Virtualized Network Function](https://www.thousandeyes.com/learning/glossary/vnf-virtual-network-functions) is the implementation of a network function by utilizing a software decoupled from the underlying hardware infrastructure. This concerns with the general requirement for significant changes to existing code in order to convert a Network Function (NF) into a Virtualized Network Function (VNF). Common VNFs include virtualized routers, firewalls, WAN optimization, and [network address translation](https://en.wikipedia.org/wiki/Network_address_translation) (NAT) services.

#### SDN

[Software Defined Networking](https://en.wikipedia.org/wiki/Software-defined_networking) is an approach that decouples the control plane from the data plane in networking equipment.  NFV and SDN  are complimentary. SDN enables keeping the intelligence of the network within the controller, leaving the network equipment handling data which can execute operations mandated by the controller.  The network equipment does not need powerful controller capabilities and can be based on POTS (Plain, Off the shelf) virtualized servers.

#### MANO

[MANO](https://en.wikipedia.org/wiki/Network_function_virtualization#Management_and_orchestration_%28MANO%29) is defined by [ETSI](https://en.wikipedia.org/wiki/ETSI) as the layer that manages and orchestrates the cloud resources infrastructure.  It consists of VIM, VNFM, and Orchestrator.  Together they provide a full end-to-end lifecycle solution of NFV orchestration and management -- from installation, deployment and through to post-deployment.   MANO makes use of [TOSCA](https://en.wikipedia.org/wiki/OASIS_TOSCA) as NFV orchestration standard.




## OVS

[Open vSwitch](https://www.openvswitch.org/), sometimes abbreviated as OVS, is an open-source implementation of a distributed virtual multilayer switch. The main purpose of Open vSwitch is to provide a switching stack for hardware virtualization environments, while supporting multiple protocols and standards used in computer networks.

It is designed to enable massive network automation through programmatic extension, while still supporting standard management interfaces and protocols (e.g. NetFlow, sFlow, IPFIX, RSPAN, CLI, LACP, 802.1ag).  In addition, it is designed to support distribution across multiple physical servers similar to VMware's vNetwork distributed vswitch or Cisco's Nexus 1000V. 


## Bridge

A [Linux bridge](https://wiki.linuxfoundation.org/networking/bridge) behaves like a network switch. It forwards packets between interfaces that are connected to it. It's usually used for forwarding packets on routers, on gateways, or between VMs and network namespaces on a host. It also supports STP, VLAN filter, and multicast snooping.

https://wiki.linuxfoundation.org/networking/bridge

## Bonding

The Linux [bonding](https://www.learnitguide.net/2015/07/what-is-bonding-how-to-configure-in-linux.html) driver provides a method for aggregating multiple network interfaces into a single logical "bonded" interface. The behavior of the bonded interface depends on the mode; generally speaking, modes provide either hot standby or load balancing services.


## Team device

Similar a bonded interface, the purpose of a [team device](https://access.redhat.com/documentation/en-us/red_hat_enterprise_linux/7/html/networking_guide/sec-comparison_of_network_teaming_to_bonding) is to provide a mechanism to group multiple NICs (ports) into one logical one (teamdev) at the L2 layer.



## VLAN

A [VLAN](https://techhub.hpe.com/eginfolib/networking/docs/switches/5820x-5800/5998-7387r_l2-lan_cg/content/441756596.htm), aka virtual LAN, separates broadcast domains by adding tags to network packets. 



## VXLAN

[VXLAN](https://networkdirection.net/articles/routingandswitching/vxlanoverview/vxlanframes/) (Virtual eXtensible Local Area Network) is a tunneling protocol designed to solve the problem of limited VLAN IDs (4,096) in IEEE 802.1q. It is described by [IETF RFC 7348](https://datatracker.ietf.org/doc/html/rfc7348).



## MACVLAN


With VLAN, you can create multiple interfaces on top of a single one and filter packages based on a VLAN tag. With [MACVLAN](https://hicu.be/bridge-vs-macvlan), you can create multiple interfaces with different Layer 2 (that is, Ethernet MAC) addresses on top of a single one.

Before MACVLAN, if you wanted to connect to physical network from a VM or namespace, you would have needed to create TAP/VETH devices and attach one side to a bridge and attach a physical interface to the bridge on the host at the same time, as shown below.



### Running Openshift on Openstack with Macvlan CNI Plug-in

https://cloud.redhat.com/blog/openshift-on-openstack-with-macvlan-cni-plug-in

## IPVLAN

IPVLAN is similar to MACVLAN with the difference being that the endpoints have the same MAC address.

https://hicu.be/macvlan-vs-ipvlan


## MACVTAP/IPVTAP

MACVTAP/IPVTAP is a new device driver meant to simplify virtualized bridged networking. When a MACVTAP/IPVTAP instance is created on top of a physical interface, the kernel also creates a character device/dev/tapX to be used just like a TUN/TAP device, which can be directly used by KVM/QEMU.

https://linuxnatives.net/2012/virtualized-bridged-networking-with-macvtap

https://liuhangbin.netlify.app/post/virtual-ifaces/#macvtapipvtap

## MACSec

[MACsec](https://developers.redhat.com/blog/2016/10/14/macsec-a-different-solution-to-encrypt-network-traffic
) (Media Access Control Security) is an IEEE standard for security in wired Ethernet LANs. Similar to IPsec, as a layer 2 specification, MACsec can protect not only IP traffic but also ARP, neighbor discovery, and DHCP. 



## VETH

The [VETH](https://developers.redhat.com/blog/2018/10/22/introduction-to-linux-interfaces-for-virtual-networking
) (virtual Ethernet) device is a local Ethernet tunnel. 


## VCAN

The VCAN (virtual CAN) driver offers a virtual local [CAN (Controller Area Network)](https://en.wikipedia.org/wiki/CAN_bus) interface, so users can send/receive CAN messages via a [VCAN interface](https://en.wikipedia.org/wiki/SocketCAN). [CAN bus](https://en.wikipedia.org/wiki/CAN_bus) is a vehicle bus standard to allow microcontrollers to communicate, mostly used in the automotive field.

## VXCAN

Similar to the VETH driver, a [VXCAN](https://cateee.net/lkddb/web-lkddb/CAN_VXCAN.html) (Virtual CAN tunnel) implements a [local CAN traffic tunnel between two VCAN network devices](https://www.lagerdata.com/articles/forwarding-can-bus-traffic-to-a-docker-container-using-vxcan-on-raspberry-pi). When you create a VXCAN instance, two VXCAN devices are created as a pair. When one end receives the packet, the packet appears on the device's pair and vice versa. VXCAN can be used for cross-namespace communication.

