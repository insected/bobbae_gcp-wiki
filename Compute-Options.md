



Every Cloud based application has needs specific to its environment, and Google Cloud offers a diverse set of options to run your code on. What option is right for you? 

[https://www.youtube.com/watch?v=2tLXKCgqwLY](https://www.youtube.com/watch?v=2tLXKCgqwLY)

Tables comparing different hosting options.

[https://cloud.google.com/hosting-options#comparing_options](https://cloud.google.com/hosting-options#comparing_options)

Decision tree for compute options.

[https://cloud.google.com/blog/products/gcp/choosing-the-right-compute-option-in-gcp-a-decision-tree?m=1](https://cloud.google.com/blog/products/gcp/choosing-the-right-compute-option-in-gcp-a-decision-tree?m=1)

### PaaS / IaaS

[PaaS](PaaS) refers to cloud-based platform services that provide developers with a framework to build custom applications. Therefore, PaaS isn’t delivering software over the internet but provides a platform that’s accessible to different developers to create software that’s delivered over the internet.

[IaaS](https://cloud.google.com/learn/what-is-iaas) cloud-based infrastructure resources are delivered to organizations with virtualization technology that helps them build and manage their servers, network, data storage and operating systems. IaaS customers can control their own data infrastructure without having to physically manage it on-site.

### App Engine


The Google [App Engine](https://github.com/bobbae/gcp/wiki/App-Engine), which is also a PaaS solution, allows you to simply deploy your code, and the platform automates everything. GAE is fully scalable, meaning that it acquires more instances automatically if the traffic of your application becomes higher.

### Cloud Functions

[Cloud Functions](https://cloud.google.com/functions) allows users to write function code and let Google Cloud handle the operational infrastructure. Develop faster by writing and running small code snippets that respond to events. Connect to Google Cloud or third-party cloud services via triggers to streamline challenging orchestration problems.

[https://cloud.google.com/functions](https://cloud.google.com/functions)


#### Cloud functions framework

[https://cloud.google.com/functions/docs/functions-framework](https://cloud.google.com/functions/docs/functions-framework)


### Cloud Task

[Cloud Tasks](Cloud-Tasks) lets you separate out pieces of work that can be performed independently, outside of your main application flow, and send them off to be processed, asynchronously, using handlers that you create.

#### Using Cloud Tasks to trigger Cloud Function

https://cloud.google.com/tasks/docs/tutorial-gcf




### Cloud Run

[Cloud Run](https://cloud.google.com/run/docs) is a managed compute platform that enables you to run stateless containers that are invocable via web requests or Pub/Sub events. Cloud Run is serverless: it abstracts away all infrastructure management.


#### Cloud Run Quickstarts

https://cloud.google.com/run/docs/quickstarts

### Cloud Run for Anthos

[Cloud Run for Anthos](https://cloud.google.com/anthos/run) provides a flexible [serverless](Serverless) development platform on Google [Kubernetes](Kubernetes) Engine -- [GKE](GKE). Cloud Run for [Anthos](Anthos) is powered by [Knative](https://knative.dev/), an open source project that supports serverless workloads on Kubernetes. 

### Cloud GPUs

[Compute Engine provides graphics processing units](https://cloud.google.com/compute/docs/gpus) (GPUs) that you can add to your virtual machine instances. You can use these GPUs to accelerate specific workloads on your instances such as machine learning and data processing. If you have graphics-intensive workloads, such as 3D visualization, 3D rendering, or virtual applications, you can create virtual workstations that use NVIDIA® GRID® technology. For information on GPUs for graphics-intensive applications, see [GPUs for graphics workloads](https://cloud.google.com/compute/docs/gpus#gpu-virtual-workstations).



[https://www.youtube.com/watch?v=l3_uE4gdAWc](https://www.youtube.com/watch?v=l3_uE4gdAWc)

#### A2

https://cloud.google.com/blog/products/compute/a2-vms-with-nvidia-a100-gpus-are-ga

### Cloud TPUs

https://cloud.google.com/tpu/docs/tpus

### Preemptible VM Instances

A [preemptible](https://cloud.google.com/compute/docs/instances/preemptible) [VM](VM) is an instance that you can create and run at a much [lower price](https://cloud.google.com/compute/vm-instance-pricing) than normal instances. However, [Compute Engine](Compute) might stop (preempt) these instances if it requires access to those resources for other tasks. Preemptible instances are excess Compute Engine capacity, so their availability varies with usage.



[https://www.youtube.com/watch?v=ljol9IipvWs](https://www.youtube.com/watch?v=ljol9IipvWs)


### Shielded VMs

[Shielded VM](https://cloud.google.com/security/shielded-cloud/shielded-vm) offers verifiable integrity of your Compute Engine VM instances, so you can be confident your instances haven't been compromised by boot- or kernel-level [malware](https://en.wikipedia.org/wiki/Malware) or [rootkits](https://en.wikipedia.org/wiki/Rootkit). Shielded VM's verifiable integrity is achieved through the use of [Secure Boot](https://cloud.google.com/security/shielded-cloud/shielded-vm#secure-boot), [virtual trusted platform module (vTPM)](https://cloud.google.com/security/shielded-cloud/shielded-vm#vtpm)-enabled [Measured Boot](https://cloud.google.com/security/shielded-cloud/shielded-vm#measured-boot), and [integrity monitoring](https://cloud.google.com/security/shielded-cloud/shielded-vm#integrity-monitoring).


[https://www.youtube.com/watch?v=o3NXEgbvdmQ](https://www.youtube.com/watch?v=o3NXEgbvdmQ)


### Sole-tenant nodes

[Sole-tenancy]https://cloud.google.com/compute/docs/nodes) lets you have exclusive access to a sole-tenant node, which is a physical Compute Engine server that is dedicated to hosting only your project's VMs. Use sole-tenant nodes to keep your VMs physically separated from VMs in other projects, or to group your VMs together on the same host hardware.


[https://www.youtube.com/watch?v=ocHadXq14v8](https://www.youtube.com/watch?v=ocHadXq14v8)


### Bare Metal Solution

Enterprises want to embrace the pace of innovation and an operational business model of the modern-day cloud, but they don’t want to disrupt their existing IT landscape or upgrade all their legacy applications. This presents a conundrum, as most legacy applications were not designed to run in the cloud, and migrating them can be challenging, risky, and cost-prohibitive.  [Bare Metal Solution](https://cloud.google.com/bare-metal/docs) addresses these challenges by providing all the infrastructure you need to run your specialized workload such as Oracle Database close to Google Cloud. 

[https://www.youtube.com/watch?v=EVWrwCUQlL8](https://www.youtube.com/watch?v=EVWrwCUQlL8)



#### Configuring Google Access for On-Premise

[Private Google Access for on-premises hosts](https://cloud.google.com/vpc/docs/configure-private-google-access-hybrid) provides a way for on-premises systems to connect to [Google APIs and services](https://developers.google.com/apis-explorer/) by routing traffic through a [Cloud VPN](https://cloud.google.com/network-connectivity/docs/vpn) tunnel or a [Cloud Interconnect](https://cloud.google.com/network-connectivity/docs/interconnect) attachment (VLAN). Private Google Access for on-premises hosts is an alternative to connecting to Google APIs and services over the internet.



[https://www.youtube.com/watch?v=QUb86NiMZ8k](https://www.youtube.com/watch?v=QUb86NiMZ8k)


## Qwiklabs


[Google Assistant: Build an Application with Dialogflow and Cloud Functions](https://www.qwiklabs.com/focuses/3634?catalog_rank=%7B%22rank%22%3A19%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&parent=catalog&search_id=7510653)
