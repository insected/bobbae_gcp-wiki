

[Infrastructure as Code](https://en.wikipedia.org/wiki/Infrastructure_as_code) (IAC) refers to the process of managing and provisioning computer data centers. It’s a strategy for managing data center servers, networking infrastructure, and storage. Its purpose is to simplify large-scale management and configuration dramatically.

IAC allows provisioning and managing of computer data centers via machine-readable definition files without having to configure tools or physical hardware. In simpler terms, IAC treats manual configurations, build guides, run books, and related procedures as code. Read by software, the code that maintains the state of the infrastructure.



Provisioning compute resources has traditionally been hard to manage, not scalable, and prone to error, so what other techniques can you use to make sure you’re ready to meet demand? You can automate the creation of your cloud resources, create templates, and store config files with the help of tools like Google [Cloud Deployment Manager](Cloud-Deployment-Manager).



[https://cloud.google.com/solutions/infrastructure-as-code](https://cloud.google.com/solutions/infrastructure-as-code)



https://phoenixnap.com/blog/infrastructure-as-code-best-practices-tools

## Cloud Foundation Toolkit

The [Cloud Foundation Toolkit](Cloud-Foundation-Toolkit) is designed specifically to meet the compliance and security needs of enterprises.

https://github.com/terraform-google-modules

### Terraform 

[Terraform](Terraform) is supported in the [Cloud Foundation Toolkit](Cloud-Foundation-Toolkit).

https://github.com/GoogleCloudPlatform/cloud-foundation-toolkit/blob/master/docs/terraform.md




### Cloud Deployment Manager


[Cloud Deployment Manager](Cloud-Deployment-Manager) is Google's own IAC tool supported in the  [Cloud Foundation Toolkit](Cloud-Foundation-Toolkit).


## Immutable infrastructure


[Immutable infrastructure]( https://www.hashicorp.com/resources/what-is-mutable-vs-immutable-infrastructure    ) is a philosophy that builds on the benefits of infrastructure as code. 

Immutable infrastructure mandates that resources never be modified after they're deployed. If a virtual machine, Kubernetes cluster, or firewall rule needs to be updated, you can update the configuration for the resource in the source repository. After you've tested and validated the changes, you fully redeploy the resource using the new configuration. In other words, rather than tweaking resources, you re-create them.

Creating immutable infrastructure leads to more predictable deployments and rollbacks. It also mitigates issues that are common in mutable infrastructures, like configuration drift and [snowflake servers](  https://martinfowler.com/bliki/SnowflakeServer.html   ). In this way, adopting immutable infrastructure further improves the consistency and reliability of your environments.


## Other IAC Tools

### Pulumi

Pulumi is open source infrastructure as code SDK that enables you to create, deploy, and manage infrastructure on different clouds in various programming languages.

[https://www.pulumi.com/docs/get-started/gcp/](https://www.pulumi.com/docs/get-started/gcp/)


### Ansible

Ansible is a way to automate apps and IT infrastructure. Application Deployment + Configuration Management + Continuous Delivery.

[Here](https://www.youtube.com/watch?v=utztQWTewWU)  is an opinionated look at how ansible and terraform complement one another in a provisioner/configuration management separated view. A key takeaway is a simplified workflow for sysadmins/operators in cloud management that can be applied in multi-cloud/hybrid cloud scenarios.


### AWS Cloud formation

AWS CloudFormation lets users model a collection of related AWS and third-party resources, provision them quickly and consistently, and manage them throughout their lifecycles, by treating infrastructure as code. A CloudFormation template describes your desired resources and their dependencies so you can launch and configure them together as a stack. 

https://aws.amazon.com/cloudformation/

### Azure Resource Manager

https://docs.microsoft.com/en-us/azure/azure-resource-manager/management/overview

### Openstack Heat

The OpenStack Foundation has also defined a similar standard for specifying resources and the orchestrations for managing infrastructure, and application lifecycles. The heat-translator project was one of the first to adopt TOSCA for standardized templating.

https://wiki.openstack.org/wiki/Heat

### TOSCA

Topology and Orchestration Specification for Cloud Applications (TOSCA), is an OASIS standard language to describe a topology of cloud based web services, their components, relationships, and the processes that manage them. The TOSCA standard includes specifications to describe processes that create or modify web services.

https://en.wikipedia.org/wiki/OASIS_TOSCA

### Cloudify

Cloudify is an open-source TOSCA-based orchestration framework based on YAML.

https://cloudify.co/

### MANO, NFV, VNF, SDN, TOSCA 


https://cloudify.co/blog/mobile-world-congress-nfv-sdn-network-orchestration-automation/

### Comparison of terraform and cloud formation and heat, etc.

https://www.terraform.io/intro/vs/cloudformation.html

### Kubernetes



https://cloud.google.com/blog/products/containers-kubernetes/understanding-configuration-as-data-in-kubernetes

##  Qwiklabs




[VM Migration](https://www.qwiklabs.com/quests/87?catalog_rank=%7B%22rank%22%3A2%2C%22num_filters%22%3A1%2C%22has_search%22%3Atrue%7D&search_id=7467726)


[Terraform Qwiklabs](https://www.qwiklabs.com/quests/44)