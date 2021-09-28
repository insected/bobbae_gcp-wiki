## IAM Overview


[Cloud IAM](https://cloud.google.com/iam/docs/overview) is Google Cloud Platform’s unified system for managing access to resources and assigning permissions for users and services to access those resources.  This video will take you through the basic terms and concepts you need to use Cloud IAM.

Limiting the use of service accounts and service account keys to situations in which [they're absolutely necessary](https://cloud.google.com/blog/products/identity-security/how-to-authenticate-service-accounts-to-help-keep-applications-secure) keeps user data more secure, reduces the chance of unauthorized activity, and makes it easier to use audit logs to determine which users performed certain operations.

## Access Control 

Prior to Cloud IAM, you could only grant Owner, Editor, or Viewer [roles](https://cloud.google.com/iam/docs/understanding-roles) to users. A wide range of services and resources now surface additional Cloud IAM roles out of the box. For example, the Pub/Sub service exposes Publisher and Subscriber roles in addition to the [Owner, Editor, and Viewer roles](https://cloud.google.com/iam/docs/understanding-roles#basic-definitions). 



## How IAM works

With [IAM](https://cloud.google.com/iam/docs/overview#how_cloud_iam_works), you manage access control by defining who (identity) has what access (role) for which resource. For example, Compute Engine virtual machine instances, Google Kubernetes Engine (GKE) clusters, and Cloud Storage buckets are all Google Cloud resources. The organizations, folders, and projects that you use to organize your resources are also resources.

### IAM Model

In IAM, permission to access a resource isn't granted directly to the end user. Instead, permissions are grouped into [roles](https://cloud.google.com/iam/docs/understanding-roles), and roles are granted to authenticated members. An IAM [policy](https://cloud.google.com/iam/docs/policies) defines and enforces what roles are granted to which members, and this policy is attached to a resource. When an authenticated member attempts to access a resource, IAM checks the resource's policy to determine whether the action is permitted.



### Model for Access management

#### Member

A member can be a Google Account (for end users), a [service account](Service-Accounts) (for apps and virtual machines), a Google group, or a Google Workspace or Cloud Identity domain that can access a resource. The identity of a member is an email address associated with a user, service account, or Google group; or a domain name associated with Google Workspace or Cloud Identity domains.


#### Role


A [role](https://cloud.google.com/iam/docs/understanding-roles) is a collection of permissions. Permissions determine what operations are allowed on a resource. When you grant a role to a member, you grant all the permissions that the role contains.

https://cloud.google.com/iam/docs/understanding-roles


#### Custom roles

https://cloud.google.com/iam/docs/understanding-custom-roles

#### Policy


The [IAM policy](https://cloud.google.com/iam/docs/policies) binds one or more members to a role. When you want to define who (member) has what type of access (role) on a resource, you create a [policy](https://cloud.google.com/iam/docs/policies) and attach it to the resource.

Access control for Google Cloud resources is managed by Identity and Access Management (IAM) policies, which are attached to resources. You can attach only one IAM policy to each resource. The IAM policy controls access to the resource itself, as well as any descendants of that resource that inherit the policy.





#### Policy intelligence tools

Large organizations often have complicated Identity and Access Management (IAM) policies. [Policy Intelligence tools](https://cloud.google.com/iam/docs/policy-intelligence-tools)  help you understand and manage your policies to proactively improve your security configuration.

## Service Accounts


A [service account](Service-Accounts) is a special kind of account used by an application or a virtual machine (VM) instance, not a person. Applications use service accounts to make authorized API calls, authorized as either the service account itself, or as Google Workspace or Cloud Identity users through domain-wide delegation.



https://cloud.google.com/iam/docs/service-accounts



## Service agents

Some Google Cloud services have Google-managed service accounts that allow the services to access your resources. These service accounts are sometimes known as service agents.

https://cloud.google.com/iam/docs/service-agents


## Granular Access

IAM lets you grant granular access to specific Google Cloud resources and helps prevent access to other resources. IAM lets you adopt the security principle of least privilege, which states that nobody should have more permissions than they actually need.

https://cloud.google.com/resource-manager/docs/access-control-proj

## Resources


Cloud Identity and Access Management (IAM) lets administrators authorize who can take action on specific resources, giving you full control and visibility to manage Google Cloud resources centrally. For enterprises with complex organizational structures, hundreds of workgroups, and many projects, Cloud IAM provides a unified view into security policy across your entire organization, with built-in [auditing](https://cloud.google.com/iam/docs/audit-logging)  to ease compliance processes. 

[https://www.youtube.com/watch?v=96HlT4f2AUU](https://www.youtube.com/watch?v=96HlT4f2AUU)

### Resource hierarchy


https://cloud.google.com/resource-manager/docs/cloud-platform-resource-hierarchy

## Delegated role grants

[Delegated role grants](https://cloud.google.com/iam/docs/setting-limits-on-granting-roles) is a new feature in GCP that allows organization administrators to control which roles a user can grant or revoke even when the user has setIamPolicy permission on a resource.

https://medium.com/google-cloud/managing-gcp-service-usage-through-delegated-role-grants-a843610f2226


## Concepts related to identity

In [IAM you grant access](https://cloud.google.com/iam/docs/overview#concepts_related_identity) to members. Members can have the following types: Google Account, Service Account, Google Group, Google Workspace domain, Cloud Identity Domain, All authenticated users, All users.


### Google Groups

[Google Groups](https://cloud.google.com/iam/docs/groups-in-cloud-console) is a service from Google that provides discussion groups for people sharing common interests. The Groups service also provides a gateway to Usenet newsgroups via a shared user interface.

Google Groups became operational in February 2001, following Google's acquisition of Deja's Usenet archive. Deja News had been operational since March 1995.

[Usenet](https://en.wikipedia.org/wiki/Usenet)  is a worldwide distributed discussion system available on computers. It was developed from the general-purpose Unix-to-Unix Copy (UUCP) dial-up network architecture. Tom Truscott and Jim Ellis conceived the idea in 1979, and it was established in 1980.




## Recommender

[Recommender](https://cloud.google.com/iam/docs/recommender-overview) is a service on Google Cloud that provides usage recommendations and insights for Cloud products and services.




### IAM Recommender

IAM uses Recommender to compare role grants with the permissions that each member used during the past 90 days. If you grant a role to a member, and the member does not use all of that role's permissions, then the IAM recommender is likely to recommend that you revoke the role. If necessary, the IAM recommender also recommends less permissive roles as a replacement. This suggested replacement could be a new custom role, an existing custom role, or one or more predefined roles. Except in the case of recommendations for Google-managed service accounts, the IAM recommender never suggests a change that increases a member's level of access.

https://cloud.google.com/iam/docs/recommender-overview

### Managing insights

In addition to providing recommendations, Recommender uses machine learning (ML) to provide detailed insights. [Insights](https://cloud.google.com/iam/docs/managing-insights) are findings that highlight notable patterns in resource usage. For example, you can collect additional information about permission usage in your project, or identify unused service accounts. Some insights also link to recommendations, because the insights provide evidence for the recommendations.


https://cloud.google.com/iam/docs/manage-service-account-insights


## Audit

Google Cloud services write [audit logs](https://cloud.google.com/iam/docs/audit-logging) to help you answer the questions, "Who did what, where, and when?" Your Cloud projects contain only the audit logs for resources that are directly within the project. Other entities, such as folders, organizations, and Cloud Billing accounts, contain the audit logs for the entity itself.


## IAM Conditions

[IAM Conditions](https://cloud.google.com/iam/docs/conditions-overview) allows you to define and enforce conditional, attribute-based access control for Google Cloud resources.

## Tags and access control

[A tag is a key-value pair](https://cloud.google.com/iam/docs/tags-access-control) that is attached to an organization, folder, or project. You can [conditionally grant IAM roles](https://cloud.google.com/iam/docs/conditions-overview) based on whether a resource has a specific tag.

## Conditional access

https://cloud.google.com/iam/docs/managing-conditional-role-bindings

## Searching policies

https://cloud.google.com/asset-inventory/docs/searching-iam-policies

## Linting policies

https://cloud.google.com/iam/docs/linting-policies


## Troubleshooting policy and access problems on Google Cloud

https://cloud.google.com/architecture/troubleshooting-policy-and-access-problems

https://cloud.google.com/architecture/troubleshooting-policy-and-access-problems-use-cases

## Securing the pipeline from your data lake to your data warehouse

https://cloud.google.com/architecture/help-secure-the-pipeline-from-your-data-lake-to-your-data-warehouse
