[Information Security](https://wikipedia.org/wiki/Information_security   ), sometimes shortened to InfoSec, is the practice of protecting information by mitigating information risks.


The Internet has transformed our lives in many good ways. Unfortunately, this vast network and its associated technologies also have brought in their wake, [the increasing number of security threats](https://wikipedia.org/wiki/Internet_security
). 

GCP doesn't rely on any single technology to make its [infrastructure secure](https://cloud.google.com/security/infrastructure). GCP [delivers](   https://cloud.google.com/blog/products/identity-security/delivering-the-industrys-most-trusted-cloud ) security through [progressive layers](https://www.youtube.com/watch?v=MHtg2Au78LI&list=PLIivdWyY5sqLO-4ePY-A2yROgONOA6Cz4) that deliver [true defense in depth](https://www.youtube.com/watch?v=vBdYVFgZ2ug). [Google datacenter security](https://www.youtube.com/watch?v=UOdUC8DhprQ) has [6 layers](https://www.youtube.com/watch?v=kd33UVZhnAA). 

## Security Command Center

[Security Command Center](https://cloud.google.com/security-command-center) is Google Cloud's centralized vulnerability and threat reporting service.

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

Google Cloud security diagnostic tool called [Risk Manager](https://cloud.google.com/risk-manager/docs) enables customers to measure and manage their risk on Google Cloud and obtain a report on their security posture. 

https://cloud.google.com/risk-protection-program

## Security Infrastructure Design

Read the [overview of how security is designed](https://cloud.google.com/security/infrastructure/design/) into Google's technical infrastructure. 

https://cloud.google.com/blog/topics/developers-practitioners/foundational-best-practices-securing-your-cloud-deployment

## Cryptography

[Cryptography](Cryptography)  is the study of secure communications techniques that allow only the sender and intended recipient of a message to view its contents.

### Encryption at Rest



Google Cloud encrypts all customer content stored [at rest](Encryption-at-Rest), without any action required from the customer, using one or more encryption mechanisms.




## Security and Identity


[Identity-based security](https://en.wikipedia.org/wiki/Identity-based_security) is a type of security that focuses on access to digital information or services based on the authenticated [identity](Identity-Management) of an individual.  


## Roles

A role contains a set of permissions that allows you to perform specific actions on Google Cloud resources. To make permissions available to members, including users, groups, and service accounts, you grant roles to the members.

[https://cloud.google.com/iam/docs/understanding-roles](https://cloud.google.com/iam/docs/understanding-roles)


## Service Accounts


[A Service Account](Service-Accounts)  is a special kind of account used by an application or a virtual machine (VM) instance, not a person. Applications use service accounts to make authorized API calls, authorized as either the service account itself, or as Google Workspace or Cloud Identity users through domain-wide delegation.

## Cloud Identity API

[Cloud Identity](https://cloud.google.com/identity/docs) API is an API for provisioning and managing identity resources.
It helps you achieve [confidentiality, data integrity, availability, non-repudiation and authentication of your data.](https://cloud.google.com/blog/products/identity-security)

Cloud Identity is an Identity as a Service (IDaaS) solution that centrally manages users and groups. You can configure Cloud Identity to federate identities between Google and other identity providers, such as [Active Directory](https://cloud.google.com/architecture/identity/federating-gcp-with-active-directory-introduction) and [Azure Active Directory](https://cloud.google.com/architecture/identity/federating-gcp-with-azure-active-directory).


## Access Control

[Access Control](Access-Control) is a mechanism you can use to define who has access to resources.



### IAM

[Identity and Access Management](IAM)  lets administrators authorize who can take action on specific resources, giving you full control and visibility. 


### Identity-Aware Proxy

[Identity-Aware Proxy](https://cloud.google.com/iap/docs) (IAP) lets you manage access to applications running in the App Engine standard environment, App Engine flexible environment, Compute Engine, and GKE. 

### Context-Aware Access

Based on the [BeyondCorp](https://cloud.google.com/beyondcorp) security model, [Context-Aware Access](Context-Aware-Access) is an approach that utilizes a variety of Google Cloud offerings to enforce granular access control based on a user's identity and context of the request.





## Identity Platform

[Google Identity Platform](https://cloud.google.com/identity-platform/docs) provides back-end services, SDKs, and UI libraries that make it easier to [authenticate users to your apps and services](https://www.youtube.com/watch?v=O_O5Hb1bJyw).




## Managed Services for Microsoft Active Directory

[Managed Service for Microsoft Active Directory](https://cloud.google.com/managed-microsoft-ad/docs) is a highly available, hardened Google Cloud service running actual Microsoft AD that enables you to manage your cloud-based AD-dependent workloads, automate AD server maintenance and security configuration, and connect your on-premises AD domain to the cloud.



## Resource Manager

The [Resource Manager](Resource-Manager) API enables you to programmatically manage these container resources.


## Security Key management

[Cloud KMS](Cloud-KMS), together with [Cloud HSM](https://cloud.google.com/kms/docs/hsm) and [Cloud EKM](https://cloud.google.com/kms/docs/ekm), supports a wide range of compliance mandates that call for specific key management procedures and technologies.  You can manage encryption keys via [secure hardware](Hardware-Key-devices).


## Access Transparency

[Access Transparency](https://cloud.google.com/logging/docs/audit/access-transparency-overview) provides you with logs that capture the actions Google personnel take when accessing your content. You might be familiar with [Cloud Audit Logs](https://cloud.google.com/logging/docs/audit), which can help you answer questions about "who did what, where, and when?" in your Google Cloud projects. While Cloud Audit Logs provides these logs about the actions taken by members within your own organization, [Access Transparency](https://www.youtube.com/watch?v=6BCuIBO0Mhg) provides logs of the actions taken by Google personnel.




## Binary Authorization

[Binary Authorization](Binary-Authorization) is a service on Google Cloud Platform (GCP) that provides software supply-chain security when deploying container-based applications. 


## Cloud Asset Inventory

[Cloud Asset Inventory](https://cloud.google.com/asset-inventory/docs/overview) provides inventory services based on a time series database. This database keeps a five-week history of Google Cloud [asset](https://cloud.google.com/asset-inventory/docs/overview#assets) metadata.



## Cloud Data Loss Prevention

[Cloud Data Loss Prevention (DLP)](https://cloud.google.com/dlp/docs) provides [access](http://bit.ly/2QmSZsr) to a powerful [sensitive data inspection](https://www.youtube.com/watch?v=GArEb2e9jGk), classification, and de-identification platform.




## Cloud HSM

[Cloud HSM](https://cloud.google.com/kms/docs/hsm) is a cloud-hosted Hardware Security Module (HSM) service that allows you to host encryption keys and perform cryptographic operations in a cluster of [FIPS 140-2 Level 3](https://csrc.nist.gov/publications/detail/fips/140/2/final) certified HSMs. Google manages [the HSM cluster](https://www.youtube.com/watch?v=DB6UfKFo3ds) for you, so you don't need to worry about clustering, scaling, or patching. Because Cloud HSM uses Cloud KMS as its front end, you can leverage all the conveniences and features that Cloud KMS provides.


## Security Command Center

[Security Command Center](https://cloud.google.com/security-command-center/docs) is the canonical security and data risk database for Google Cloud. [Security Command Center](https://www.youtube.com/watch?v=k7ZEfAocMq4) enables you to understand your security and data attack surface by providing asset inventory, discovery, search, and management.



## VPC Service Controls

With [VPC Service Controls](https://cloud.google.com/vpc-service-controls/docs), administrators can define a security perimeter around resources of Google-managed services to [control communication to and between those services](https://www.youtube.com/watch?v=EXwJFL24QzY).


[VPC](VPC) Service Controls enables you to establish security perimeters around sensitive data in Google Cloud Platform services such as [Google Cloud Storage](https://cloud.google.com/storage) and [BigQuery](BigQuery). 



## Incident Response and Management

The [incident](https://cloud.google.com/monitoring/alerts/incidents-events) response problem space can be divided into three categories: people, process, and data management. 

Users have long had access to solid people-management solutions (on-call rotation schedulers, etc.) and Google’s [SRE book](https://sre.google/sre-book/table-of-contents/) outlines their [Incident Management](https://cloud.google.com/blog/products/management-tools/meeting-reliability-challenges-with-sre-principles) at Google (IMAG) process. 

The  [Stackdriver](https://cloud.google.com/monitoring) supports [Incident Response and Management](https://www.youtube.com/watch?v=VXqfbp_zE0c) (IRM)  Insights and the supporting GCP technology that makes the innovation possible.



## Phishing Protection

[Phishing Protection](https://cloud.google.com/phishing-protection/docs) is a phishing countermeasure platform that helps to detect phishing attacks against your users. 

The Phishing Protection Submission API also enables you to submit URLs suspected to be unsafe to [Safe Browsing](http://safebrowsing.google.com/). 

Any URLs that are confirmed to match the Safe Browsing Policies will be added to the Safe Browsing list, which is used by over three billion devices to show warnings when a user visits a known unsafe web resource. Common sources of these URLs are customer reports or internal phishing detection results.

[Security keys prevent phishing attacks](https://www.youtube.com/watch?v=c9EOETFnB74) by recognizing a domain name and using its hidden private key. 



## Cloud KMS

[Cloud KMS](Cloud-KMS) is a service that lets you manage symmetric and asymmetric cryptographic keys for your cloud services the same way you do on-premises. 


## reCAPTCHA Enterprise

Google has been defending millions of sites with [reCAPTCHA](https://cloud.google.com/recaptcha-enterprise/docs) for almost a decade. 
[reCAPTCHA](https://www.youtube.com/watch?v=ic3Fj2B1LR4) Enterprise is an extension of that effort to help enterprises detect other types of fraudulent activity on their sites, like scraping, credential stuffing, and automated account creation. 



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

GCP [Certificate Authority Service](https://cloud.google.com/certificate-authority-service) implements [PKI](PKI) and private [CAs](https://en.wikipedia.org/wiki/Certificate_authority).


## OAuth, OpenID Connect, SAML

[Federated Identity Management](Identity-Management) methods include OAuth, OpenID and SAML.


## Machine Learning for Cybersecurity

There have been attempts to aid Cybersecurity concerns using [Machine Learning](Machine-Learning).

### NTA

[ML in network security](https://towardsdatascience.com/machine-learning-for-cybersecurity-101-7822b802790b) implies new solutions called [Network Traffic Analytics]( https://www.cisco.com/c/en/us/products/security/what-is-network-traffic-analysis.html  ) (NTA) aimed at in-depth analysis of all the traffic at each layer and detect attacks and anomalies.

## Data Governance 


[Data governance](data-governance) is a principled approach to manage data during its lifecycle — from acquisition, to use, to disposal.


### Data De-risk methods

https://medium.com/google-cloud/de-risk-your-data-to-accelerate-your-cloud-journey-part-3-turning-design-into-reality-363fd6c21e41

## Cloud Governance

[Cloud governance](Cloud-Governance) is a set of practices that help ensure users operate in the cloud in ways that they want, that the operations are efficient, and that the user can monitor and correct operations as needed. A cloud governance framework is not a new set of concepts or practices, but simply the application of existing governance practices to cloud operations.

## BigQuery Security

[BigQuery](BigQuery) Security topics include [Column-level security](https://cloud.google.com/bigquery/docs/column-level-security-intro) and [row-level security](https://cloud.google.com/bigquery/docs/row-level-security-intro).




## BGP

The [Border Gateway Protocol](BGP) (BGP) is the protocol used throughout the Internet to exchange routing information between networks. The dynamic nature of the [routing protocols](Router) means [the risks associated](  https://www.secureworks.com/research/bgp-hijacking-for-cryptocurrency-profit  ) must be considered.

The challenge with BGP is that the protocol does not directly include security mechanisms and is based largely on trust between network operators that they will secure their systems correctly and not send incorrect data. 

[RFC 7454](https://tools.ietf.org/html/rfc7454) discusses BGP related Operations and Security issues.

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

Google APIs use the [OAuth 2.0 protocol](https://datatracker.ietf.org/doc/html/rfc6749) for [authentication](Authentication) and authorization. Google supports common OAuth 2.0 scenarios such as those for web server, client-side, installed, and limited-input device applications.

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
