[Information Security](https://wikipedia.org/wiki/Information_security   ), sometimes shortened to InfoSec, is the practice of protecting information by mitigating information risks.


The Internet has transformed our lives in many good ways. Unfortunately, this vast network and its associated technologies also have brought in their wake, [the increasing number of security threats](https://wikipedia.org/wiki/Internet_security
). 

GCP doesn't rely on any single technology to make its [infrastructure secure](https://cloud.google.com/security/infrastructure). GCP [delivers](   https://cloud.google.com/blog/products/identity-security/delivering-the-industrys-most-trusted-cloud ) security through [progressive layers](https://www.youtube.com/watch?v=MHtg2Au78LI&list=PLIivdWyY5sqLO-4ePY-A2yROgONOA6Cz4) that deliver [true defense in depth](https://www.youtube.com/watch?v=vBdYVFgZ2ug). [Google datacenter security](https://www.youtube.com/watch?v=UOdUC8DhprQ) has [6 layers](https://www.youtube.com/watch?v=kd33UVZhnAA). 


## GCP Infrastructure Security

https://cloud.google.com/security/infrastructure/design

## Privacy

We need a holistic approach to security and [privacy](Privacy) and must protect information through its entire lifecycle, from the moment it's captured to the day it's destroyed.

## Security issues in cloud computing

https://jisajournal.springeropen.com/articles/10.1186/1869-0238-4-5

## Security Foundations Blueprint

The [Security Foundations Blueprint](https://services.google.com/fh/files/misc/google-cloud-security-foundations-guide.pdf) presents [an opinionated view](https://cloud.google.com/blog/products/identity-security/google-cloud-security-foundations-guide) of Google Cloud security best practices, organized to allow
users to adopt or adapt them and then automatically deploy them for their estates on Google Cloud.


There is an [example repo showing how the CFT Terraform modules can be composed to build a secure GCP foundation](https://github.com/terraform-google-modules/terraform-example-foundation).

https://cloud.google.com/blog/products/devops-sre/using-the-cloud-foundation-toolkit-with-terraform

## Risk Manager

Google Cloud security diagnostic tool called Risk Manager enables customers to measure and manage their risk on Google Cloud and obtain a report on their security posture. 

https://cloud.google.com/risk-protection-program

## Security Infrastructure Design

Read the [overview of how security is designed](https://cloud.google.com/security/infrastructure/design/) into Google's technical infrastructure. 

https://cloud.google.com/blog/topics/developers-practitioners/foundational-best-practices-securing-your-cloud-deployment

## Cryptography

[Cryptography](Cryptography)  is the study of secure communications techniques that allow only the sender and intended recipient of a message to view its contents.

### Encryption at Rest



Google Cloud encrypts all customer content stored [at rest](Encryption-at-Rest), without any action required from the customer, using one or more encryption mechanisms.



## IAM

[Identity and Access Management](IAM)  lets administrators authorize who can take action on specific resources, giving you full control and visibility. 



## Security and Identity

Computer security, cybersecurity or information technology security (IT security) is the protection of computer systems and networks from information disclosure, theft of or damage to their hardware, software, or electronic data, as well as from the disruption or misdirection of the services they provide.

[Identity-based security](https://en.wikipedia.org/wiki/Identity-based_security) is a type of security that focuses on access to digital information or services based on the authenticated identity of an individual.  

https://cloud.google.com/identity/docs/overview

[Account management](Accounts-and-Billing), [authentication](Authentication) and password management can be tricky. Often, account management is a dark corner that isn't a top priority for developers or product managers. The resulting experience often falls short of what some of your users would expect for data security and user experience.  Use  [the best practices](https://cloud.google.com/blog/products/identity-security/account-authentication-and-password-management-best-practices) to  ensure you have a safe, scalable, usable account authentication system.

### Some articles on Identity and Security

https://cloud.google.com/blog/products/identity-security

## Operational security

Google [administrates a vulnerability management process that actively scans](https://cloud.google.com/security/overview/whitepaper#operational_security) for security threats using a combination of commercially available and purpose-built in-house tools, intensive automated and manual penetration efforts, quality assurance processes, software security reviews and external audits. 



## Roles

A role contains a set of permissions that allows you to perform specific actions on Google Cloud resources. To make permissions available to members, including users, groups, and service accounts, you grant roles to the members.

[https://cloud.google.com/iam/docs/understanding-roles](https://cloud.google.com/iam/docs/understanding-roles)


## Service Accounts


[A Service Account](Service-Accounts)  is a special kind of account used by an application or a virtual machine (VM) instance, not a person. Applications use service accounts to make authorized API calls, authorized as either the service account itself, or as Google Workspace or Cloud Identity users through domain-wide delegation.

## Cloud Identity API

[Cloud Identity](https://cloud.google.com/identity/docs) API is an API for provisioning and managing identity resources.
It helps you achieve [confidentiality, data integrity, availability, non-repudiation and authentication of your data.](https://cloud.google.com/blog/products/identity-security)

Cloud Identity is an Identity as a Service (IDaaS) solution that centrally manages users and groups. You can configure Cloud Identity to federate identities between Google and other identity providers, such as [Active Directory](https://cloud.google.com/architecture/identity/federating-gcp-with-active-directory-introduction) and [Azure Active Directory](https://cloud.google.com/architecture/identity/federating-gcp-with-azure-active-directory).



### Identity-Aware Proxy

[Identity-Aware Proxy](https://cloud.google.com/iap/docs) (IAP) lets you manage access to applications running in the App Engine standard environment, App Engine flexible environment, Compute Engine, and GKE. IAP establishes a central authorization layer for applications accessed by HTTPS, so you can adopt an application-level access control model instead of using network-level firewalls. When you turn on IAP, you must also use [signed headers](https://cloud.google.com/iap/docs/signed-headers-howto) or the App Engine standard environment [Users API](https://cloud.google.com/appengine/docs/standard#users) to secure your app.


Identity Aware Proxy enables you to configure secure controlled access to your applications so you can enforce "who can see what" access control at the application layer.  You don't need client software, remote access VPNs, firewalls, network configurations. 

[https://www.youtube.com/watch?v=XqMY-rPk3MY](https://www.youtube.com/watch?v=XqMY-rPk3MY)


### Device Identity

The Cloud Identity Groups API allows you to create and manage different types of devices within your organization.


https://cloud.google.com/identity/docs/concepts/overview-devices

### Groups Identity

A group is a collection of entities, where each entity can be either another group or a user. 

https://cloud.google.com/identity/docs/groups



## Context-Aware Access

Based on the [BeyondCorp](https://cloud.google.com/beyondcorp) security model, Context-Aware Access is an approach that utilizes a variety of Google Cloud offerings to enforce granular access control based on a user's identity and context of the request.



[https://cloud.google.com/context-aware-access/docs/overview](https://cloud.google.com/context-aware-access/docs/overview)

Envisioned in 2011, the [BeyondCorp](https://www.beyondcorp.com/) security model leverages identity and context to evaluate trust for access decisions rather than using the corporate network as the perimeter. 

[https://www.youtube.com/watch?v=Sq9gp8KBsY0](https://www.youtube.com/watch?v=Sq9gp8KBsY0)

In the same way that BeyondCorp helped us to evolve beyond a perimeter based security model, [BeyondProd](https://cloud.google.com/security/beyondprod) represents a similar leap forward in our approach to production security. The BeyondProd approach describes a cloud-native security architecture that assumes no trust between services, provides isolation between workloads, verifies that only centrally built applications are deployed, automates vulnerability management, and enforces strong access controls to critical data. The BeyondProd architecture led Google to innovate several new systems in order to meet these requirements.

### BeyondCorp and BeyondProd

https://cloud.google.com/blog/products/identity-security/applying-zero-trust-to-user-access-and-production-services

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

### Titan Security chip

Titan comprises several components: a secure application processor, a cryptographic co-processor, a hardware random number generator, a sophisticated key hierarchy, embedded [static RAM](https://en.wikipedia.org/wiki/Static_random-access_memory) (SRAM), embedded flash and a read-only memory block. Titan communicates with the main CPU via the [Serial Peripheral Interface](https://en.wikipedia.org/wiki/Serial_Peripheral_Interface) (SPI) bus, and interposes between the boot firmware flash of the first privileged component, e.g., the [BMC](https://en.wikipedia.org/wiki/Intelligent_Platform_Management_Interface) or [Platform Controller Hub](https://en.wikipedia.org/wiki/Platform_Controller_Hub) (PCH), allowing Titan to observe every byte of boot firmware.

https://cloud.google.com/blog/products/identity-security/titan-in-depth-security-in-plaintext


## Access Transparency

[Access Transparency](https://cloud.google.com/logging/docs/audit/access-transparency-overview) provides you with logs that capture the actions Google personnel take when accessing your content. You might be familiar with [Cloud Audit Logs](https://cloud.google.com/logging/docs/audit), which can help you answer questions about "who did what, where, and when?" in your Google Cloud projects. While Cloud Audit Logs provides these logs about the actions taken by members within your own organization, Access Transparency provides logs of the actions taken by Google personnel.



[https://www.youtube.com/watch?v=6BCuIBO0Mhg](https://www.youtube.com/watch?v=6BCuIBO0Mhg)


## Binary Authorization

[Binary Authorization](https://cloud.google.com/binary-authorization/docs) is a service on Google Cloud that provides software supply-chain security for applications that run in the cloud. Binary Authorization is a service on Google Cloud Platform (GCP) that provides software supply-chain security when deploying container-based applications. Binary Authorization extends Google Kubernetes Engine (GKE) and enforces security policies at deploy time. Binary Authorization works with container images from Container Registry or another container image registry. With Binary Authorization, you can automatically and digitally check each component of your software supply chain, ensuring the quality and integrity of your software before an application is deployed to your production environment.



Check out a demo of Binary Authorization, a Google Cloud Platform security feature. Binary Authorization is a deploy-time security control that ensures only trusted container images are deployed on Kubernetes Engine.

[https://www.youtube.com/watch?v=mi50OJq6wd0](https://www.youtube.com/watch?v=mi50OJq6wd0)


### Container image binary authorization


[Binary Authorization](https://cloud.google.com/binary-authorization/) is a deploy-time security control that ensures only trusted container images are deployed on Google Kubernetes Engine (GKE). With Binary Authorization, you can require images to be signed by trusted authorities during the development process and then enforce signature validation when deploying. By enforcing validation, you can gain tighter control over your container environment by ensuring only verified images are integrated into the build-and-release process.





### Binary Authorization Attestations with Voucher

An [attestor](https://cloud.google.com/binary-authorization/docs/creating-attestations-voucher) is a Google Cloud resource that Binary Authorization uses to verify the attestation at container image deploy time. Attestors contain the public key that corresponds to the private key used by a signer to sign the container image digest and create the attestation. 

The Binary Authorization enforcer uses the attestor at deploy time to limit which container images are allowed to be deployed to those with an accompanying, verifiable attestation created prior to deployment.


### Binary Authorization for Borg

https://cloud.google.com/security/binary-authorization-for-borg

## DevSecOps

Whether you call it [DevOps](DevOps) or DevSecOps, it has always been ideal to include security as an integral part of the entire app life cycle. DevSecOps is about built-in security, not security that functions as a perimeter around apps and data. If security remains at the end of the development pipeline, organizations adopting DevOps can find themselves back to the long development cycles they were trying to avoid in the first place.

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


[VPC](VPC) Service Controls enables you to establish security perimeters around sensitive data in Google Cloud Platform services such as [Google Cloud Storage](https://cloud.google.com/storage) and [BigQuery](BigQuery). 

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

[Cloud KMS](Cloud-KMS) is a service that lets you manage symmetric and asymmetric cryptographic keys for your cloud services the same way you do on-premises. 


## reCAPTCHA Enterprise

Google has been defending millions of sites with [reCAPTCHA](https://cloud.google.com/recaptcha-enterprise/docs) for almost a decade. 
reCAPTCHA Enterprise is an extension of that effort to help enterprises detect other types of fraudulent activity on their sites, like scraping, credential stuffing, and automated account creation. reCAPTCHA Enterprise offers enhanced detection with more granular scores, reason codes for risky events, and the ability to tune your site-specific model.  reCAPTCHA Enterprise is a service that protects your site from spam and abuse. reCAPTCHA Enterprise builds on the existing reCAPTCHA API which uses advanced risk analysis techniques to tell humans and bots apart.  reCAPTCHA Enterprise adds enhancements specifically designed to protect enterprise businesses, such as more granular scoring and returning reason codes with low scores to aid in analysis.

[See](https://www.youtube.com/watch?v=ic3Fj2B1LR4) how reCAPTCHA Enterprise can help protect your websites from fraud and abuse.


## Web Risk

[Web Risk](https://cloud.google.com/web-risk/docs) is a new enterprise security product that lets your client applications check URLs against Google's constantly updated lists of unsafe web resources.


### Best practices using Web Risk API to help stop phishing 

https://cloud.google.com/blog/products/identity-security/follow-web-risk-apis-best-practices-to-stop-attacks

## Cloud Audit Logs

Cloud Audit Logs](https://cloud.google.com/logging/docs/audit)  helps security, auditing, and compliance entities maintain audit trails in Google Cloud. With Cloud Audit Logs, your enterprise can attain the same level of transparency over administrative activities and accesses to data in Google Cloud as in on-premises environments. Audit logs help the Google Cloud Support team troubleshoot issues with your account.


## Cloud IDS

Cloud IDS delivers cloud-native, managed, network-based threat detection, built with Palo Alto Networks’ industry-leading threat detection technologies to provide high levels of security efficacy.

https://cloud.google.com/intrusion-detection-system


### Network security threat detection - Comparison of analytics methods


https://cloud.google.com/blog/products/networking/when-to-use-5-telemetry-types-in-security-threat-monitoring

### Identity and Security

https://cloud.google.com/blog/products/identity-security/how-google-cloud-ids-helps-detect-advanced-network-threats

## Leveraging Network Telemetry for Forensics in Google Cloud

https://cloud.google.com/blog/products/networking/open-source-solutions-and-how-tos

## PKI

A [public key infrastructure](https://www.ssh.com/pki/) (PKI) is a set of roles, policies, hardware, software and procedures needed to create, manage, distribute, use, store and revoke [digital certificates](https://en.wikipedia.org/wiki/Public_key_certificate) and manage [public-key encryption](https://en.wikipedia.org/wiki/Public-key_cryptography). The purpose of a PKI is to facilitate the secure electronic transfer of information for a range of network activities such as e-commerce, internet banking and confidential email. It is required for activities where simple passwords are an inadequate authentication method and more rigorous proof is required to confirm the identity of the parties involved in the communication and to validate the information being transferred.


## OAuth, OpenID Connect, SAML

### OAuth

[OAuth](https://en.wikipedia.org/wiki/OAuth) is an open standard for access delegation, commonly used as a way for Internet users to grant websites or applications access to their information on other websites but without giving them the passwords. f you’ve ever signed up to a new application and agreed to let it automatically source new contacts via Facebook or your phone contacts, then you’ve likely used OAuth 2.0. This standard provides secure delegated access. 

### SAML

[Security Assertion Markup Language](https://en.wikipedia.org/wiki/Security_Assertion_Markup_Language) (SAML) is an open standard for exchanging authentication and authorization data between parties, in particular, between an identity provider and a service provider. You’ve more likely experienced SAML authentication in action in the work environment. For example, it enables you to log into your corporate intranet or IdP and then access numerous additional services, such as Salesforce, Box, or Workday, without having to re-enter your credentials.

### OpenID

[OpenID](https://en.wikipedia.org/wiki/OpenID) Connect allows clients of all types, including Web-based, mobile, and JavaScript clients, to request and receive information about authenticated sessions and end-users. The specification suite is extensible, allowing participants to use optional features such as encryption of identity data, discovery of OpenID Providers, and session management, when it makes sense for them.  If you’ve used your Google to sign in to applications like YouTube, or Facebook to log into an online shopping cart, then you’re familiar with this authentication option. OpenID Connect is an open standard that organizations use to authenticate users.


### Comparisons

[https://www.okta.com/identity-101/whats-the-difference-between-oauth-openid-connect-and-saml/](https://www.okta.com/identity-101/whats-the-difference-between-oauth-openid-connect-and-saml/)



## Machine Learning for Cybersecurity

There have been attempts to aid Cybersecurity concerns using [Machine Learning](Machine-Learning).

### NTA

[ML in network security](https://towardsdatascience.com/machine-learning-for-cybersecurity-101-7822b802790b) implies new solutions called [Network Traffic Analytics]( https://www.cisco.com/c/en/us/products/security/what-is-network-traffic-analysis.html  ) (NTA) aimed at in-depth analysis of all the traffic at each layer and detect attacks and anomalies.

## Data Governance 


[Data governance](data-governance) is a principled approach to manage data during its lifecycle — from acquisition, to use, to disposal.




## Cloud Governance

[Cloud governance](Cloud-Governance) is a set of practices that help ensure users operate in the cloud in ways that they want, that the operations are efficient, and that the user can monitor and correct operations as needed. A cloud governance framework is not a new set of concepts or practices, but simply the application of existing governance practices to cloud operations.
## BigQuery Security

### BigQuery Column-level security

[https://cloud.google.com/blog/products/data-analytics/data-governance-new-ways-to-securely-access-and-discover-data](https://cloud.google.com/blog/products/data-analytics/data-governance-new-ways-to-securely-access-and-discover-data)



### BigQuery row level security

https://cloud.google.com/blog/products/data-analytics/bigquery-provides-tighter-controls-over-data-access

## Access Context Manager

[Access Context Manager](https://cloud.google.com/access-context-manager/docs/overview) allows Google Cloud organization administrators to define fine-grained, attribute based access control for projects and resources in Google Cloud.

Administrators first define an access policy, which is an organization-wide container for access levels and service perimeters.

Access levels describe the necessary requirements for requests to be honored. 



## BGP

Internet routing depends on continuous  correct configuration and operation of its routing protocols. The dynamic nature of the [routing protocols](Router) means [the risks associated](  https://www.secureworks.com/research/bgp-hijacking-for-cryptocurrency-profit  ) must be considered.

## Kubernetes security

[Kubernetes Security](Kubernetes-Security)  is important throughout the container lifecycle due to the distributed, dynamic nature of a Kubernetes cluster. Different security approaches are required for each of the three phases of an application lifecycle: build, deploy, and runtime. 

## IPSec

https://www.juniper.net/documentation/us/en/software/junos/vpn-ipsec/topics/topic-map/security-ipsec-vpn-overview.html

### Cryptographic evaluation of IPSec

http://citeseerx.ist.psu.edu/viewdoc/summary?doi=10.1.1.33.7922

### AES Key agility issues

https://www.researchgate.net/publication/2646713_AES_Key_Agility_Issues_in_High-Speed_IPsec_Implementations

## Comparison of VPN Protocols

There are many [VPNs](VPN).

https://www.ivpn.net/pptp-vs-ipsec-ikev2-vs-openvpn-vs-wireguard/

## IoT Security

https://internetofthingsagenda.techtarget.com/definition/IoT-security-Internet-of-Things-security



## Using OAuth 2.0 to Access Google APIs

Google APIs use the [OAuth 2.0 protocol](https://datatracker.ietf.org/doc/html/rfc6749) for authentication and authorization. Google supports common OAuth 2.0 scenarios such as those for web server, client-side, installed, and limited-input device applications.

## DNS Security

The [Domain Name System]( DNS  ) Security Extensions (DNSSEC) is a feature of the Domain Name System (DNS) that authenticates responses to domain name lookups. [DNSSEC](https://en.wikipedia.org/wiki/Domain_Name_System_Security_Extensions) does not provide privacy protections for those lookups, but prevents attackers from manipulating or poisoning the responses to DNS requests.

https://cloud.google.com/dns/docs/dnssec

### DNS over TLS

https://developers.google.com/speed/public-dns/docs/dns-over-tls

### DNS over HTTPS

https://wikipedia.org/wiki/DNS_over_HTTPS

## Cloud Storage Security

https://www.researchgate.net/publication/300003200_Security_Techniques_for_Data_Protection_in_Cloud_Computing

### Enhance Security in cloud storage

https://cloud.google.com/blog/products/storage-data-transfer/5-ways-to-enhance-your-cloud-storage-security-and-data-protection

### Cloud Storage security issues

https://www.researchgate.net/publication/306071422_A_Study_on_Data_Storage_Security_Issues_in_Cloud_Computing

### GDPR

https://gdpr-info.eu/

### Credential Types Supporting Various Use Cases

https://cloud.google.com/storage/docs/gsutil/addlhelp/CredentialTypesSupportingVariousUseCases


## Examine Google Cloud Platform security vulnerabilities using Cloud Functions

Monitor security threats in IAM and Firewall via Cloud Functions.

https://blog.searce.com/examine-google-cloud-platform-security-vulnerabilities-using-cloud-functions-40f1d96d69a4


## Confidential Computing

Encrypt data in-use with Confidential VMs and Confidential GKE Nodes.

https://cloud.google.com/confidential-computing


## Google Cloud Vault Secrets Engine


The Google Cloud Vault secrets engine dynamically generates Google Cloud service account keys and OAuth tokens based on IAM policies. This enables users to gain access to Google Cloud resources without needing to create or manage a dedicated service account.


https://www.vaultproject.io/docs/secrets/gcp

https://registry.terraform.io/providers/hashicorp/vault/latest/docs

## BYOD

### Managed Devices

https://cloud.google.com/identity/docs/concepts/managed-devices

### G Suite and BYOD

https://cloud.google.com/blog/products/g-suite/use-byod-safely-in-g-suite-with-these-6-controls-

### Endpoint verification

https://cloud.google.com/blog/products/gcp/introducing-endpoint-verification-visibility-into-the-desktops-accessing-your-enterprise-applications


## ACL


An [access control list](https://en.wikipedia.org/wiki/Access-control_list) (ACL) is a mechanism you can use to define who has access to your buckets and objects, as well as what level of access they have. In Cloud Storage, you apply ACLs to individual buckets and objects. Each ACL consists of one or more entries. An entry gives a specific user (or group) the ability to perform specific actions. Each entry consists of two pieces of information:

A permission, which defines what actions can be performed (for example, read or write).

A scope (sometimes referred to as a grantee), which defines who can perform the specified actions (for example, a specific user or group of users).


https://cloud.google.com/storage/docs/gsutil/addlhelp/SecurityandPrivacyConsiderations#access-control-lists

### Predefined ACLs


A predefined or "canned" ACL is an alias for a set of specific ACL entries that you can use to quickly apply many ACL entries at once to a bucket or object.

https://cloud.google.com/storage/docs/access-control/lists#predefined-acl


### Concentric permissions and scopes


Cloud Storage uses concentric permissions, so when you grant WRITER permission, you also grant READER permission, and if you grant OWNER permission, you also grant READER and WRITER permission.

https://cloud.google.com/storage/docs/access-control/lists#concentric

### CORS

Cross Origin Resource Sharing (CORS) allows interactions between resources from different origins, something that is normally prohibited in order to prevent malicious behavior. 

https://cloud.google.com/storage/docs/configuring-cors

### RBAC

[Role-based access control](https://en.wikipedia.org/wiki/Role-based_access_control) (RBAC) is a policy-neutral access-control mechanism defined around roles and privileges.


#### Tailscale

https://tailscale.com/kb/1018/acls/

## Vulnerability scanning


https://cloud.google.com/security-command-center/docs/concepts-web-security-scanner-overview


### SCC

https://cloud.google.com/security-command-center/




### Forseti

https://forsetisecurity.org/


### OWASP

https://owasp.org/

### Aqua CSPM

https://www.aquasec.com/products/cspm/

### Cloud guard


https://www.checkpoint.com/solutions/cloud-security/#

### Cloud Security Suite

https://github.com/SecurityFTW/cs-suite

### Cloudspoilt

https://cloudsploit.com/google


### Cloud Custodian

https://github.com/cloud-custodian/cloud-custodian


### GCP bucket brute

https://github.com/RhinoSecurityLabs/GCPBucketBrute

### Prisma

https://www.paloaltonetworks.com/prisma/environments/gcp


### Snyk

https://snyk.io/

### McAfee MVision


https://www.mcafee.com/enterprise/en-us/solutions/mvision.html



### Netskope

https://www.netskope.com/products/google-cloud-platform


### Tripwire

https://www.tripwire.com/solutions/cloud-cybersecurity



### ScoutSuite


https://github.com/nccgroup/ScoutSuite

## Cyber attack

https://geekflare.com/cyberattack-simulation-tools/

### CrowdSec

[CrowdSec](  https://github.com/crowdsecurity/crowdsec ) - an open-source massively multiplayer firewall able to analyze visitor behavior & provide an adapted response to all kinds of attacks. It also leverages the crowd power to generate a global IP reputation database to protect the user network.



## Qwiklabs

### Cloud KMS

[Getting Started with Cloud KMS](https://www.qwiklabs.com/focuses/1713?catalog_rank=%7B%22rank%22%3A20%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&parent=catalog&search_id=7468061)


[Security & Identity Fundamentals](https://www.qwiklabs.com/quests/40?catalog_rank=%7B%22rank%22%3A1%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&search_id=7482841)

[Ensure Access & Identity in Google Cloud](https://www.qwiklabs.com/quests/150?catalog_rank=%7B%22rank%22%3A3%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&search_id=7482841)
