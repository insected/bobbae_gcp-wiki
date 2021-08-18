[Terraform](https://terraform.io) is a tool from Hashicorp for building, changing, and versioning infrastructure safely and efficiently. Terraform can manage existing and popular service providers as well as custom in-house solutions.


## Infrastructure as Code

[Infrastructure as Code](Infrastructure-as-Code)  is the process of managing and provisioning computer data centers through machine-readable definition files, rather than physical hardware configuration or interactive configuration tools.

Terraform's infrastructure-as-code (IAC) approach supports [DevOps](https://cloud.google.com/devops) best practices for change management, letting you manage Terraform configuration files in source control to maintain an ideal provisioning state for testing and production environments.



[https://www.terraform.io/intro/index.html](https://www.terraform.io/intro/index.html)

## Cloud Foundation Toolkit

Google Cloud Foundation Toolkit supports Terraform as well as Google Cloud Deployment manager.

[Cloud Foundation Toolkit](Cloud-Foundation-Toolkit)

## Using terraform with Google Cloud

https://cloud.google.com/docs/terraform

## Provisioning Anthos clusters with Terraform

https://cloud.google.com/architecture/provisioning-anthos-clusters-with-terraform


## Terraform examples for GKE

https://github.com/terraform-google-modules/terraform-google-kubernetes-engine/tree/master/examples/deploy_service


### Terraform, GKE, and network policy add-on

Problems that occur when there are too many layers of abstraction happening without considering affects that permeate through the layers and assumptions made in each layer.

https://blog.ml6.eu/how-proper-default-settings-can-save-money-and-trees-99783752d81c

## Cloud Foundation terraform templates

https://github.com/GoogleCloudPlatform/cloud-foundation-toolkit/blob/master/docs/terraform.md

## Getting Started on GCP with terraform

[https://cloud.google.com/community/tutorials/getting-started-on-gcp-with-terraform](https://cloud.google.com/community/tutorials/getting-started-on-gcp-with-terraform)

Defining and managing your development, test, staging, and production environments using infra-as-code tools such as [Deployment Manager](https://cloud.google.com/deployment-manager) or [Terraform](https://www.terraform.io/) is a common practice. Ensuring that any changes you make to your environment config definitions are “safe” remains challenging, though.

[https://www.youtube.com/watch?v=3vfXQxWJazM](https://www.youtube.com/watch?v=3vfXQxWJazM)


## Managing infrastructure as code with Terraform, Cloud Build, and GitOps

[https://cloud.google.com/solutions/managing-infrastructure-as-code](https://cloud.google.com/solutions/managing-infrastructure-as-code)


## Hashicorp  terraform on GCP tutorials

[https://learn.hashicorp.com/collections/terraform/gcp-get-started#gcp](https://learn.hashicorp.com/collections/terraform/gcp-get-started#gcp)


## Terraform Modules for GCP

[https://github.com/terraform-google-modules](https://github.com/terraform-google-modules)


## Manage GCP projects with terraform

https://cloud.google.com/community/tutorials/managing-gcp-projects-with-terraform

Discuss whether the project is the right unit of delivery.  There are resources that are bound to the projects.
Is it wise to have a long running project that must be kept alive for months or years? When can one delete such a project?
Are there any resources that can only be removed when project is removed?  (Hint: dataflow jobs, firestore database, scattered IAM service accounts, ... ).  What does it mean to deliver terraform for resources inside a project?   Should the unit of delivery be at a minimum the whole project?


https://github.com/GoogleCloudPlatform/community/tree/master/tutorials/managing-gcp-projects-with-terraform

## Terraform Google modules Examples

[https://github.com/terraform-google-modules/docs-examples](https://github.com/terraform-google-modules/docs-examples)


## CDK

[CDK](https://github.com/hashicorp/terraform-cdk) (Cloud Development Kit) for Terraform allows developers to use familiar programming languages to define cloud infrastructure and provision it through HashiCorp Terraform.

## Terraformer

Reverse of terraform.  

[https://github.com/GoogleCloudPlatform/terraformer](https://github.com/GoogleCloudPlatform/terraformer)

## Terragrunt



https://terragrunt.gruntwork.io/


## Terraspace



https://terraspace.cloud/

## Atlantis

Terraform pull request automation

https://www.runatlantis.io/

## Terraform validator

https://github.com/GoogleCloudPlatform/terraform-validator

## A list of URLs related to terraform

[https://github.com/shuaibiyy/awesome-terraform](https://github.com/shuaibiyy/awesome-terraform)

## Integrate GCP with Datadog using terraform

https://medium.com/sardineai/integrating-gcp-with-datadog-with-terraform-d88c5c65dc0a

## Qwiklabs


### Terraform Quest

In this Quest, the experienced user of Google Cloud will learn how to describe and launch cloud resources with Terraform, an open source tool that codifies APIs into declarative configuration files that can be shared amongst team members, treated as code, edited, reviewed, and versioned. In these nine hands-on labs, you will work with example templates and understand how to launch a range of configurations, from simple servers, through full load-balanced applications.

[Managing Cloud Infrastructure with Terraform](https://www.qwiklabs.com/quests/44?catalog_rank=%7B%22rank%22%3A1%2C%22num_filters%22%3A1%2C%22has_search%22%3Atrue%7D&search_id=7467726)