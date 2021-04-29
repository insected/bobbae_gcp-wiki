- [Accounts & Billing](#accounts---billing)
  * [Concepts](#concepts)
    + [Important Roles](#important-roles)
    + [Resource Hierarchy](#resource-hierarchy)
    + [Projects, Folders, Labels](#projects--folders--labels)
    + [Relationships between Resources](#relationships-between-resources)
  * [Organizations](#organizations)
  * [Accounts](#accounts)
  * [Folders](#folders)
  * [Billing Account & Payment Profile](#billing-account---payment-profile)
  * [GCP Cloud Customer Onboarding Checklist](#gcp-cloud-customer-onboarding-checklist)
  * [Key Decisions](#key-decisions)
  * [Google Cloud Pricing Calculator](#google-cloud-pricing-calculator)
- [Channel Services](#channel-services)
  * [Channel Services console for Google Cloud Platform resale](#channel-services-console-for-google-cloud-platform-resale)
  * [Channel Services console for Google Workspace](#channel-services-console-for-google-workspace)
  * [Sub Accounts](#sub-accounts)
  * [Qwiklabs](#qwiklabs)
    + [Optimizing GCP Costs](#optimizing-gcp-costs)

<small><i><a href='http://ecotrust-canada.github.io/markdown-toc/'>Table of contents generated with markdown-toc</a></i></small>

## Accounts & Billing

A Cloud Billing account defines who pays for a given set of Google Cloud resources. To use Google Cloud services, you must have a valid Cloud Billing account, and must link it to your Google Cloud projects. Your project's Google Cloud usage is charged to the linked Cloud Billing account.

Google Cloud resources are organized hierarchically. This hierarchy allows you to map your organization's operational structure to Google Cloud, and to manage access control and permissions for groups of related resources.

### Concepts

In the context of Google Cloud, a resource can refer to the service-level resources that are used to process your workloads (VMs, DBs, and so on) as well as to the account-level resources that sit above the services, such as projects, folders, and the organization.

https://cloud.google.com/billing/docs/concepts

#### Important Roles

[https://cloud.google.com/billing/docs/concepts#important_roles](https://cloud.google.com/billing/docs/concepts#important_roles)


#### Resource Hierarchy

[https://cloud.google.com/resource-manager/docs/cloud-platform-resource-hierarchy#resource-hierarchy-detail](https://cloud.google.com/resource-manager/docs/cloud-platform-resource-hierarchy#resource-hierarchy-detail)


#### Projects, Folders, Labels

[https://cloud.google.com/billing/docs/onboarding-checklist#projects-folders-labels](https://cloud.google.com/billing/docs/onboarding-checklist#projects-folders-labels)


#### Relationships between Resources

Relationships between organizations, projects, Cloud Billing accounts, and payments profiles

[https://cloud.google.com/billing/docs/concepts#relationships-between-resources](https://cloud.google.com/billing/docs/concepts#relationships-between-resources)


### Organizations

[https://cloud.google.com/resource-manager/docs/creating-managing-organization](https://cloud.google.com/resource-manager/docs/creating-managing-organization)


### Accounts

[https://cloud.google.com/billing/docs/how-to/manage-billing-account](https://cloud.google.com/billing/docs/how-to/manage-billing-account)


### Folders

[https://cloud.google.com/resource-manager/docs/creating-managing-folders](https://cloud.google.com/resource-manager/docs/creating-managing-folders)


### Billing Account & Payment Profile

[https://cloud.google.com/billing/docs/concepts#billing_account](https://cloud.google.com/billing/docs/concepts#billing_account)


### GCP Cloud Customer Onboarding Checklist

Google Cloud customers can be assisted in setting up their various Google Cloud resources to avoid common issues and enable best practices for access control and cost management. There are some design decisions and configuration options that help set you up for success in administering your cloud resources.

[https://cloud.google.com/billing/docs/onboarding-checklist](https://cloud.google.com/billing/docs/onboarding-checklist)


### Key Decisions

[https://cloud.google.com/billing/docs/onboarding-checklist#cloud-billing-accounts](https://cloud.google.com/billing/docs/onboarding-checklist#cloud-billing-accounts)


### Google Cloud Pricing Calculator

[https://cloud.google.com/products/calculator](https://cloud.google.com/products/calculator)

Managing GCP usage and cost trends is easier than you think. In this session, we'll show you how to quickly view your GCP costs, forecast your month-end bill, and provide an overview of some of the controls you can put in place to prevent budget overruns.

[https://www.youtube.com/watch?v=UocD6uY2-js](https://www.youtube.com/watch?v=UocD6uY2-js)

## Channel Services

The Channel Services console is designed for resellers of Google Cloud products. Use the console to add customers, manage accounts, create orders, and other key tasks for reselling. 

 

### Channel Services console for Google Cloud Platform resale

https://support.google.com/channelservices/answer/9789535

### Channel Services console for Google Workspace


https://support.google.com/channelservices/answer/9400042

### Sub Accounts

Subaccounts are intended for resellers. If you are a reseller, you can use subaccounts to represent your customers' charges for the purpose of chargebacks.

Cloud Billing subaccounts allow you to group charges from projects together on a separate section of your invoice. A billing subaccount is a Cloud Billing account that is owned by a reseller's parent Cloud Billing account. The usage charges for all billing subacccounts are paid for by the reseller's parent Cloud Billing account. Note that the parent Cloud Billing account must be on invoiced billing.

A subaccount behaves like a Cloud Billing account in most ways: it can have projects linked to it, Cloud Billing data exports can be configured on it, and it can have IAM roles defined on it. Any charges made to projects linked to the subaccount are grouped and subtotalled on the invoice, and the effect on resource management is that access control policy can be entirely segregated on the subaccount to allow for customer separation and management.

https://cloud.google.com/billing/docs/concepts#subaccounts


### Qwiklabs


#### Optimizing GCP Costs

Here you'll learn several ways to control and optimize your GCP costs, including setting up budgets and alerts, managing quota limits, and taking advantage of committed use discounts. In the hands-on labs, you’ll practice using various tools to control and optimize your GCP costs or to influence your technology teams to apply the cost optimization best practices.

[Optimizing Your GCP Costs](https://www.qwiklabs.com/quests/97?catalog_rank=%7B%22rank%22%3A4%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&search_id=7468028)

