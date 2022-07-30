[Terraform](https://terraform.io) is a tool  for building, changing, and versioning infrastructure. Terraform can manage existing a service providers as well as custom in-house solutions.

## Cloud Foundation Toolkit

[Google Cloud Foundation Toolkit](Cloud-Foundation-Toolkit) supports Terraform as well as Google Cloud Deployment manager.


## Infrastructure as Code

[Infrastructure as Code](Infrastructure-as-Code)  is the process of managing and provisioning computer data centers through [machine-readable definition](https://www.mineiros.io/blog/the-ultimate-guide-on-how-to-write-terraform-modules-part-1) files, rather than physical hardware configuration or interactive configuration tools.



Terraform's [infrastructure-as-code](Infrastructure-as-Code)  (IAC) approach supports [DevOps](DevOps) best practices for change management, letting you manage Terraform configuration files in source control to maintain an ideal provisioning state for testing and production environments.

### Best Practices


https://geekflare.com/terraform-best-practices/

### Terraform Blueprints

https://cloud.google.com/docs/terraform/blueprints/terraform-blueprints

### terraform docker image

https://hub.docker.com/r/hashicorp/terraform/

### Gcloud and terraform

https://cloud.google.com/blog/products/application-development/google-cloud-cli-declarative-export-preview

### RAD Lab

https://github.com/GoogleCloudPlatform/rad-lab

### Immutable infrastructure

The benefits of an [immutable infrastructure](https://www.digitalocean.com/community/tutorials/what-is-immutable-infrastructure) include more consistency and reliability in your infrastructure and a simpler, more predictable deployment process. 


### HCL

https://www.terraform.io/docs/language/index.html



Defining and managing your development, test, staging, and production environments using infra-as-code tools such as [Deployment Manager](https://cloud.google.com/deployment-manager) or [Terraform](https://www.terraform.io/) is a common practice. 

[https://www.youtube.com/watch?v=3vfXQxWJazM](https://www.youtube.com/watch?v=3vfXQxWJazM)

[https://www.terraform.io/intro/index.html](https://www.terraform.io/intro/index.html)

### Policy validation

https://cloud.google.com/docs/terraform/policy-validation


### Terraform JSON support

https://www.terraform.io/docs/language/syntax/json.html

### Module

A Terraform module is a set of Terraform configuration files in a single directory. Even a simple configuration consisting of a single directory with one or more .tf files is a module. When you run Terraform commands directly from such a directory, it is considered the root module. So in this sense, every Terraform configuration is part of a module. 

https://registry.terraform.io/browse/modules

### Using terraform with Google Cloud

https://cloud.google.com/docs/terraform

### Importing resources from gcloud to Terraform

How to import manually created resources using gcloud into terraform?

https://teracloud.medium.com/google-cloud-importing-resources-from-the-gcloud-to-iaac-in-terraform-b25a05787144

### Encoring Policy as Code using Atlantis

https://tech.loveholidays.com/enforcing-best-practice-on-self-serve-infrastructure-with-terraform-atlantis-and-policy-as-code-911f4f8c3e00

### Selective deployment

https://github.com/GoogleCloudPlatform/professional-services/tree/main/examples/cloudbuild-selective-deployment

## Extending terraform 

### Plugins

https://www.terraform.io/docs/extend/how-terraform-works.html

### Custom Providers

https://www.terraform.io/docs/extend/hashicorp-provider-design-principles.html




## Using terraform

https://www.digitalocean.com/community/tutorial_series/how-to-manage-infrastructure-with-terraform




### Loops and conditions

https://blog.gruntwork.io/terraform-tips-tricks-loops-if-statements-and-gotchas-f739bbae55f9


### Troubleshooting

https://learn.hashicorp.com/tutorials/terraform/troubleshooting-workflow


### Mistakes


https://blog.pipetail.io/posts/2020-10-29-most-common-mistakes-terraform/

### state

https://tryingthings.wordpress.com/2021/03/31/lessons-learned-after-losing-the-terraform-state-file/

https://medium.com/@moabu/oops-deleted-the-terraform-state-file-imported-the-resource-but-now-it-wants-to-recreate-it-1695e9b6e8

### Pain points



https://adambrodziak.pl/terraform-is-terrible

### Issues

https://www.schibsted.pl/blog/9-reasons-why-terraform-is-a-pain-and-1-why-you-should-still-care/

### Debugging terraform

https://www.terraform.io/docs/internals/debugging.html

#### Debug a Terraform Provider

https://learn.hashicorp.com/tutorials/terraform/provider-debug




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
Is it wise to have a long-running project that must be kept alive for months or years? When can one delete such a project?
Are there any resources that can only be removed when the project is removed?  (Hint: dataflow jobs, Firestore database, scattered IAM service accounts, ... ).  What does it mean to deliver terraform for resources inside a project?   Should the unit of delivery be at a minimum the whole project?


https://github.com/GoogleCloudPlatform/community/tree/master/tutorials/managing-gcp-projects-with-terraform


### Terraform, GKE, and network policy add-on

Problems that occur when there are too many layers of abstraction happening without considering affects that permeate through the layers and assumptions made in each layer.

https://blog.ml6.eu/how-proper-default-settings-can-save-money-and-trees-99783752d81c

### Cloud Foundation terraform templates

https://github.com/GoogleCloudPlatform/cloud-foundation-toolkit/blob/master/docs/terraform.md

### Integrate GCP with Datadog using terraform

https://medium.com/sardineai/integrating-gcp-with-datadog-with-terraform-d88c5c65dc0a

### Google Cloud security foundations guide

CFT Terraform modules can be composed to build a secure GCP foundation, following the [Google Cloud security foundations guide](  https://services.google.com/fh/files/misc/google-cloud-security-foundations-guide.pdf
 ) .

https://github.com/terraform-google-modules/terraform-example-foundation

## Tools


### Infracost

https://Infracost.io

### Terraformer

Reverse of terraform.  

[https://github.com/GoogleCloudPlatform/terraformer](https://github.com/GoogleCloudPlatform/terraformer)

#### Gcloud resource-config bulk-export

https://www.teracloud.io/single-post/google-cloud-importing-resources-from-the-gcloud-to-iaac-in-terraform

#### Bulk import and export of existing Google resources


https://cloud.google.com/config-connector/docs/how-to/import-export/bulk-export

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

### Env0

https://www.env0.com/

### Spacelift

https://spacelift.io/

### Terraform validator

https://github.com/GoogleCloudPlatform/terraform-validator

#### Terraform Validator tutorial

https://github.com/GoogleCloudPlatform/terraform-validator/blob/main/docs/tutorial.md

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

[CDK](https://github.com/hashicorp/terraform-cdk) (Cloud Development Kit) for Terraform allows developers to use familiar programming languages to define cloud infrastructure and provision it through Terraform.

https://cdk.dev/

https://github.com/hashicorp/terraform-cdk

https://learn.hashicorp.com/tutorials/terraform/cdktf

https://dev.to/michael_lin/deploy-infrastructure-using-cdk-for-terraform-with-go-28ne

### Troposphere

https://github.com/cloudtools/troposphere

### Terrible

https://github.com/89luca89/terrible

https://github.com/antonbabenko/terrible

https://registry.terraform.io/modules/cloudboss/terrible/cloudinit/latest

## A list of URLs related to terraform

[https://github.com/shuaibiyy/awesome-terraform](https://github.com/shuaibiyy/awesome-terraform)


## Terraform associate certification


https://www.freecodecamp.org/news/hashicorp-terraform-associate-certification-study-course-pass-the-exam-with-this-free-12-hour-course/


## Examples

### Creating a VM

#### Create a VM using GCP Console

https://cloud.google.com/compute/docs/instances/create-start-instance

#### Create a VM using gcloud CLI

https://cloud.google.com/compute/docs/instances/create-start-instance#gcloud

#### Create a VM using REST API

https://cloud.google.com/compute/docs/instances/create-start-instance#startinstanceapi

#### Create a VM using Python 

https://cloud.google.com/compute/docs/instances/create-start-instance#python


#### Create a VM using Terraform

https://cloud.google.com/community/tutorials/getting-started-on-gcp-with-terraform

### Terraform Google modules

https://github.com/terraform-google-modules

### Terraform Cloud Foundation Fabric Examples

https://vaishnavi-amirapu-83592.medium.com/terraform-cft-for-gcp-664fa3c68ae3

https://github.com/terraform-google-modules/cloud-foundation-fabric

### Service Account impersonation in your Terraform code

https://cloud.google.com/blog/topics/developers-practitioners/using-google-cloud-service-account-impersonation-your-terraform-code


### Terraform Google modules Examples

[https://github.com/terraform-google-modules/docs-examples](https://github.com/terraform-google-modules/docs-examples)

### Create GCP VM instance

https://sanket-wadekar3.medium.com/create-gcp-vm-instance-using-terraform-d14d3887445b

### Terraform examples: VPC, Subnets, Firewalls, Routes, IAP Tunnel, Internet Gateway, Cloud NAT and Cloud Router 
https://medium.com/@nanditasahu031/terraform-with-gcp-cloud-d25d60a6e740

### Terraform examples for GKE

https://github.com/GoogleCloudPlatform/gke-private-cluster-demo


https://devopsarena.medium.com/provision-gke-cluster-with-terraform-28bf2973c3d4


https://github.com/terraform-google-modules/terraform-google-kubernetes-engine/tree/master/examples/deploy_service


### Provisioning Spanner with Terraform

https://cloud.google.com/blog/topics/developers-practitioners/provisioning-cloud-spanner-using-terraform

### Triggering Cloud functions using Cloud Schedulers with Terraform

https://medium.com/geekculture/setup-gcp-cloud-functions-triggering-by-cloud-schedulers-with-terraform-1433fbf1abbe

### CI/CD Pipeline with Cloud Build and Composer

https://medium.com/marcelo-marques/ci-cd-pipeline-with-cloud-build-and-composer-with-terraform-379a05a4ca09



### GKE cluster with LB, NAT and Bastion host

https://orlando-thoeny.medium.com/create-a-private-gcp-kubernetes-cluster-using-terraform-1a830dd802a8

### Automating Terraform with GitHub Actions

https://blog.searce.com/automating-terraform-with-github-actions-5b3aac5abea7

### Typhoon

https://github.com/poseidon/typhoon


### CICD Pipeline as Code using Terraform

[CICD](CICD) Pipeline set up in Terraform.

https://genekuo.medium.com/setting-up-a-ci-cd-pipeline-on-gcp-with-terraform-539e66797072

### Eventarc trigger with terraform

https://cloud.google.com/blog/topics/developers-practitioners/creating-eventarc-triggers-terraform

### Terraform Google Load Balancer examples

https://github.com/terraform-google-modules/terraform-google-lb-http/tree/master/examples

### GCP integration with PagerDuty using Terraform

https://medium.com/storyteltech/gcp-integration-with-pagerduty-using-terraform-257db26363f9




## Qwiklabs



[Automating Infrastructure on Google Cloud with Terraform](https://www.qwiklabs.com/quests/159)

[Managing Cloud Infrastructure with Terraform](https://www.qwiklabs.com/quests/44?catalog_rank=%7B%22rank%22%3A1%2C%22num_filters%22%3A1%2C%22has_search%22%3Atrue%7D&search_id=7467726)

[Interact with Terraform Modules](https://www.qwiklabs.com/focuses/15836?parent=catalog)

[Building a VPN Between Google Cloud and AWS with Terraform](https://www.qwiklabs.com/focuses/17869?parent=catalog)