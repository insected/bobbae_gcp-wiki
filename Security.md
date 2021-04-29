- [Security and Identity](#security-and-identity)
  * [Introduction](#introduction)
    + [Authentication Options](#authentication-options)
  * [IAM](#iam)
    + [Roles](#roles)
    + [Service Accounts](#service-accounts)
  * [Cloud Identity API](#cloud-identity-api)
  * [Identity-Aware Proxy](#identity-aware-proxy)
  * [Context-Aware Access](#context-aware-access)
  * [Identity Platform](#identity-platform)
  * [Managed Services for Microsoft Active Directory](#managed-services-for-microsoft-active-directory)
  * [Resource Manager](#resource-manager)
  * [Security Key enforcement](#security-key-enforcement)
  * [Titan Security Keys](#titan-security-keys)
  * [Access Transparency](#access-transparency)
  * [Binary Authorization](#binary-authorization)
  * [Cloud Asset Inventory](#cloud-asset-inventory)
  * [Cloud Data Loss Prevention](#cloud-data-loss-prevention)
  * [Cloud HSM](#cloud-hsm)
  * [Security Command Center](#security-command-center)
  * [VPC Service Controls](#vpc-service-controls)
  * [Incident Response and Management](#incident-response-and-management)
  * [Phishing Protection](#phishing-protection)
  * [Cloud KMS](#cloud-kms)
  * [reCAPTCHA Enterprise](#recaptcha-enterprise)
  * [Web Risk](#web-risk)
  * [Identity & Security Topics](#identity---security-topics)
  * [Data Governance](#data-governance)
    + [BigQuery Column-level security](#bigquery-column-level-security)
  * [Access Context Manager](#access-context-manager)
  * [Binary Authorization](#binary-authorization)
  * [Qwiklabs](#qwiklabs)
    + [Cloud KMS](#cloud-kms-1)
    + [Security & Identity](#security---identity)
    + [IAM](#iam-1)

<small><i><a href='http://ecotrust-canada.github.io/markdown-toc/'>Table of contents generated with markdown-toc</a></i></small>


## Security and Identity

Computer security, cybersecurity or information technology security (IT security) is the protection of computer systems and networks from information disclosure, theft of or damage to their hardware, software, or electronic data, as well as from the disruption or misdirection of the services they provide.

Identity-based security is a type of security that focuses on access to digital information or services based on the authenticated identity of an individual.

### Introduction

GCP doesn't rely on any single technology to make it secure. GCP builds security through progressive layers that deliver true defense in depth.

https://cloud.google.com/security/infrastructure


Google Infrastructure Security.
[https://www.youtube.com/watch?v=UOdUC8DhprQ](https://www.youtube.com/watch?v=UOdUC8DhprQ)

Google datacenter security has 6 layers. 
[https://www.youtube.com/watch?v=kd33UVZhnAA](https://www.youtube.com/watch?v=kd33UVZhnAA)

Security Foundations.
https://services.google.com/fh/files/misc/google-cloud-security-foundations-guide.pdf

#### Operational security

Google administrates a vulnerability management process that actively scans for security threats using a combination of commercially available and purpose-built in-house tools, intensive automated and manual penetration efforts, quality assurance processes, software security reviews and external audits. 

https://cloud.google.com/security/overview/whitepaper#operational_security

#### Authentication Options

[https://cloud.google.com/blog/products/identity-security/identity-and-authentication-the-google-cloud-way](https://cloud.google.com/blog/products/identity-security/identity-and-authentication-the-google-cloud-way)


### IAM

https://github.com/bobbae/gcp/wiki/IAM


#### Roles

[https://cloud.google.com/iam/docs/understanding-roles](https://cloud.google.com/iam/docs/understanding-roles)


#### Service Accounts

[https://cloud.google.com/iam/docs/service-accounts](https://cloud.google.com/iam/docs/service-accounts)


### Cloud Identity API

Cloud Identity API is an API for provisioning and managing identity resources.

[https://cloud.google.com/identity/docs](https://cloud.google.com/identity/docs)


### Identity-Aware Proxy

Identity-Aware Proxy (IAP) lets you manage access to applications running in the App Engine standard environment, App Engine flexible environment, Compute Engine, and GKE. IAP establishes a central authorization layer for applications accessed by HTTPS, so you can adopt an application-level access control model instead of using network-level firewalls. When you turn on IAP, you must also use [signed headers](https://cloud.google.com/iap/docs/signed-headers-howto) or the App Engine standard environment [Users API](https://cloud.google.com/appengine/docs/standard#users) to secure your app.

[https://cloud.google.com/iap/docs](https://cloud.google.com/iap/docs)

Identity Aware Proxy enables you to configure secure controlled access to your applications so you can enforce "who can see what" access control at the application layer.  You don't need client software, remote access VPNs, firewalls, network configurations. 

[https://www.youtube.com/watch?v=XqMY-rPk3MY](https://www.youtube.com/watch?v=XqMY-rPk3MY)


### Context-Aware Access

Based on the [BeyondCorp](https://cloud.google.com/beyondcorp) security model, Context-Aware Access is an approach that utilizes a variety of Google Cloud offerings to enforce granular access control based on a user's identity and context of the request.

https://www.beyondcorp.com/

[https://cloud.google.com/context-aware-access/docs/overview](https://cloud.google.com/context-aware-access/docs/overview)

Envisioned in 2011, the BeyondCorp security model leverages identity and context to evaluate trust for access decisions rather than using the corporate network as the perimeter. 

[https://www.youtube.com/watch?v=Sq9gp8KBsY0](https://www.youtube.com/watch?v=Sq9gp8KBsY0)

### Zero Trust

Zero Trust is a security concept centered on the belief that organizations should not automatically trust anything inside or outside its perimeters and instead must verify anything and everything trying to connect to its systems before granting access.

The philosophy behind a zero trust network assumes that there are attackers both within and outside of the network, so no users or machines should be automatically trusted.

https://www.cloudflare.com/learning/security/glossary/what-is-zero-trust/

### SASE

Secure access service edge, or SASE, is a cloud-based security model which bundles software-defined networking with network security functions and delivers them from a single service provider. 

SASE brings network security services and access control closer to the end user by shifting those key processes to the cloud, and operates on a global network in order to minimize latency while doing so.

https://www.cloudflare.com/learning/access-management/what-is-sase/

### BeyondCorp Enterprise

A zero trust solution that enables secure access with integrated threat and data protection.

https://cloud.google.com/beyondcorp-enterprise

### Identity Platform

Identity Platform provides back-end services, SDKs, and UI libraries that make it easier to authenticate users to your apps and services.

[https://cloud.google.com/identity-platform/docs](https://cloud.google.com/identity-platform/docs)

Manage the identities of customers, partners, and Things through Identity Platform.

[https://www.youtube.com/watch?v=O_O5Hb1bJyw](https://www.youtube.com/watch?v=O_O5Hb1bJyw)


### Managed Services for Microsoft Active Directory

Managed Service for Microsoft Active Directory is a highly available, hardened Google Cloud service running actual Microsoft AD that enables you to manage your cloud-based AD-dependent workloads, automate AD server maintenance and security configuration, and connect your on-premises AD domain to the cloud.

[https://cloud.google.com/managed-microsoft-ad/docs](https://cloud.google.com/managed-microsoft-ad/docs)


### Resource Manager

Google Cloud provides container resources such as organizations and projects that allow you to group and hierarchically organize other Google Cloud resources. This hierarchical organization helps you manage common aspects of your resources, such as access control and configuration settings. The Resource Manager API enables you to programmatically manage these container resources.

[https://cloud.google.com/ntresource-manager/docs](https://cloud.google.com/resource-manager/docs)

Setting up your Google Cloud Platform resources correctly can save you a lot of trouble down the road. 

[https://www.youtube.com/watch?v=MzclA_hdNLY](https://www.youtube.com/watch?v=MzclA_hdNLY)

Folders are a powerful tool for administering GCP resources in Cloud Resource Manager. Watch this demo video to learn how to get started using folders to help organize and control your cloud resources.

[https://www.youtube.com/watch?v=0oJZhlgDbg8](https://www.youtube.com/watch?v=0oJZhlgDbg8)


### Security Key enforcement

Service to enforce usage of security keys to prevent account takeovers.

[https://vecta.io/symbols/4/google-cloud-platform/44/security-key-enforcement](https://vecta.io/symbols/4/google-cloud-platform/44/security-key-enforcement)

Use 2-Step Verification to protect accounts from unauthorized access. 2-Step Verification puts an extra barrier between your business and cybercriminals who try to steal usernames and passwords to access business data. Turning on 2-Step Verification is the single most important action you can take to protect your business.

[https://support.google.com/cloudidentity/answer/175197/](https://support.google.com/cloudidentity/answer/175197/)

Security in the Cloud vs. on-prem. Sharing responsibility of security in the Cloud.

[https://www.youtube.com/watch?v=wDwQ1YMEyE8](https://www.youtube.com/watch?v=wDwQ1YMEyE8)


### Titan Security Keys

Titan Security Keys are built with a hardware chip that includes firmware engineered by Google to verify the key’s integrity. This helps to ensure that the keys haven’t been physically tampered with.

[https://cloud.google.com/titan-security-key](https://cloud.google.com/titan-security-key)


### Access Transparency

Access Transparency provides you with logs that capture the actions Google personnel take when accessing your content. You might be familiar with [Cloud Audit Logs](https://cloud.google.com/logging/docs/audit), which can help you answer questions about "who did what, where, and when?" in your Google Cloud projects. While Cloud Audit Logs provides these logs about the actions taken by members within your own organization, Access Transparency provides logs of the actions taken by Google personnel.

[https://cloud.google.com/logging/docs/audit/access-transparency-overview](https://cloud.google.com/logging/docs/audit/access-transparency-overview)

[https://www.youtube.com/watch?v=6BCuIBO0Mhg](https://www.youtube.com/watch?v=6BCuIBO0Mhg)


### Binary Authorization

Binary Authorization is a service on Google Cloud that provides software supply-chain security for applications that run in the cloud. Binary Authorization is a service on Google Cloud Platform (GCP) that provides software supply-chain security when deploying container-based applications. Binary Authorization extends Google Kubernetes Engine (GKE) and enforces security policies at deploy time. Binary Authorization works with container images from Container Registry or another container image registry. With Binary Authorization, you can automatically and digitally check each component of your software supply chain, ensuring the quality and integrity of your software before an application is deployed to your production environment.

[https://cloud.google.com/binary-authorization/docs](https://cloud.google.com/binary-authorization/docs)

Check out a demo of Binary Authorization, a Google Cloud Platform security feature. Binary Authorization is a deploy-time security control that ensures only trusted container images are deployed on Kubernetes Engine.

[https://www.youtube.com/watch?v=mi50OJq6wd0](https://www.youtube.com/watch?v=mi50OJq6wd0)


### Cloud Asset Inventory

Cloud Asset Inventory provides inventory services based on a time series database. This database keeps a five-week history of Google Cloud [asset](https://cloud.google.com/asset-inventory/docs/overview#assets) metadata.

[https://cloud.google.com/asset-inventory/docs/overview](https://cloud.google.com/asset-inventory/docs/overview)


### Cloud Data Loss Prevention

Welcome to Cloud Data Loss Prevention (DLP)! Cloud DLP provides access to a powerful sensitive data inspection, classification, and de-identification platform.

[https://cloud.google.com/dlp/docs](https://cloud.google.com/dlp/docs)

Learn how to automatically discover and redact sensitive data everywhere. Try the Data Loss Prevention: Qwik Start lab here:[ http://bit.ly/2QmSZsr](https://www.youtube.com/redirect?event=video_description&v=GArEb2e9jGk&q=http%3A%2F%2Fbit.ly%2F2QmSZsr&redir_token=QUFFLUhqbERxVzNuUE9wY3lHeHJDWGFuZkN4TkExNG9UUXxBQ3Jtc0trbGZ2dW5TYjJYd2FwQmFqZWlIek16QjdScG43R1hXekpkVU9sZTM5dFk1RjNJYkRRaFpEZ3lIdDhuRlVfQVltcVd2MF85aE1YUk9BMzAzOElNSW9qTndXejZURkxiY1hOdXRxTlEwTjJtVlRWTUY4cw%3D%3D)

[https://www.youtube.com/watch?v=GArEb2e9jGk](https://www.youtube.com/watch?v=GArEb2e9jGk)


### Cloud HSM

Cloud HSM is a cloud-hosted Hardware Security Module (HSM) service that allows you to host encryption keys and perform cryptographic operations in a cluster of [FIPS 140-2 Level 3](https://csrc.nist.gov/publications/detail/fips/140/2/final) certified HSMs. Google manages the HSM cluster for you, so you don't need to worry about clustering, scaling, or patching. Because Cloud HSM uses Cloud KMS as its front end, you can leverage all the conveniences and features that Cloud KMS provides.

[https://cloud.google.com/kms/docs/hsm](https://cloud.google.com/kms/docs/hsm)

[https://www.youtube.com/watch?v=DB6UfKFo3ds](https://www.youtube.com/watch?v=DB6UfKFo3ds)


### Security Command Center

Security Command Center is the canonical security and data risk database for Google Cloud. Security Command Center enables you to understand your security and data attack surface by providing asset inventory, discovery, search, and management.

[https://cloud.google.com/security-command-center/docs](https://cloud.google.com/security-command-center/docs)

[https://www.youtube.com/watch?v=k7ZEfAocMq4](https://www.youtube.com/watch?v=k7ZEfAocMq4)


### VPC Service Controls

With VPC Service Controls, administrators can define a security perimeter around resources of Google-managed services to control communication to and between those services.

[https://cloud.google.com/vpc-service-controls/docs](https://cloud.google.com/vpc-service-controls/docs)

VPC Service Controls enables you to establish security perimeters around sensitive data in Google Cloud Platform services such as Google Cloud Storage and BigQuery. 

[https://www.youtube.com/watch?v=EXwJFL24QzY](https://www.youtube.com/watch?v=EXwJFL24QzY)


### Incident Response and Management

The incident response problem space can be divided into three categories: people, process, and data management. Users have long had access to solid people-management solutions (on-call rotation schedulers, etc.) and Google’s SRE book outlines their Incident Management at Google (IMAG) process. In this presentation, attendees will learn the benefits of data management and how Google Cloud Platform (GCP) is providing technology to leverage the idea and accelerate users’ investigations. Attendees will see live demos of Stackdriver Incident Response and Management (IRM) Insights and the supporting GCP technology that makes the innovation possible.

[https://www.youtube.com/watch?v=VXqfbp_zE0c](https://www.youtube.com/watch?v=VXqfbp_zE0c)


### Phishing Protection

Phishing Protection is a phishing countermeasure platform that helps to detect phishing attacks against your users. The Phishing Protection Submission API also enables you to submit URLs suspected to be unsafe to [Safe Browsing](http://safebrowsing.google.com/). Any URLs that are confirmed to match the Safe Browsing Policies will be added to the Safe Browsing list, which is used by over three billion devices to show warnings when a user visits a known unsafe web resource. Common sources of these URLs are customer reports or internal phishing detection results.

[https://cloud.google.com/phishing-protection/docs](https://cloud.google.com/phishing-protection/docs)

A video to show you how security keys prevent phishing attacks by recognizing a domain name and using its hidden private key. 

[https://www.youtube.com/watch?v=c9EOETFnB74](https://www.youtube.com/watch?v=c9EOETFnB74)


### Cloud KMS

A cloud-hosted key management service that lets you manage symmetric and asymmetric cryptographic keys for your cloud services the same way you do on-premises. You can generate, use, rotate, and destroy AES256, RSA 2048, RSA 3072, RSA 4096, EC P256, and EC P384 cryptographic keys. Toggle between software- and hardware-protected encryption keys with the press of a button. Host encryption keys and perform cryptographic operations in FIPS 140-2 Level 3 certified HSMs. With this fully managed service, you can protect your most sensitive workloads without the need to worry about the operational overhead of managing an HSM cluster. Encrypt data in [BigQuery](https://cloud.google.com/bigquery) and [Compute Engine](https://cloud.google.com/compute) with encryption keys that are stored and managed in a third-party key management system that’s deployed outside Google’s infrastructure. External Key Manager allows you to maintain separation between your data at rest and your encryption keys while still leveraging the power of cloud for compute and analytics. Key Access Justifications works with [Cloud EKM](https://cloud.google.com/blog/products/identity-security/cloud-external-key-manager-now-in-beta) to greatly advance the control you have over your data. It’s the only product that gives you visibility into every request for an encryption key, a justification for that request, and a mechanism to approve or deny decryption in the context of that request. 

[https://cloud.google.com/security-key-management](https://cloud.google.com/security-key-management)

Learn about how Google automatically encrypts your data and how to take control of encryption by managing your own keys. 

[https://www.youtube.com/watch?v=38_dWxOHUN8](https://www.youtube.com/watch?v=38_dWxOHUN8)


### reCAPTCHA Enterprise

Google has been defending millions of sites with reCAPTCHA for almost a decade. reCAPTCHA Enterprise is an extension of that effort to help enterprises detect other types of fraudulent activity on their sites, like scraping, credential stuffing, and automated account creation. reCAPTCHA Enterprise offers enhanced detection with more granular scores, reason codes for risky events, and the ability to tune your site-specific model. reCAPTCHA Enterprise is a service that protects your site from spam and abuse. reCAPTCHA Enterprise builds on the existing reCAPTCHA API which uses advanced risk analysis techniques to tell humans and bots apart. reCAPTCHA Enterprise adds enhancements specifically designed to protect enterprise businesses, such as more granular scoring and returning reason codes with low scores to aid in analysis.

[https://cloud.google.com/recaptcha-enterprise/docs](https://cloud.google.com/recaptcha-enterprise/docs)

See how reCAPTCHA Enterprise can help protect your websites from fraud and abuse.

[https://www.youtube.com/watch?v=ic3Fj2B1LR4](https://www.youtube.com/watch?v=ic3Fj2B1LR4)


### Web Risk

Web Risk is a new enterprise security product that lets your client applications check URLs against Google's constantly updated lists of unsafe web resources.

[https://cloud.google.com/web-risk/docs](https://cloud.google.com/web-risk/docs)


### Identity & Security Topics

[https://cloud.google.com/blog/products/identity-security](https://cloud.google.com/blog/products/identity-security)


### Authentication, Identity, Security, AuthN, AuthZ

Access control for Google Cloud APIs encompasses authentication, authorization, and auditing. Authentication determines who you are, authorization determines what you can do, and auditing logs what you did.  For authorization, see [Identity and Access Management](https://cloud.google.com/iam/docs) (IAM). For auditing, see [Cloud Audit Logs](https://cloud.google.com/logging/docs/audit).

https://cloud.google.com/docs/authentication

### PKI

A public key infrastructure (PKI) is a set of roles, policies, hardware, software and procedures needed to create, manage, distribute, use, store and revoke [digital certificates](https://en.wikipedia.org/wiki/Public_key_certificate) and manage [public-key encryption](https://en.wikipedia.org/wiki/Public-key_cryptography). The purpose of a PKI is to facilitate the secure electronic transfer of information for a range of network activities such as e-commerce, internet banking and confidential email. It is required for activities where simple passwords are an inadequate authentication method and more rigorous proof is required to confirm the identity of the parties involved in the communication and to validate the information being transferred.

[https://www.ssh.com/pki/](https://www.ssh.com/pki/)


### OAthu, OpenID Connect, SAML

[https://www.okta.com/identity-101/whats-the-difference-between-oauth-openid-connect-and-saml/](https://www.okta.com/identity-101/whats-the-difference-between-oauth-openid-connect-and-saml/)

### Data Governance 


#### BigQuery Column-level security

[https://cloud.google.com/blog/products/data-analytics/data-governance-new-ways-to-securely-access-and-discover-data](https://cloud.google.com/blog/products/data-analytics/data-governance-new-ways-to-securely-access-and-discover-data)

### Access Context Manager
Access Context Manager allows Google Cloud organization administrators to define fine-grained, attribute based access control for projects and resources in Google Cloud.

Administrators first define an access policy, which is an organization-wide container for access levels and service perimeters.

Access levels describe the necessary requirements for requests to be honored. 

https://cloud.google.com/access-context-manager/docs/overview

### Binary Authorization

Binary Authorization is a deploy-time security control that ensures only trusted container images are deployed on Google Kubernetes Engine (GKE). With Binary Authorization, you can require images to be signed by trusted authorities during the development process and then enforce signature validation when deploying. By enforcing validation, you can gain tighter control over your container environment by ensuring only verified images are integrated into the build-and-release process.

https://cloud.google.com/binary-authorization/


### Qwiklabs


#### Cloud KMS

In this lab you'll learn how to use some advanced features of Google Cloud Security and Privacy APIs, including:



*   Setting up a secure Cloud Storage bucket
*   Managing keys and encrypted data using Key Management Storage
*   Viewing Cloud Storage audit logs

You'll take abridged data from the Enron Corpus, encrypt it and load it into Cloud Storage.

[Getting Started with Cloud KMS](https://www.qwiklabs.com/focuses/1713?catalog_rank=%7B%22rank%22%3A20%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&parent=catalog&search_id=7468061)


#### Security & Identity

Security is an uncompromising feature of Google Cloud services, and Google Cloud has developed specific tools for ensuring safety and identity across your projects. In this fundamental-level quest, you will get hands-on practice with Google Cloud’s Identity and Access Management (IAM) service, which is the go-to for managing user and virtual machine accounts.

[Security & Identity Fundamentals](https://www.qwiklabs.com/quests/40?catalog_rank=%7B%22rank%22%3A1%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&search_id=7482841)


#### IAM

In this fundamental-level quest, you will get hands-on practice with Google Cloud’s Identity and Access Management (IAM) service, which is the go-to for managing user and virtual machine accounts. You will get experience with network security by provisioning VPCs and VPNs, and learn what tools are available for security threat and data loss protections.

[Ensure Access & Identity in Google Cloud](https://www.qwiklabs.com/quests/150?catalog_rank=%7B%22rank%22%3A3%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&search_id=7482841)

