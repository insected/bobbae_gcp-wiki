Terraform is a tool from Hashicorp for building, changing, and versioning infrastructure safely and efficiently. Terraform can manage existing and popular service providers as well as custom in-house solutions.

Terraform is a widely used tool to create cloud infrastructure to public clouds — and this is Terraform’s most compelling pro: If you do multi-cloud development (as I do — AWS, GCP and Azure) it is a really powerful benefit to have one tool to create IaC for all three cloud platforms. Terraform also provides powerful declarative language (HCL) for creating IaC solutions. All major cloud services are supported in Terraform and usually new major services are supported pretty soon they are launched by the cloud provider.

Terraform is a declarative language but compared to other declarative languages used by some public cloud provider native IaC tools (like JSON or YAML) Terraform provides nice constructs to modularize your cloud resources into logical re-usable entities.

# Infrastructure as Code

Terraform's infrastructure-as-code (IAC) approach supports [DevOps](https://cloud.google.com/devops) best practices for change management, letting you manage Terraform configuration files in source control to maintain an ideal provisioning state for testing and production environments.

[https://cloud.google.com/docs/terraform](https://cloud.google.com/docs/terraform)

Google Cloud Deployment Manager allows you to specify all the resources needed for your application in a declarative format using yaml. On the other hand, Terraform is detailed as "Describe your complete infrastructure as code and build resources across providers".

[https://www.terraform.io/intro/index.html](https://www.terraform.io/intro/index.html)

# Using terraform with Google Cloud

https://cloud.google.com/docs/terraform

# Getting Started on GCP with terraform

[https://cloud.google.com/community/tutorials/getting-started-on-gcp-with-terraform](https://cloud.google.com/community/tutorials/getting-started-on-gcp-with-terraform)

Defining and managing your development, test, staging, and production environments using infra-as-code tools such as [Deployment Manager](https://cloud.google.com/deployment-manager) or [Terraform](https://www.terraform.io/) is a common practice. Ensuring that any changes you make to your environment config definitions are “safe” remains challenging, though.

[https://www.youtube.com/watch?v=3vfXQxWJazM](https://www.youtube.com/watch?v=3vfXQxWJazM)


# Managing infrastructure as code with Terraform, Cloud Build, and GitOps

[https://cloud.google.com/solutions/managing-infrastructure-as-code](https://cloud.google.com/solutions/managing-infrastructure-as-code)


# Hashicorp  terraform on GCP tutorials

[https://learn.hashicorp.com/collections/terraform/gcp-get-started#gcp](https://learn.hashicorp.com/collections/terraform/gcp-get-started#gcp)


# Terraform Modules for GCP

[https://github.com/terraform-google-modules](https://github.com/terraform-google-modules)


# Manage GCP projects with terraform

https://cloud.google.com/community/tutorials/managing-gcp-projects-with-terraform

<img src="https://storage.googleapis.com/gcp-community/tutorials/managing-gcp-projects-with-terraform/diagram.png" width="800">

https://github.com/GoogleCloudPlatform/community/tree/master/tutorials/managing-gcp-projects-with-terraform

# Terraform Google modules Examples

[https://github.com/terraform-google-modules/docs-examples](https://github.com/terraform-google-modules/docs-examples)


# Terraformer

Reverse of terraform.  

[https://github.com/GoogleCloudPlatform/terraformer](https://github.com/GoogleCloudPlatform/terraformer)

# Terragrunt

Terragrunt is a thin wrapper that provides extra tools for keeping your configurations DRY, working with multiple Terraform modules, and managing remote state.

https://terragrunt.gruntwork.io/

# A list of URLs related to terraform

[https://github.com/shuaibiyy/awesome-terraform](https://github.com/shuaibiyy/awesome-terraform)


# Qwiklabs


## Terraform Quest

In this Quest, the experienced user of Google Cloud will learn how to describe and launch cloud resources with Terraform, an open source tool that codifies APIs into declarative configuration files that can be shared amongst team members, treated as code, edited, reviewed, and versioned. In these nine hands-on labs, you will work with example templates and understand how to launch a range of configurations, from simple servers, through full load-balanced applications.

[Managing Cloud Infrastructure with Terraform](https://www.qwiklabs.com/quests/44?catalog_rank=%7B%22rank%22%3A1%2C%22num_filters%22%3A1%2C%22has_search%22%3Atrue%7D&search_id=7467726)