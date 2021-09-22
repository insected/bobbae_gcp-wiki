
### 802.15.4

[IEEE 802.15.4](https://standards.ieee.org/standard/802_15_4-2020.html
) is a technical standard which defines the operation of low-rate wireless personal area networks (LR-WPANs). It specifies the physical layer and media access control for LR-WPANs, and is maintained by the IEEE 802.15 working group, which defined the standard in 2003.



### ZigBee 

[ZigBee](https://zigbeealliance.org/solution/zigbee/
) is a 2.4 GHz mesh local area network (LAN) protocol. It was originally designed for building automation and control—so things like wireless thermostats and lighting systems often use ZigBee.




### LoRaWAN 

[LoRaWAN](https://lora-alliance.org/
) is a media access control (MAC) layer protocol designed for large-scale public networks with a single operator. It is built using Semtech’s LoRa modulation as the underlying PHY, but it is important to note that LoRa and LoRaWAN are two seperate things that are often (mistakenly) conflated. 



### GPRS 

[General Packet Radio Service](https://www.twilio.com/docs/glossary/what-general-packet-radio-service-gprs
) (GPRS) is a packet oriented mobile data standard on the 2G and 3G cellular communication network's global system for mobile communications (GSM). GPRS was established by European Telecommunications Standards Institute (ETSI) in response to the earlier CDPD and i-mode packet-switched cellular technologies. It is now maintained by the 3rd Generation Partnership Project (3GPP).



### 3G & 4G

[3G](https://en.wikipedia.org/wiki/3G) was the first “high speed” cellular network, and is a name that refers to a number of technologies that meet IMT-2000 standards. 4G is the generation of cellular standards that followed 3G, and is what most people use today for mobile cellular data. You can use 3G and 4G for IoT devices, but the application needs a constant power source or must be able to be recharged regularly.


### GSM

The [Global System for Mobile Communications](https://en.wikipedia.org/wiki/GSM) (GSM) is a standard developed by the European Telecommunications Standards Institute (ETSI) to describe the protocols for second-generation (2G) digital cellular networks used by mobile devices such as mobile phones and tablets. It was first deployed in Finland in December 1991.


### LTE 

The Long-Term Evolution [LTE](https://en.wikipedia.org/wiki/LTE) is a standard for wireless broadband for mobile access based on GSM/EDGE and UMTS/HSPA.


### LTE-M1

[LTE-M1](https://en.wikipedia.org/wiki/LTE-M) is the first cellular wireless protocol that was build from the ground up for IoT devices. 


### NB-IoT

[NB-IoT](https://en.wikipedia.org/wiki/Narrowband_IoT), or Narrowband IoT, is another way to tackle cellular M2M for low power devices. It is based on a DSSS modulation similar to the old Neul version of Weightless-W. Huawei, Ericsson, and Qualcomm are active proponents of this protocol and are involved in putting it together.


### 5G


[5G](https://en.wikipedia.org/wiki/5G
) is the fifth generation technology standard for broadband cellular networks, which cellular phone companies began deploying worldwide in 2019, and is the planned successor to the 4G networks which provide connectivity to most current cellphones. 5G networks are predicted to have more than 1.7 billion subscribers worldwide by 2025, according to the GSM Association.


### O-RAN

https://cloud.google.com/blog/topics/telecommunications/google-cloud-joins-o-ran-alliance

### Cellular IoT Overview

https://www.iotforall.com/cellular-iot-explained-nb-iot-vs-lte-m

### MQTT 

An MQTT (Message Queuing Telemetry Transport) is a lightweight IoT data protocol. It features a publisher-subscriber messaging model and allows for simple data flow between different devices.

MQTT’s main selling point is its architecture. Its genetic make-up is basic and lightweight and, therefore, it’s able to provide low power consumption for devices. It also works on top of a TCP/IP protocol.

IoT data protocols were designed to tackle unreliable communication networks. This became a need in the IoT world due to the increasing number of small, cheap, and lower-power objects that have appeared in the network over the past few years.

https://en.wikipedia.org/wiki/MQTT

### CoAP

A [CoAp](https://en.wikipedia.org/wiki/Constrained_Application_Protocol
) (Constrained Application Protocol) is an application layer protocol. It’s designed to address the needs of HTTP-based IoT systems. HTTP stands for Hypertext Transfer Protocol, and it’s the foundation of data communication for the World Wide Web.

While the existing structure of the internet is freely available and usable by any IoT device, it’s often too heavy and power-consuming for most IoT applications. This has led to many within the IoT community dismissing HTTP as a protocol not suitable for IoT.



### AMQP 

An [Advanced Message Queuing Protocol](https://en.wikipedia.org/wiki/Advanced_Message_Queuing_Protocol) (AMQP) is an open standard application layer protocol used for transactional messages between servers.

AMQP is an open standard application layer protocol for message-oriented middleware. The defining features of AMQP are message orientation, queuing, routing (including point-to-point and publish-and-subscribe), reliability and security.

AMQP mandates the behavior of the messaging provider and client to the extent that implementations from different vendors are interoperable, in the same way as SMTP, HTTP, FTP, etc. have created interoperable systems. Previous standardizations of middleware have happened at the API level (e.g. JMS) and were focused on standardizing programmer interaction with different middleware implementations, rather than on providing interoperability between multiple implementations.

AMQP was originated in 2003 by John O'Hara at JPMorgan Chase in London. AMQP was conceived as a co-operative open effort. The initial design was by JPMorgan Chase from mid-2004 to mid-2006 and it contracted iMatix Corporation to develop a C broker and protocol documentation. In 2005 JPMorgan Chase approached other firms to form a working group that included Cisco Systems, IONA Technologies, iMatix, Red Hat, and Transaction Workflow Innovation Standards Team (TWIST). In the same year JPMorgan Chase partnered with Red Hat to create Apache Qpid, initially in Java and soon after C++. Independently, [RabbitMQ](https://en.wikipedia.org/wiki/RabbitMQ) was developed in [Erlang](https://en.wikipedia.org/wiki/Erlang_(programming_language)) by Rabbit Technologies, followed later by the Microsoft and StormMQ implementations.



### DDS 


[DDS](https://en.wikipedia.org/wiki/Data_Distribution_Service) (Data Distribution Service) is another scalable IoT protocol that enables high-quality communication in IoT. Similar to the MQTT, DDS also works to a publisher-subscriber model.

It can be deployed in multiple settings, from the cloud to very small devices. This makes it perfect for real-time and embedded systems. Moreover, unlike [MQTT](https://en.wikipedia.org/wiki/MQTT), the DDS protocol allows for interoperable data exchange that is independent of the hardware and the software platform.

## Industrial Networking

### Modbus

[Modbus](https://instrumentationtools.com/compare-modbus-fieldbus-and-profibus/
) is a granddaddy of industrial communication protocols. Modbus is Modicon plus fieldbus.

Modbus, a serial communication protocol developed by Modicon in 1979. It is developed by  Modicon for PLC in industrial applications, now it an open protocol. It is used over serial and Ethernet cable.



### Profibus


[Profibus](https://en.wikipedia.org/wiki/Profibus
) (usually styled as PROFIBUS, as a portmanteau for Process Field Bus) is a standard for fieldbus communication in automation technology and was first promoted in 1989 by BMBF (German department of education and research) and then used by Siemens. It should not be confused with the Profinet standard for Industrial Ethernet. Profibus is openly published as part of IEC 61158.



### CAN Bus

A [Controller Area Network](https://en.wikipedia.org/wiki/CAN_bus
) (CAN bus) is a robust vehicle bus standard designed to allow microcontrollers and devices to communicate with each other's applications without a host computer. It is a message-based protocol, designed originally for multiplex electrical wiring within automobiles to save on copper, but it can also be used in many other contexts. For each device, the data in a frame is transmitted sequentially but in such a way that if more than one device transmits at the same time, the highest priority device can continue while the others back off. Frames are received by all devices, including by the transmitting device.


