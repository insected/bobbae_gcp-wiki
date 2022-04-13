Using Workload identity federation, you can grant on-premises or multi-cloud workloads access to Google Cloud resources, without using a service account key.


Traditionally, applications running outside Google Cloud have used service account keys to access Google Cloud resources. [Service account](Service-accounts) keys are powerful credentials and can represent a security risk if they are not managed correctly.

With identity federation, you can use [Identity and Access Management](IAM) (IAM) to grant external identities IAM roles, including the ability to impersonate service accounts. This lets you access resources directly, using a short-lived access token, and eliminates the maintenance and security burden associated with service account keys.

You can use identity federation with Amazon Web Services (AWS), or with any identity provider that supports OpenID Connect (OIDC), such as Microsoft Azure.


https://cloud.google.com/iam/docs/workload-identity-federation

### OIDC

https://ldapwiki.com/wiki/OpenID%20Connect


https://goteleport.com/blog/how-oidc-authentication-works/

https://www.ibm.com/docs/en/sva/9.0.5?topic=methods-openid-connect-oidc-authentication


### Openid-configuration

https://ldapwiki.com/wiki/Openid-configuration




### Obtaining short-lived credentials with identity federation 

https://cloud.google.com/iam/docs/using-workload-identity-federation

### Configuring workload identity federation

https://cloud.google.com/iam/docs/configuring-workload-identity-federation

### Access GCP from AWS using Workload Identity Federation

https://scalesec.com/blog/access-gcp-from-aws-using-workload-identity-federation/


### How to use Google's workload federation with AWS


https://www.techtarget.com/searchcloudcomputing/tip/How-to-use-Googles-workload-identity-federation-with-AWS

### GitHub Actions and Workload Identity Federation

https://medium.com/kpmg-uk-engineering/workload-identity-federation-authenticate-github-actions-to-google-cloud-f773079e1336

### GitLab and Workload Identity Federation

https://gbostoen.medium.com/integrate-gitlab-with-google-cloud-workload-identity-federation-7afb2aac3a89

### Using Workload Identity to access Google Cloud Pub/Sub from GKE

https://medium.com/@karthikg_54738/using-workload-identity-to-access-google-cloud-pub-sub-from-gke-2d6818d58f83

### Enabling keyless authentication from GitHub actions

https://cloud.google.com/blog/products/identity-security/enabling-keyless-authentication-from-github-actions


### Keyless GCP authentication from GitHub actions with workload identity federation

https://alwaysupalwayson.com/posts/2022/01/workload-identity-federation/



### SPIFFE


https://spiffe.io/docs/latest/spiffe-about/overview/


### Workload Identity Federation for On-Premise Workloads with SPIFFE

https://medium.com/google-cloud/workload-identity-federation-for-on-premise-workloads-with-spiffe-24a861b3cf6c

