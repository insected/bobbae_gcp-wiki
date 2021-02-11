
- [Infrastructure as Code](#infrastructure-as-code)
  * [Introduction](#introduction)
    + [Google Cloud Deployment Manager](#google-cloud-deployment-manager)
      - [Cloud Deployment Quickstart](#cloud-deployment-quickstart)
      - [Deployments](#deployments)
      - [Manifests](#manifests)
      - [Cloud Deployment Manager Deploying Network Load Balanced Logbook](#cloud-deployment-manager-deploying-network-load-balanced-logbook)
      - [Shard VPC with Cloud Deployment Manager](#shard-vpc-with-cloud-deployment-manager)
      - [Solutions that use Cloud Deployment Manager](#solutions-that-use-cloud-deployment-manager)
      - [More examples](#more-examples)
    + [Cloud Foundation Toolkit](#cloud-foundation-toolkit)
  * [Terraform](#terraform)
    + [Introduction](#introduction-1)
    + [Getting Started on GCP](#getting-started-on-gcp)
      - [Managing infrastructure as code with Terraform, Cloud Build, and GitOps](#managing-infrastructure-as-code-with-terraform--cloud-build--and-gitops)
      - [Hashicorp tutorials](#hashicorp-tutorials)
      - [Terraform Modules for GCP](#terraform-modules-for-gcp)
      - [Examples](#examples)
    + [Terraformer](#terraformer)
    + [A list of URLs related to terraform](#a-list-of-urls-related-to-terraform)
  * [Pulumi](#pulumi)
  * [Ansible](#ansible)
  * [Qwiklabs](#qwiklabs)
    + [Terraform Quest](#terraform-quest)
    + [Terraform](#terraform-1)
    + [VM Migration](#vm-migration)

<small><i><a href='http://ecotrust-canada.github.io/markdown-toc/'>Table of contents generated with markdown-toc</a></i></small>

## Infrastructure as Code


### Introduction

Provisioning compute resources has traditionally been hard to manage, not scalable, and prone to error, so what other techniques can you use to make sure you’re ready to meet demand? In this episode of Season of Scale, Stephanie Wong explains why you should adopt an Infrastructure as code (IaC) strategy, so you can automate the creation of your cloud resources, create templates, and store config files with the help of tools like Google Cloud Deployment Manager.

[https://cloud.google.com/solutions/infrastructure-as-code](https://cloud.google.com/solutions/infrastructure-as-code)


#### Google Cloud Deployment Manager

[https://www.youtube.com/watch?v=z-caqPtEw58](https://www.youtube.com/watch?v=z-caqPtEw58)


##### Cloud Deployment Quickstart

[https://cloud.google.com/deployment-manager/docs/quickstart](https://cloud.google.com/deployment-manager/docs/quickstart)


##### Deployments

[https://cloud.google.com/deployment-manager/docs/deployments](https://cloud.google.com/deployment-manager/docs/deployments)


##### Manifests

[https://cloud.google.com/deployment-manager/docs/deployments/viewing-manifest](https://cloud.google.com/deployment-manager/docs/deployments/viewing-manifest)


##### Cloud Deployment Manager Deploying Network Load Balanced Logbook 

[https://cloud.google.com/deployment-manager/docs/create-advanced-deployment](https://cloud.google.com/deployment-manager/docs/create-advanced-deployment)


##### Shard VPC with Cloud Deployment Manager

[https://cloud.google.com/solutions/shared-vpc-with-deployment-manager](https://cloud.google.com/solutions/shared-vpc-with-deployment-manager)


##### Solutions that use Cloud Deployment Manager

[https://cloud.google.com/docs/tutorials?sortBy=relevance#%22deployment%20manager%22](https://cloud.google.com/docs/tutorials?sortBy=relevance#%22deployment%20manager%22)


##### More examples

[https://github.com/GoogleCloudPlatform/deploymentmanager-samples/tree/master/examples/v2](https://github.com/GoogleCloudPlatform/deploymentmanager-samples/tree/master/examples/v2)


#### Cloud Foundation Toolkit

The Cloud Foundation Toolkit provides a series of reference templates for Deployment Manager and Terraform which reflect Google Cloud best practices. These templates can be used off-the-shelf to quickly build a repeatable enterprise-ready foundation in Google Cloud. This frees you to focus on deploying your applications on this baseline secure environment. And with infrastructure as code (IaC), you can easily update the foundation as your needs change.

[https://cloud.google.com/foundation-toolkit/](https://cloud.google.com/foundation-toolkit/)


The [Cloud Foundation toolkit](https://github.com/GoogleCloudPlatform/cloud-foundation-toolkit) (henceforth, CFT) includes the following parts:

- A comprehensive set of production-ready resource templates that follow
  Google's best practices, which can be used with the CFT or the gcloud
  utility (part of the Google Cloud SDK) - see
  [the template directory](dm/templates/)
- A command-line interface (henceforth, CLI) that deploys resources defined in
  single or multiple CFT-compliant config files - see:
  - The CFT source Python files (the `src/` directory)
  - The [CFT DM User Guide](dm/docs/userguide.md)
- A growing set of sample [Config
  Connector](https://cloud.google.com/config-connector/docs/overview)
  YAML configurations - see [the solutions directory](config-connector/solutions/)

In addition, the CFT repository includes a sample pipeline that enables running
CFT deployment operations from Jenkins.


### Terraform 


#### Introduction

Terraform's infrastructure-as-code (IaC) approach supports [DevOps](https://cloud.google.com/devops) best practices for change management, letting you manage Terraform configuration files in source control to maintain an ideal provisioning state for testing and production environments.

[https://cloud.google.com/docs/terraform](https://cloud.google.com/docs/terraform)

Terraform is a tool from Hashicorp for building, changing, and versioning infrastructure safely and efficiently. Terraform can manage existing and popular service providers as well as custom in-house solutions.

[https://www.terraform.io/intro/index.html](https://www.terraform.io/intro/index.html)


#### Getting Started on GCP

[https://cloud.google.com/community/tutorials/getting-started-on-gcp-with-terraform](https://cloud.google.com/community/tutorials/getting-started-on-gcp-with-terraform)

Defining and managing your development, test, staging, and production environments using infra-as-code tools such as [Deployment Manager](https://cloud.google.com/deployment-manager) or [Terraform](https://www.terraform.io/) is a common practice. Ensuring that any changes you make to your environment config definitions are “safe” remains challenging, though.

[https://www.youtube.com/watch?v=3vfXQxWJazM](https://www.youtube.com/watch?v=3vfXQxWJazM)


##### Managing infrastructure as code with Terraform, Cloud Build, and GitOps

[https://cloud.google.com/solutions/managing-infrastructure-as-code](https://cloud.google.com/solutions/managing-infrastructure-as-code)


##### Hashicorp tutorials

[https://learn.hashicorp.com/collections/terraform/gcp-get-started#gcp](https://learn.hashicorp.com/collections/terraform/gcp-get-started#gcp)


##### Terraform Modules for GCP

[https://github.com/terraform-google-modules](https://github.com/terraform-google-modules)


##### Examples

[https://github.com/terraform-google-modules/docs-examples](https://github.com/terraform-google-modules/docs-examples)


#### Terraformer

Reverse of terraform.  

[https://github.com/GoogleCloudPlatform/terraformer](https://github.com/GoogleCloudPlatform/terraformer)


#### A list of URLs related to terraform

[https://github.com/shuaibiyy/awesome-terraform](https://github.com/shuaibiyy/awesome-terraform)


### Pulumi

[https://www.pulumi.com/docs/get-started/gcp/](https://www.pulumi.com/docs/get-started/gcp/)


### Ansible

An opinionated look at how ansible and terraform complement one another in a provisioner/configuration management separated view. A key takeaway is a simplified workflow for sysadmins/operators in cloud management that can be applied in multi-cloud/hybrid cloud scenarios.

[https://www.youtube.com/watch?v=utztQWTewWU](https://www.youtube.com/watch?v=utztQWTewWU)


### Qwiklabs


#### Terraform Quest

[https://www.qwiklabs.com/quests/44](https://www.qwiklabs.com/quests/44)


#### Terraform

In this Quest, the experienced user of Google Cloud will learn how to describe and launch cloud resources with Terraform, an open source tool that codifies APIs into declarative configuration files that can be shared amongst team members, treated as code, edited, reviewed, and versioned. In these nine hands-on labs, you will work with example templates and understand how to launch a range of configurations, from simple servers, through full load-balanced applications.

[Managing Cloud Infrastructure with Terraform](https://www.qwiklabs.com/quests/44?catalog_rank=%7B%22rank%22%3A1%2C%22num_filters%22%3A1%2C%22has_search%22%3Atrue%7D&search_id=7467726)


#### VM Migration

Google Cloud’s four step structured Cloud Migration Path Methodology provides a defined and repeatable path for users to follow when migrating and modernizing Virtual Machines. In this quest, you will get hands-on practice with Google’s current solution set for VM assessment, planning, migration, and modernization. You will start by analyzing your lab environment and building assessment reports with CloudPhysics and StratoZone, then build a landing zone within Google Cloud leveraging Terraform’s infrastructure-as-code templates, next you will manually transform a two-tier application into a cloud-native workload running on Kubernetes, and finally, transform a VM workload into Kubernetes with Migrate for Anthos and migrate a VM between cloud environments.

[VM Migration](https://www.qwiklabs.com/quests/87?catalog_rank=%7B%22rank%22%3A2%2C%22num_filters%22%3A1%2C%22has_search%22%3Atrue%7D&search_id=7467726)
