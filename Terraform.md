[Terraform](https://terraform.io) is a tool from Hashicorp for building, changing, and versioning infrastructure safely and efficiently. Terraform can manage existing and popular service providers as well as custom in-house solutions.

## Cloud Foundation Toolkit

Google Cloud Foundation Toolkit supports Terraform as well as Google Cloud Deployment manager.

[Cloud Foundation Toolkit](Cloud-Foundation-Toolkit)


## Infrastructure as Code

[Infrastructure as Code](Infrastructure-as-Code)  is the process of managing and provisioning computer data centers through machine-readable definition files, rather than physical hardware configuration or interactive configuration tools.

https://www.mineiros.io/blog/the-ultimate-guide-on-how-to-write-terraform-modules-part-1

Terraform's infrastructure-as-code (IAC) approach supports [DevOps](https://cloud.google.com/devops) best practices for change management, letting you manage Terraform configuration files in source control to maintain an ideal provisioning state for testing and production environments.

### HCL

https://www.terraform.io/docs/language/index.html



Defining and managing your development, test, staging, and production environments using infra-as-code tools such as [Deployment Manager](https://cloud.google.com/deployment-manager) or [Terraform](https://www.terraform.io/) is a common practice. 

[https://www.youtube.com/watch?v=3vfXQxWJazM](https://www.youtube.com/watch?v=3vfXQxWJazM)

[https://www.terraform.io/intro/index.html](https://www.terraform.io/intro/index.html)

### Module

A Terraform module is a set of Terraform configuration files in a single directory. Even a simple configuration consisting of a single directory with one or more .tf files is a module. When you run Terraform commands directly from such a directory, it is considered the root module. So in this sense, every Terraform configuration is part of a module. 

https://registry.terraform.io/browse/modules

### Using terraform with Google Cloud

https://cloud.google.com/docs/terraform

## Extending terraform 

### Plugins

https://www.terraform.io/docs/extend/how-terraform-works.html

### Custom Providers

https://www.terraform.io/docs/extend/hashicorp-provider-design-principles.html




## Using terraform

https://www.digitalocean.com/community/tutorial_series/how-to-manage-infrastructure-with-terraform


### Best Practices


https://geekflare.com/terraform-best-practices/


### Loops and conditions

https://blog.gruntwork.io/terraform-tips-tricks-loops-if-statements-and-gotchas-f739bbae55f9


### Troubleshooting

https://learn.hashicorp.com/tutorials/terraform/troubleshooting-workflow


### Mistakes


https://blog.pipetail.io/posts/2020-10-29-most-common-mistakes-terraform/


### Pain points



https://adambrodziak.pl/terraform-is-terrible

### Issues

https://www.schibsted.pl/blog/9-reasons-why-terraform-is-a-pain-and-1-why-you-should-still-care/

### Debugging terraform

https://www.terraform.io/docs/internals/debugging.html

#### Debug a Terraform Provider

https://learn.hashicorp.com/tutorials/terraform/provider-debug






## Tutorials

### Getting Started on GCP with terraform

[https://cloud.google.com/community/tutorials/getting-started-on-gcp-with-terraform](https://cloud.google.com/community/tutorials/getting-started-on-gcp-with-terraform)


### Managing infrastructure as code with Terraform, Cloud Build, and GitOps

[https://cloud.google.com/solutions/managing-infrastructure-as-code](https://cloud.google.com/solutions/managing-infrastructure-as-code)


### Hashicorp  terraform on GCP tutorials

[https://learn.hashicorp.com/collections/terraform/gcp-get-started#gcp](https://learn.hashicorp.com/collections/terraform/gcp-get-started#gcp)

### Provisioning Anthos clusters with Terraform

https://cloud.google.com/architecture/provisioning-anthos-clusters-with-terraform



### Manage GCP projects with terraform

https://cloud.google.com/community/tutorials/managing-gcp-projects-with-terraform

Discuss whether the project is the right unit of delivery.  There are resources that are bound to the projects.
Is it wise to have a long running project that must be kept alive for months or years? When can one delete such a project?
Are there any resources that can only be removed when project is removed?  (Hint: dataflow jobs, firestore database, scattered IAM service accounts, ... ).  What does it mean to deliver terraform for resources inside a project?   Should the unit of delivery be at a minimum the whole project?


https://github.com/GoogleCloudPlatform/community/tree/master/tutorials/managing-gcp-projects-with-terraform

### Terraform Google modules Examples

[https://github.com/terraform-google-modules/docs-examples](https://github.com/terraform-google-modules/docs-examples)



### Terraform examples for GKE

https://github.com/terraform-google-modules/terraform-google-kubernetes-engine/tree/master/examples/deploy_service


### Terraform, GKE, and network policy add-on

Problems that occur when there are too many layers of abstraction happening without considering affects that permeate through the layers and assumptions made in each layer.

https://blog.ml6.eu/how-proper-default-settings-can-save-money-and-trees-99783752d81c

### Cloud Foundation terraform templates

https://github.com/GoogleCloudPlatform/cloud-foundation-toolkit/blob/master/docs/terraform.md

### Integrate GCP with Datadog using terraform

https://medium.com/sardineai/integrating-gcp-with-datadog-with-terraform-d88c5c65dc0a

## Tools


### Terraformer

Reverse of terraform.  

[https://github.com/GoogleCloudPlatform/terraformer](https://github.com/GoogleCloudPlatform/terraformer)

### Terracognita

https://github.com/cycloidio/terracognita

### Terragrunt



https://terragrunt.gruntwork.io/



https://github.com/gruntwork-io/terragrunt

https://medium.com/bestmile/migrating-from-terraform-to-terragrunt-cf91f5d7a301

### Terratest

https://github.com/gruntwork-io/terratest

### Terraspace



https://terraspace.cloud/

### Atlantis

Terraform pull request automation

https://www.runatlantis.io/

### Spacelift

https://spacelift.io/

### Terraform validator

https://github.com/GoogleCloudPlatform/terraform-validator

### Terraform module generator


Scaffolding / Boilerplate generator for new Terraform module projects

https://github.com/sudokar/generator-tf-module

### Chekov

Terraform static analysis tool.

https://github.com/bridgecrewio/checkov/

### GitHub pre commit


https://github.com/antonbabenko/pre-commit-terraform

### Bridegecrew  

https://bridgecrew.io/


### Snyk

https://support.snyk.io/hc/en-us/articles/360010916577-Scan-and-fix-security-issues-in-your-Terraform-files

### Geodesic


https://github.com/cloudposse/geodesic

### Deep source

https://deepsource.io/static-analysis/terraform/

### Atmos

https://github.com/cloudposse/atmos

### Cloud Custodian

https://github.com/cloud-custodian/cloud-custodian

### Pulumi

https://www.pulumi.com/docs/intro/vs/terraform/


### CDK

[CDK](https://github.com/hashicorp/terraform-cdk) (Cloud Development Kit) for Terraform allows developers to use familiar programming languages to define cloud infrastructure and provision it through HashiCorp Terraform.

### Troposphere

https://github.com/cloudtools/troposphere

### Terrible

https://github.com/89luca89/terrible

https://github.com/antonbabenko/terrible

https://registry.terraform.io/modules/cloudboss/terrible/cloudinit/latest

## A list of URLs related to terraform

[https://github.com/shuaibiyy/awesome-terraform](https://github.com/shuaibiyy/awesome-terraform)




## Qwiklabs


### Terraform Quest

In this Quest, the experienced user of Google Cloud will learn how to describe and launch cloud resources with Terraform, an open source tool that codifies APIs into declarative configuration files that can be shared amongst team members, treated as code, edited, reviewed, and versioned. In these nine hands-on labs, you will work with example templates and understand how to launch a range of configurations, from simple servers, through full load-balanced applications.

[Managing Cloud Infrastructure with Terraform](https://www.qwiklabs.com/quests/44?catalog_rank=%7B%22rank%22%3A1%2C%22num_filters%22%3A1%2C%22has_search%22%3Atrue%7D&search_id=7467726)