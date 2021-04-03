- [Comparisons](#comparisons)
  * [AWS vs. GCP](#aws-vs-gcp)
  * [VMs vs. Containers](#vms-vs-containers)
  * [DevOps vs. SRE](#devops-vs-sre)
  * [Terraform vs. Ansible](#terraform-vs-ansible)
  * [SQL vs NoSQL](#sql-vs-nosql)
  * [Data Engineering vs. Data Science](#data-engineering-vs-data-science)
  * [ETL vs ELT](#etl-vs-elt)
  * [Deep Learning vs. Machine Learning](#deep-learning-vs-machine-learning)
  * [TLS vs SSL](#tls-vs-ssl)
  * [TLS vs HTTPS](#tls-vs-https)

<small><i><a href='http://ecotrust-canada.github.io/markdown-toc/'>Table of contents generated with markdown-toc</a></i></small>

<small><i><a href='http://ecotrust-canada.github.io/markdown-toc/'>Table of contents generated with markdown-toc</a></i></small>


## Comparisons

A Collection of differences between similar topics often compared in the context of Cloud computing and Data Analytics.

### AWS vs. GCP 

Compare Google Cloud with AWS and highlight the similarities and differences between the two. 

[https://cloud.google.com/docs/compare/aws](https://cloud.google.com/docs/compare/aws) 

### VMs vs. Containers

Virtual machines (VMs) are a technology for building virtualized computing environments. They have been around for quite a while and are considered the foundation of the first generation of cloud computing.

Containers are a lighter-weight, more agile way of handling virtualization. Rather than spinning up an entire virtual machine, a container packages together everything needed to run a small piece of software. The container includes all the code, its dependencies, and even the operating system itself. This enables applications to run almost anywhere—a desktop computer, a traditional IT infrastructure, or the cloud.

https://www.ibm.com/cloud/blog/containers-vs-vms




### DevOps vs. SRE

A video discussing differences and similarities between DevOps and SRE.

[https://www.youtube.com/watch?v=uTEL8Ff1Zvk](https://www.youtube.com/watch?v=uTEL8Ff1Zvk)

Some books on SRE from google.

[https://landing.google.com/sre/books/](https://landing.google.com/sre/books/)

### Terraform vs. Ansible

Infrastructure as Code (IAC) refers to the process of managing and provisioning computer data centers. It’s a strategy for managing data center servers, networking infrastructure, and storage. Its purpose is to simplify large-scale management and configuration dramatically.

IAC allows provisioning and managing of computer data centers via machine-readable definition files without having to configure tools or physical hardware. In simpler terms, IAC treats manual configurations, build guides, run books, and related procedures as code. Read by software, the code that maintains the state of the infrastructure.


There are several IAC tools to choose from, with three major examples being Ansible, Terraform, and Puppet.

Hashicorp developed Terraform as an infrastructure orchestrator and service provisioner. It is cloud-agnostic, supporting several providers. As a result, users can manage multi-cloud or multi offering environments, using the same programming language and configuration construct. It utilizes the Haschorp Language and is quite user-friendly as compared to other tools.

Ansible is a powerful tool used to bring services and servers into the desired state, utilizing an assortment of classes and configuration methods. Additionally, it can also connect to different providers via wrapper modules to configure resources. Users prefer it because it is lightweight when coding is concerned, with speedy deployment capabilities.



https://phoenixnap.com/blog/ansible-vs-terraform-vs-puppet

### SQL vs NoSQL

Structured Query language (SQL) pronounced as "S-Q-L" or sometimes as "See-Quel" is the standard language for dealing with Relational Databases. A relational database defines relationships in the form of tables.

NoSQL is a non-relational DMS, that does not require a fixed schema, avoids joins, and is easy to scale. NoSQL database is used for distributed data stores with humongous data storage needs. NoSQL is used for Big data and real-time web apps. For example companies like Twitter, Facebook, Google that collect terabytes of user data every single day.

https://www.guru99.com/sql-vs-nosql.html

### Data Engineering vs. Data Science

https://www.datacamp.com/community/blog/data-scientist-vs-data-engineer

### ETL vs ELT

ETL stands for Extract, Transform, and Load, while ELT stands for Extract, Load, and Transform. In ETL, data flow from the data source to staging to the data destination. ELT lets the data destination do the transformation, eliminating the need for data staging.

https://www.xplenty.com/blog/etl-vs-elt/

### Deep Learning vs. Machine Learning

Machine Learning and Deep Learning are concepts that are often overlapping. There can be a slight confusion between the terms, and thus, let us look at Machine learning vs Deep learning, and understand the similarities and differences between the same.

Machine learning uses algorithms to parse data, learn from that data, and make informed decisions based on what it has learned. While both fall under the broad category of artificial intelligence, deep learning is what powers the most human-like artificial intelligence. Deep learning structures algorithms in layers to create an “artificial neural network” that can learn and make intelligent decisions on its own.

https://www.zendesk.com/blog/machine-learning-and-deep-learning/

### TLS vs SSL


Transport Layer Security, or TLS, is a widely adopted security protocol designed to facilitate privacy and data security for communications over the Internet. 

TLS evolved from a previous encryption protocol called Secure Sockets Layer (SSL), which was developed by Netscape. TLS version 1.0 actually began development as SSL version 3.1, but the name of the protocol was changed before publication in order to indicate that it was no longer associated with Netscape. Because of this history, the terms TLS and SSL are sometimes used interchangeably.

### TLS vs HTTPS

HTTPS is an implementation of TLS encryption on top of the HTTP protocol, which is used by all websites as well as some other web services. Any website that uses HTTPS is therefore employing TLS encryption.

https://www.cloudflare.com/learning/ssl/transport-layer-security-tls/

