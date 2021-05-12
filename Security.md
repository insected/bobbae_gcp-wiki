
The Internet has transformed our lives in many good ways. Unfortunately, this vast network and its associated technologies also have brought in their wake, [the increasing number of security threats](https://en.wikipedia.org/wiki/Computer_security
). When it comes to [privacy](Privacy) and security, [it’s a good idea to have both](https://us.norton.com/internetsecurity-privacy-privacy-vs-security-whats-the-difference.html).

GCP doesn't rely on any single technology to make its [infrastructure secure](https://cloud.google.com/security/infrastructure). GCP builds security through [progressive layers](https://www.youtube.com/watch?v=MHtg2Au78LI&list=PLIivdWyY5sqLO-4ePY-A2yROgONOA6Cz4) that deliver [true defense in depth](https://www.youtube.com/watch?v=vBdYVFgZ2ug). [Google datacenter security](https://www.youtube.com/watch?v=UOdUC8DhprQ) has [6 layers](https://www.youtube.com/watch?v=kd33UVZhnAA). 

## Security Foundations Blueprint

The [Security Foundations Blueprint](https://services.google.com/fh/files/misc/google-cloud-security-foundations-guide.pdf) presents [an opinionated view](https://cloud.google.com/blog/products/identity-security/google-cloud-security-foundations-guide) of Google Cloud security best practices, organized to allow
users to adopt or adapt them and then automatically deploy them for their estates on Google Cloud.


There is an [example repo showing how the CFT Terraform modules can be composed to build a secure GCP foundation](https://github.com/terraform-google-modules/terraform-example-foundation).

## Security Infrastructure Design

Read the [overview of how security is designed](https://cloud.google.com/security/infrastructure/design/) into Google's technical infrastructure. 

## Cryptography

[Cryptography](Cryptography)  is the study of secure communications techniques that allow only the sender and intended recipient of a message to view its contents.

## IAM

[Identity and Access Management](IAM)  lets administrators authorize who can take action on specific resources, giving you full control and visibility. 

## Security and Identity

Computer security, cybersecurity or information technology security (IT security) is the protection of computer systems and networks from information disclosure, theft of or damage to their hardware, software, or electronic data, as well as from the disruption or misdirection of the services they provide.

[Identity-based security](https://en.wikipedia.org/wiki/Identity-based_security) is a type of security that focuses on access to digital information or services based on the authenticated identity of an individual.  

Account management, authentication and password management can be tricky. Often, account management is a dark corner that isn't a top priority for developers or product managers. The resulting experience often falls short of what some of your users would expect for data security and user experience.  Use  [the best practices](https://cloud.google.com/blog/products/identity-security/account-authentication-and-password-management-best-practices) to  ensure you have a safe, scalable, usable account authentication system.

## Operational security

Google [administrates a vulnerability management process that actively scans](https://cloud.google.com/security/overview/whitepaper#operational_security) for security threats using a combination of commercially available and purpose-built in-house tools, intensive automated and manual penetration efforts, quality assurance processes, software security reviews and external audits. 



## Authentication Options

[[https://storage.googleapis.com/gweb-cloudblog-publish/images/1_YvHxYeQ.max-600x600.png]]

[https://cloud.google.com/blog/products/identity-security/identity-and-authentication-the-google-cloud-way](https://cloud.google.com/blog/products/identity-security/identity-and-authentication-the-google-cloud-way)





## Roles

A role contains a set of permissions that allows you to perform specific actions on Google Cloud resources. To make permissions available to members, including users, groups, and service accounts, you grant roles to the members.

[https://cloud.google.com/iam/docs/understanding-roles](https://cloud.google.com/iam/docs/understanding-roles)


## Service Accounts


[A Service Account](Service-Accounts)  is a special kind of account used by an application or a virtual machine (VM) instance, not a person. Applications use service accounts to make authorized API calls, authorized as either the service account itself, or as Google Workspace or Cloud Identity users through domain-wide delegation.

## Cloud Identity API

[Cloud Identity](https://cloud.google.com/identity/docs) API is an API for provisioning and managing identity resources.

Cloud Identity is an Identity as a Service (IDaaS) solution that centrally manages users and groups. You can configure Cloud Identity to federate identities between Google and other identity providers, such as [Active Directory](https://cloud.google.com/architecture/identity/federating-gcp-with-active-directory-introduction) and [Azure Active Directory](https://cloud.google.com/architecture/identity/federating-gcp-with-azure-active-directory).

### Identity-Aware Proxy

[Identity-Aware Proxy](https://cloud.google.com/iap/docs) (IAP) lets you manage access to applications running in the App Engine standard environment, App Engine flexible environment, Compute Engine, and GKE. IAP establishes a central authorization layer for applications accessed by HTTPS, so you can adopt an application-level access control model instead of using network-level firewalls. When you turn on IAP, you must also use [signed headers](https://cloud.google.com/iap/docs/signed-headers-howto) or the App Engine standard environment [Users API](https://cloud.google.com/appengine/docs/standard#users) to secure your app.


Identity Aware Proxy enables you to configure secure controlled access to your applications so you can enforce "who can see what" access control at the application layer.  You don't need client software, remote access VPNs, firewalls, network configurations. 

[https://www.youtube.com/watch?v=XqMY-rPk3MY](https://www.youtube.com/watch?v=XqMY-rPk3MY)


## Context-Aware Access

Based on the [BeyondCorp](https://cloud.google.com/beyondcorp) security model, Context-Aware Access is an approach that utilizes a variety of Google Cloud offerings to enforce granular access control based on a user's identity and context of the request.



[https://cloud.google.com/context-aware-access/docs/overview](https://cloud.google.com/context-aware-access/docs/overview)

Envisioned in 2011, the [BeyondCorp](https://www.beyondcorp.com/) security model leverages identity and context to evaluate trust for access decisions rather than using the corporate network as the perimeter. 

[https://www.youtube.com/watch?v=Sq9gp8KBsY0](https://www.youtube.com/watch?v=Sq9gp8KBsY0)

In the same way that BeyondCorp helped us to evolve beyond a perimeter based security model, [BeyondProd](https://cloud.google.com/security/beyondprod) represents a similar leap forward in our approach to production security. The BeyondProd approach describes a cloud-native security architecture that assumes no trust between services, provides isolation between workloads, verifies that only centrally built applications are deployed, automates vulnerability management, and enforces strong access controls to critical data. The BeyondProd architecture led Google to innovate several new systems in order to meet these requirements.

### Zero Trust

[Zero Trust](https://www.cloudflare.com/learning/security/glossary/what-is-zero-trust/) is a security concept centered on the belief that organizations should not automatically trust anything inside or outside its perimeters and instead must verify anything and everything trying to connect to its systems before granting access.

The philosophy behind a zero trust network assumes that there are attackers both within and outside of the network, so no users or machines should be automatically trusted.


## SASE

[Secure access service edge](https://www.cloudflare.com/learning/access-management/what-is-sase/), or SASE, is a cloud-based security model which bundles software-defined networking with network security functions and delivers them from a single service provider. 

SASE brings network security services and access control closer to the end user by shifting those key processes to the cloud, and operates on a global network in order to minimize latency while doing so.




## Identity Platform

[Google Identity Platform](https://cloud.google.com/identity-platform/docs) provides back-end services, SDKs, and UI libraries that make it easier to authenticate users to your apps and services.


Manage the identities of customers, partners, and Things through Identity Platform.

[https://www.youtube.com/watch?v=O_O5Hb1bJyw](https://www.youtube.com/watch?v=O_O5Hb1bJyw)


## Managed Services for Microsoft Active Directory

[Managed Service for Microsoft Active Directory](https://cloud.google.com/managed-microsoft-ad/docs) is a highly available, hardened Google Cloud service running actual Microsoft AD that enables you to manage your cloud-based AD-dependent workloads, automate AD server maintenance and security configuration, and connect your on-premises AD domain to the cloud.



## Resource Manager

Google Cloud provides container resources such as organizations and projects that allow you to group and hierarchically organize other Google Cloud resources. This hierarchical organization helps you manage common aspects of your resources, such as access control and configuration settings. The [Resource Manager](https://cloud.google.com/ntresource-manager/docs) API enables you to programmatically manage these container resources.


Setting up your Google Cloud Platform resources correctly can save you a lot of trouble down the road. 

[https://www.youtube.com/watch?v=MzclA_hdNLY](https://www.youtube.com/watch?v=MzclA_hdNLY)

Folders are a powerful tool for administering GCP resources in Cloud Resource Manager. Watch this demo video to learn how to get started using folders to help organize and control your cloud resources.

[https://www.youtube.com/watch?v=0oJZhlgDbg8](https://www.youtube.com/watch?v=0oJZhlgDbg8)


## Security Key enforcement

Service to enforce usage of security keys to prevent account takeovers.

[https://vecta.io/symbols/4/google-cloud-platform/44/security-key-enforcement](https://vecta.io/symbols/4/google-cloud-platform/44/security-key-enforcement)

Use 2-Step Verification to protect accounts from unauthorized access. 2-Step Verification puts an extra barrier between your business and cybercriminals who try to steal usernames and passwords to access business data. Turning on 2-Step Verification is the single most important action you can take to protect your business.

[https://support.google.com/cloudidentity/answer/175197/](https://support.google.com/cloudidentity/answer/175197/)

Security in the Cloud vs. on-prem. Sharing responsibility of security in the Cloud.

[https://www.youtube.com/watch?v=wDwQ1YMEyE8](https://www.youtube.com/watch?v=wDwQ1YMEyE8)


### Titan Security Keys

[Titan Security Keys](https://cloud.google.com/titan-security-key) are built with a hardware chip that includes firmware engineered by Google to verify the key’s integrity. This helps to ensure that the keys haven’t been physically tampered with.



## Access Transparency

[Access Transparency](https://cloud.google.com/logging/docs/audit/access-transparency-overview) provides you with logs that capture the actions Google personnel take when accessing your content. You might be familiar with [Cloud Audit Logs](https://cloud.google.com/logging/docs/audit), which can help you answer questions about "who did what, where, and when?" in your Google Cloud projects. While Cloud Audit Logs provides these logs about the actions taken by members within your own organization, Access Transparency provides logs of the actions taken by Google personnel.



[https://www.youtube.com/watch?v=6BCuIBO0Mhg](https://www.youtube.com/watch?v=6BCuIBO0Mhg)


## Binary Authorization

[Binary Authorization](https://cloud.google.com/binary-authorization/docs) is a service on Google Cloud that provides software supply-chain security for applications that run in the cloud. Binary Authorization is a service on Google Cloud Platform (GCP) that provides software supply-chain security when deploying container-based applications. Binary Authorization extends Google Kubernetes Engine (GKE) and enforces security policies at deploy time. Binary Authorization works with container images from Container Registry or another container image registry. With Binary Authorization, you can automatically and digitally check each component of your software supply chain, ensuring the quality and integrity of your software before an application is deployed to your production environment.



Check out a demo of Binary Authorization, a Google Cloud Platform security feature. Binary Authorization is a deploy-time security control that ensures only trusted container images are deployed on Kubernetes Engine.

[https://www.youtube.com/watch?v=mi50OJq6wd0](https://www.youtube.com/watch?v=mi50OJq6wd0)


## Cloud Asset Inventory

[Cloud Asset Inventory](https://cloud.google.com/asset-inventory/docs/overview) provides inventory services based on a time series database. This database keeps a five-week history of Google Cloud [asset](https://cloud.google.com/asset-inventory/docs/overview#assets) metadata.



## Cloud Data Loss Prevention

[Cloud Data Loss Prevention (DLP)](https://cloud.google.com/dlp/docs) provides access to a powerful sensitive data inspection, classification, and de-identification platform.


Learn how to automatically discover and redact sensitive data everywhere. 

Try the [Data Loss Prevention Qwik Start lab](http://bit.ly/2QmSZsr).

[https://www.youtube.com/watch?v=GArEb2e9jGk](https://www.youtube.com/watch?v=GArEb2e9jGk)


## Cloud HSM

[Cloud HSM](https://cloud.google.com/kms/docs/hsm) is a cloud-hosted Hardware Security Module (HSM) service that allows you to host encryption keys and perform cryptographic operations in a cluster of [FIPS 140-2 Level 3](https://csrc.nist.gov/publications/detail/fips/140/2/final) certified HSMs. Google manages the HSM cluster for you, so you don't need to worry about clustering, scaling, or patching. Because Cloud HSM uses Cloud KMS as its front end, you can leverage all the conveniences and features that Cloud KMS provides.


[https://www.youtube.com/watch?v=DB6UfKFo3ds](https://www.youtube.com/watch?v=DB6UfKFo3ds)


## Security Command Center

[Security Command Center](https://cloud.google.com/security-command-center/docs) is the canonical security and data risk database for Google Cloud. Security Command Center enables you to understand your security and data attack surface by providing asset inventory, discovery, search, and management.



[https://www.youtube.com/watch?v=k7ZEfAocMq4](https://www.youtube.com/watch?v=k7ZEfAocMq4)


## VPC Service Controls

With [VPC Service Controls](https://cloud.google.com/vpc-service-controls/docs), administrators can define a security perimeter around resources of Google-managed services to control communication to and between those services.


VPC Service Controls enables you to establish security perimeters around sensitive data in Google Cloud Platform services such as [Google Cloud Storage](https://cloud.google.com/storage) and [BigQuery](BigQuery). 

[https://www.youtube.com/watch?v=EXwJFL24QzY](https://www.youtube.com/watch?v=EXwJFL24QzY)


## Incident Response and Management

The [incident](https://cloud.google.com/monitoring/alerts/incidents-events) response problem space can be divided into three categories: people, process, and data management. 

Users have long had access to solid people-management solutions (on-call rotation schedulers, etc.) and Google’s [SRE book](https://sre.google/sre-book/table-of-contents/) outlines their [Incident Management](https://cloud.google.com/blog/products/management-tools/meeting-reliability-challenges-with-sre-principles) at Google (IMAG) process. 

The  [Stackdriver](https://cloud.google.com/monitoring) supports Incident Response and Management (IRM)  Insights and the supporting GCP technology that makes the innovation possible.

[https://www.youtube.com/watch?v=VXqfbp_zE0c](https://www.youtube.com/watch?v=VXqfbp_zE0c)


## Phishing Protection

[Phishing Protection](https://cloud.google.com/phishing-protection/docs) is a phishing countermeasure platform that helps to detect phishing attacks against your users. 

The Phishing Protection Submission API also enables you to submit URLs suspected to be unsafe to [Safe Browsing](http://safebrowsing.google.com/). 

Any URLs that are confirmed to match the Safe Browsing Policies will be added to the Safe Browsing list, which is used by over three billion devices to show warnings when a user visits a known unsafe web resource. Common sources of these URLs are customer reports or internal phishing detection results.


A video to show you how security keys prevent phishing attacks by recognizing a domain name and using its hidden private key. 

[https://www.youtube.com/watch?v=c9EOETFnB74](https://www.youtube.com/watch?v=c9EOETFnB74)


## Cloud KMS

A cloud-hosted [key management](https://cloud.google.com/security-key-management) service that lets you manage symmetric and asymmetric cryptographic keys for your cloud services the same way you do on-premises. You can generate, use, rotate, and destroy AES256, RSA 2048, RSA 3072, RSA 4096, EC P256, and EC P384 cryptographic keys. Toggle between software- and hardware-protected encryption keys with the press of a button. Host encryption keys and perform cryptographic operations in FIPS 140-2 Level 3 certified HSMs. With this fully managed service, you can protect your most sensitive workloads without the need to worry about the operational overhead of managing an HSM cluster. 

Encrypt data in [BigQuery](https://cloud.google.com/bigquery) and [Compute Engine](https://cloud.google.com/compute) with encryption keys that are stored and managed in a third-party key management system that’s deployed outside Google’s infrastructure. External Key Manager allows you to maintain separation between your data at rest and your encryption keys while still leveraging the power of cloud for compute and analytics. 

Key Access Justifications works with [Cloud EKM](https://cloud.google.com/blog/products/identity-security/cloud-external-key-manager-now-in-beta) to greatly advance the control you have over your data. It’s the only product that gives you visibility into every request for an encryption key, a justification for that request, and a mechanism to approve or deny decryption in the context of that request. 


Learn about how Google automatically encrypts your data and how to take control of encryption by managing your own keys. 

[https://www.youtube.com/watch?v=38_dWxOHUN8](https://www.youtube.com/watch?v=38_dWxOHUN8)


## reCAPTCHA Enterprise

Google has been defending millions of sites with [reCAPTCHA](https://cloud.google.com/recaptcha-enterprise/docs) for almost a decade. 
reCAPTCHA Enterprise is an extension of that effort to help enterprises detect other types of fraudulent activity on their sites, like scraping, credential stuffing, and automated account creation. reCAPTCHA Enterprise offers enhanced detection with more granular scores, reason codes for risky events, and the ability to tune your site-specific model.  reCAPTCHA Enterprise is a service that protects your site from spam and abuse. reCAPTCHA Enterprise builds on the existing reCAPTCHA API which uses advanced risk analysis techniques to tell humans and bots apart.  reCAPTCHA Enterprise adds enhancements specifically designed to protect enterprise businesses, such as more granular scoring and returning reason codes with low scores to aid in analysis.

[See](https://www.youtube.com/watch?v=ic3Fj2B1LR4) how reCAPTCHA Enterprise can help protect your websites from fraud and abuse.


## Web Risk

[Web Risk](https://cloud.google.com/web-risk/docs) is a new enterprise security product that lets your client applications check URLs against Google's constantly updated lists of unsafe web resources.



## Identity & Security Topics

See how Google Cloud [Identity](https://cloud.google.com/identity)  achieves [confidentiality, data integrity, availability, non-repudiation and authentication of your data.](https://cloud.google.com/blog/products/identity-security)


## Authentication, Identity, Security, AuthN, AuthZ

Access control for Google Cloud APIs encompasses [authentication](https://cloud.google.com/docs/authentication), authorization, and auditing. Authentication determines who you are, authorization determines what you can do, and auditing logs what you did.  For authorization, see [Identity and Access Management](https://cloud.google.com/iam/docs) (IAM). For auditing, see [Cloud Audit Logs](https://cloud.google.com/logging/docs/audit).


## PKI

A [public key infrastructure](https://www.ssh.com/pki/) (PKI) is a set of roles, policies, hardware, software and procedures needed to create, manage, distribute, use, store and revoke [digital certificates](https://en.wikipedia.org/wiki/Public_key_certificate) and manage [public-key encryption](https://en.wikipedia.org/wiki/Public-key_cryptography). The purpose of a PKI is to facilitate the secure electronic transfer of information for a range of network activities such as e-commerce, internet banking and confidential email. It is required for activities where simple passwords are an inadequate authentication method and more rigorous proof is required to confirm the identity of the parties involved in the communication and to validate the information being transferred.


## OAuth, OpenID Connect, SAML

[OAuth](https://en.wikipedia.org/wiki/OAuth) is an open standard for access delegation, commonly used as a way for Internet users to grant websites or applications access to their information on other websites but without giving them the passwords. f you’ve ever signed up to a new application and agreed to let it automatically source new contacts via Facebook or your phone contacts, then you’ve likely used OAuth 2.0. This standard provides secure delegated access. 

[Security Assertion Markup Language](https://en.wikipedia.org/wiki/Security_Assertion_Markup_Language) (SAML) is an open standard for exchanging authentication and authorization data between parties, in particular, between an identity provider and a service provider. You’ve more likely experienced SAML authentication in action in the work environment. For example, it enables you to log into your corporate intranet or IdP and then access numerous additional services, such as Salesforce, Box, or Workday, without having to re-enter your credentials.

[OpenID](https://en.wikipedia.org/wiki/OpenID) Connect allows clients of all types, including Web-based, mobile, and JavaScript clients, to request and receive information about authenticated sessions and end-users. The specification suite is extensible, allowing participants to use optional features such as encryption of identity data, discovery of OpenID Providers, and session management, when it makes sense for them.  If you’ve used your Google to sign in to applications like YouTube, or Facebook to log into an online shopping cart, then you’re familiar with this authentication option. OpenID Connect is an open standard that organizations use to authenticate users.

[https://www.okta.com/identity-101/whats-the-difference-between-oauth-openid-connect-and-saml/](https://www.okta.com/identity-101/whats-the-difference-between-oauth-openid-connect-and-saml/)



## Machine Learning for Cybersecurity

There have been attempts to aid Cybersecurity concerns using [Machine Learning](Machine-Learning).
[ML in network security](https://towardsdatascience.com/machine-learning-for-cybersecurity-101-7822b802790b) implies new solutions called Network Traffic Analytics (NTA) aimed at in-depth analysis of all the traffic at each layer and detect attacks and anomalies.

## Data Governance 

[Data governance](https://cloud.google.com/learn/what-is-data-governance) is a principled approach to managing data during its life cycle, from acquisition to use to disposal. 

### BigQuery Column-level security

[https://cloud.google.com/blog/products/data-analytics/data-governance-new-ways-to-securely-access-and-discover-data](https://cloud.google.com/blog/products/data-analytics/data-governance-new-ways-to-securely-access-and-discover-data)

### Access Context Manager

[Access Context Manager](https://cloud.google.com/access-context-manager/docs/overview) allows Google Cloud organization administrators to define fine-grained, attribute based access control for projects and resources in Google Cloud.

Administrators first define an access policy, which is an organization-wide container for access levels and service perimeters.

Access levels describe the necessary requirements for requests to be honored. 



### Binary Authorization

[Binary Authorization](https://cloud.google.com/binary-authorization/) is a deploy-time security control that ensures only trusted container images are deployed on Google Kubernetes Engine (GKE). With Binary Authorization, you can require images to be signed by trusted authorities during the development process and then enforce signature validation when deploying. By enforcing validation, you can gain tighter control over your container environment by ensuring only verified images are integrated into the build-and-release process.





### Binary Authorization Attestations with Voucher

An [attestor](https://cloud.google.com/binary-authorization/docs/creating-attestations-voucher) is a Google Cloud resource that Binary Authorization uses to verify the attestation at container image deploy time. Attestors contain the public key that corresponds to the private key used by a signer to sign the container image digest and create the attestation. 

The Binary Authorization enforcer uses the attestor at deploy time to limit which container images are allowed to be deployed to those with an accompanying, verifiable attestation created prior to deployment.

## StackRox

[StackRox](https://www.stackrox.com/post/2020/11/stackrox-integrates-with-google-artifact-registry/) provides full life cycle security across build, deploy, and runtime phases for your Google Kubernetes Engine (GKE), Google Compute Engine (GCE), or Anthos environments. Alternatively, use StackRox to enforce security policies for GKE with Cloud Run. 

## Qwiklabs

### Cloud KMS

[Getting Started with Cloud KMS](https://www.qwiklabs.com/focuses/1713?catalog_rank=%7B%22rank%22%3A20%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&parent=catalog&search_id=7468061)


[Security & Identity Fundamentals](https://www.qwiklabs.com/quests/40?catalog_rank=%7B%22rank%22%3A1%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&search_id=7482841)

[Ensure Access & Identity in Google Cloud](https://www.qwiklabs.com/quests/150?catalog_rank=%7B%22rank%22%3A3%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&search_id=7482841)

