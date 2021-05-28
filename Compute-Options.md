



Every Cloud based application has needs specific to its environment, and Google Cloud offers a diverse set of options to run your code on. What option is right for you? 

[https://www.youtube.com/watch?v=2tLXKCgqwLY](https://www.youtube.com/watch?v=2tLXKCgqwLY)

Tables comparing different hosting options.

[https://cloud.google.com/hosting-options#comparing_options](https://cloud.google.com/hosting-options#comparing_options)

Decision tree for compute options.

[https://cloud.google.com/blog/products/gcp/choosing-the-right-compute-option-in-gcp-a-decision-tree?m=1](https://cloud.google.com/blog/products/gcp/choosing-the-right-compute-option-in-gcp-a-decision-tree?m=1)

### PaaS / IaaS

PaaS refers to cloud-based platform services that provide developers with a framework to build custom applications. Therefore, PaaS isn’t delivering software over the internet but provides a platform that’s accessible to different developers to create software that’s delivered over the internet.

IaaS cloud-based infrastructure resources are delivered to organizations with virtualization technology that helps them build and manage their servers, network, data storage and operating systems. IaaS customers can control their own data infrastructure without having to physically manage it on-site.

### App Engine


The Google [App Engine](https://github.com/bobbae/gcp/wiki/App-Engine), which is also a PaaS solution, allows you to simply deploy your code, and the platform automates everything. GAE is fully scalable, meaning that it acquires more instances automatically if the traffic of your application becomes higher.

### Cloud Functions

[Cloud Functions](https://cloud.google.com/functions) has a simple and intuitive developer experience. Just write your code and let Google Cloud handle the operational infrastructure. Develop faster by writing and running small code snippets that respond to events. Connect to Google Cloud or third-party cloud services via triggers to streamline challenging orchestration problems.

[https://cloud.google.com/functions](https://cloud.google.com/functions)

[https://cloud.google.com/functions/docs/functions-framework](https://cloud.google.com/functions/docs/functions-framework)

#### Using Cloud Tasks to trigger Cloud Function

https://cloud.google.com/tasks/docs/tutorial-gcf


### Cloud Run

[Cloud Run](https://cloud.google.com/run/docs) is a managed compute platform that enables you to run stateless containers that are invocable via web requests or Pub/Sub events. Cloud Run is serverless: it abstracts away all infrastructure management.


Cloud Run takes containers and makes them invocable via HTTP requests, Cloud Functions remain as Google's event-driven serverless platform.

https://cloud.google.com/run/docs/quickstarts

### Cloud Run for Anthos

[Cloud Run for Anthos](https://cloud.google.com/anthos/run) provides a flexible serverless development platform on Google Kubernetes Engine (GKE). Cloud Run for Anthos is powered by [Knative](https://knative.dev/), an open source project that supports serverless workloads on Kubernetes. 

### Cloud GPUs

Compute Engine provides graphics processing units (GPUs) that you can add to your virtual machine instances. You can use these GPUs to accelerate specific workloads on your instances such as machine learning and data processing. If you have graphics-intensive workloads, such as 3D visualization, 3D rendering, or virtual applications, you can create virtual workstations that use NVIDIA® GRID® technology. For information on GPUs for graphics-intensive applications, see [GPUs for graphics workloads](https://cloud.google.com/compute/docs/gpus#gpu-virtual-workstations).

[https://cloud.google.com/compute/docs/gpus](https://cloud.google.com/compute/docs/gpus)

A video about using GPUs to accelerate and scale as needed.

[https://www.youtube.com/watch?v=l3_uE4gdAWc](https://www.youtube.com/watch?v=l3_uE4gdAWc)


### Preemptible VM Instances

A preemptible VM is an instance that you can create and run at a much [lower price](https://cloud.google.com/compute/vm-instance-pricing) than normal instances. However, Compute Engine might stop (preempt) these instances if it requires access to those resources for other tasks. Preemptible instances are excess Compute Engine capacity, so their availability varies with usage.

[https://cloud.google.com/compute/docs/instances/preemptible](https://cloud.google.com/compute/docs/instances/preemptible)

A video about bringing cost down using preemptible VMs.

[https://www.youtube.com/watch?v=ljol9IipvWs](https://www.youtube.com/watch?v=ljol9IipvWs)


### Shielded VMs

Shielded VM offers verifiable integrity of your Compute Engine VM instances, so you can be confident your instances haven't been compromised by boot- or kernel-level [malware](https://en.wikipedia.org/wiki/Malware) or [rootkits](https://en.wikipedia.org/wiki/Rootkit). Shielded VM's verifiable integrity is achieved through the use of [Secure Boot](https://cloud.google.com/security/shielded-cloud/shielded-vm#secure-boot), [virtual trusted platform module (vTPM)](https://cloud.google.com/security/shielded-cloud/shielded-vm#vtpm)-enabled [Measured Boot](https://cloud.google.com/security/shielded-cloud/shielded-vm#measured-boot), and [integrity monitoring](https://cloud.google.com/security/shielded-cloud/shielded-vm#integrity-monitoring).

[https://cloud.google.com/security/shielded-cloud/shielded-vm](https://cloud.google.com/security/shielded-cloud/shielded-vm)

How do you secure sensitive data and workloads in the cloud, while still keeping it private? In this video, we address just that, and show you how to create a shielded VM in Google Cloud Console, and how to ensure encryption in-use for workloads with Google Cloud Confidential Computing. 

[https://www.youtube.com/watch?v=o3NXEgbvdmQ](https://www.youtube.com/watch?v=o3NXEgbvdmQ)


### Sole-tenant nodes

Sole-tenancy lets you have exclusive access to a sole-tenant node, which is a physical Compute Engine server that is dedicated to hosting only your project's VMs. Use sole-tenant nodes to keep your VMs physically separated from VMs in other projects, or to group your VMs together on the same host hardware.

[https://cloud.google.com/compute/docs/nodes](https://cloud.google.com/compute/docs/nodes)

Sole-tenant nodes? VMaaS and CloudSimple? N1 vs N2 vs E2 instances? BYO Microsoft or Linux licenses? Understand how the choices available with Google Cloud can maximize your savings while expanding your migration scenarios. 

[https://www.youtube.com/watch?v=ocHadXq14v8](https://www.youtube.com/watch?v=ocHadXq14v8)


### Bare Metal Solution

Enterprises want to embrace the pace of innovation and an operational business model of the modern-day cloud, but they don’t want to disrupt their existing IT landscape or upgrade all their legacy applications. This presents a conundrum, as most legacy applications were not designed to run in the cloud, and migrating them can be challenging, risky, and cost-prohibitive.  Bare Metal Solution addresses these challenges by providing all the infrastructure you need to run your specialized workload such as Oracle Database close to Google Cloud. Learn how Bare Metal Solutions enable enterprises to migrate all such workloads to GCP in a simple, cost effective and secure way.

[https://www.youtube.com/watch?v=EVWrwCUQlL8](https://www.youtube.com/watch?v=EVWrwCUQlL8)

Documentation on Bare Metal solutions.

[https://cloud.google.com/bare-metal/docs](https://cloud.google.com/bare-metal/docs)


#### Configuring Google Access for On-Premise

Private Google Access for on-premises hosts provides a way for on-premises systems to connect to [Google APIs and services](https://developers.google.com/apis-explorer/) by routing traffic through a [Cloud VPN](https://cloud.google.com/network-connectivity/docs/vpn) tunnel or a [Cloud Interconnect](https://cloud.google.com/network-connectivity/docs/interconnect) attachment (VLAN). Private Google Access for on-premises hosts is an alternative to connecting to Google APIs and services over the internet.

[https://cloud.google.com/vpc/docs/configure-private-google-access-hybrid](https://cloud.google.com/vpc/docs/configure-private-google-access-hybrid)

Before migrating a portion of your environment to the Cloud, it is important to plan ahead for IP address changes that could affect your workloads. Learn about private and public IPs on Google Cloud and how you can achieve remappable IP addresses for your Cloud resources. 

[https://www.youtube.com/watch?v=QUb86NiMZ8k](https://www.youtube.com/watch?v=QUb86NiMZ8k)


## Qwiklabs


[Google Assistant: Build an Application with Dialogflow and Cloud Functions](https://www.qwiklabs.com/focuses/3634?catalog_rank=%7B%22rank%22%3A19%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&parent=catalog&search_id=7510653)
