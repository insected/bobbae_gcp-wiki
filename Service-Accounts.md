A [service account](  https://cloud.google.com/iam/docs/service-accounts ) is a special kind of account used by an application or a virtual machine (VM) instance, not a person. Applications use service accounts to make authorized API calls, authorized as either the service account itself, or as Google Workspace or Cloud Identity users through domain-wide delegation.

https://www.youtube.com/watch?v=xXk1YlkKW_k&list=PLIivdWyY5sqIlPnZ7cvkg2Ck-8ZZ8TA5t

For example, a Compute Engine VM can run as a service account, and that account can be given permissions to access the resources it needs. This way the service account is the identity of the service, and the service account's permissions control which resources the service can access.

A service account is identified by its email address, which is unique to the account.

https://cloud.google.com/iam/docs/service-accounts

## Difference between a service account and a user account

Service accounts are associated with private/public [RSA](https://en.wikipedia.org/wiki/RSA_Security) key-pairs that are used for authentication to Google. You can let other users or service accounts impersonate a service account. 

### Service Accounts and Google Workspace

Service accounts are not members of your [Google Workspace](https://support.google.com/domains/answer/6069226) domain, unlike user accounts. If you share Google Workspace assets, like docs or events, with all members in your Google Workspace domain, they are not shared with service accounts. Similarly, Google Workspace assets created by a service account are not created in your Google Workspace domain. As a result, your [Google Workspace](https://workspace.google.com/) and [Cloud Identity](https://cloud.google.com/identity) admins can't own or manage these assets.

## Default service account

If your application runs in a Google Cloud environment that has a default service account, your application can use the credentials for the default service account to call Google Cloud APIs. Alternatively, you can create your own user-managed service account and use it to authenticate. 

https://cloud.google.com/iam/docs/service-accounts#default

## Google managed service accounts

https://cloud.google.com/iam/docs/service-accounts#google-managed

## Service account locations

https://cloud.google.com/iam/docs/service-accounts#locations

## Short lived service account credentials

https://cloud.google.com/iam/docs/service-accounts#short-lived_service_account_credentials

### Creating short-lived service account credentials

https://cloud.google.com/iam/docs/creating-short-lived-service-account-credentials

### Impersonated Credentials

https://salmaan-rashid.medium.com/using-impersonatedcredentials-for-google-cloud-apis-and-idtokens-4ec18013fd91

### Account impersonation for local testing of apps

https://medium.com/google-cloud/run-your-app-locally-as-if-you-were-on-google-cloud-2722e33e5656

## Finding credentials automatically 

If your application runs inside a Google Cloud environment, and you have attached a service account to that environment, your application can retrieve credentials for the service account. The application can then use the credentials to call Google Cloud APIs.

https://cloud.google.com/docs/authentication/production

## ADC Application Default Credentials

Google Cloud Client Libraries use a library called [Application Default Credentials](https://cloud.google.com/iam/docs/service-accounts#application_default_credentials) (ADC) to automatically find your service account credentials. ADC looks for service account credentials in the following order

1. If the environment variable GOOGLE_APPLICATION_CREDENTIALS is set, ADC uses the service account key or configuration file that the variable points to.
2. If the environment variable GOOGLE_APPLICATION_CREDENTIALS isn't set, ADC uses the service account that is attached to the resource that is running your code.
3. This service account might be a default service account provided by Compute Engine, Google Kubernetes Engine, App Engine, Cloud Run, or Cloud Functions. It might also be a user-managed service account that you created.

If ADC can't use any of the above credentials, an error occurs.



https://cloud.google.com/docs/authentication/production#automatically

## Service account impersonation

The token exchange flow returns a [federated access token](https://cloud.google.com/iam/docs/workload-identity-federation). You can use this token to impersonate a service account and obtain a short-lived OAuth 2.0 access token. The short-lived access token lets you call any Google Cloud APIs that the service account has access to.



https://cloud.google.com/iam/docs/workload-identity-federation#impersonation


## Workload identity federation

You can use identity federation with Amazon Web Services (AWS), or with any identity provider that supports OpenID Connect (OIDC), such as Microsoft Azure.


https://cloud.google.com/iam/docs/workload-identity-federation

### GitHub Actions and Workload Identity Federation

https://medium.com/kpmg-uk-engineering/workload-identity-federation-authenticate-github-actions-to-google-cloud-f773079e1336

### GitLab and Workload Identity Federation

https://gbostoen.medium.com/integrate-gitlab-with-google-cloud-workload-identity-federation-7afb2aac3a89

### Using Workload Identity to access Google Cloud Pub/Sub from GKE

https://medium.com/@karthikg_54738/using-workload-identity-to-access-google-cloud-pub-sub-from-gke-2d6818d58f83

## Securing Service Accounts

https://cloud.google.com/iam/docs/best-practices-for-securing-service-accounts

## Investigation of Service Account usage

https://cloud.google.com/blog/products/identity-security/three-services-to-investigate-gcp-service-account-usage

## Service agents

Some Google Cloud services have Google-managed service accounts that allow the services to access your resources. These service accounts are sometimes known as service agents.

https://cloud.google.com/iam/docs/service-agents

## Best Practices

Service accounts represent non-human users. They're intended for scenarios where a workload, such as a custom application, needs to access resources or perform actions without end-user involvement. Service accounts can be used for many different purposes, but they aren't always the best choice.

Not every application interacts with human users—instead, an application might be running in the background unattended. Unattended applications include batch jobs, worker processes that dispatch messages read from a queue, or a resource-monitoring agent.

Whenever an unattended application needs to access a resource, like a Cloud Storage bucket, it must act on its own behalf, not on behalf of any end-user. To act on its own behalf, an application needs its own identity that's unrelated to any end-user identity.

https://cloud.google.com/iam/docs/granting-changing-revoking-access

To equip an application with its own identity, create a service account for the application, and grant the service account access to the resources that the application needs to access. By letting an application use its own service account, you help ensure that the application can work without user interaction. In addition, you also ensure that any resource accesses initiated by the application can be attributed back to the same application.



https://cloud.google.com/iam/docs/best-practices-for-using-and-managing-service-accounts

## terraform support for SA

https://github.com/terraform-google-modules/terraform-google-service-accounts


## Secure service account keys by eliminating them

https://medium.com/@derekheld/secure-your-google-service-account-keys-by-eliminating-them-14f8aa679d73

## Examples

```

SERVICE_ACCOUNT_NAME=example-gcs-svc-account
SERVICE_ACCOUNT_DEST=~/example-gcs-svc-account.json

gcloud iam service-accounts create \
    $SERVICE_ACCOUNT_NAME \
    --display-name $SERVICE_ACCOUNT_NAME

SA_EMAIL=$(gcloud iam service-accounts list \
    --filter="displayName:$SERVICE_ACCOUNT_NAME" \
    --format='value(email)')

PROJECT=$(gcloud config get-value project)

gcloud projects add-iam-policy-binding $PROJECT \
    --role roles/storage.admin --member serviceAccount:$SA_EMAIL

mkdir -p $(dirname $SERVICE_ACCOUNT_DEST)

gcloud iam service-accounts keys create $SERVICE_ACCOUNT_DEST \
    --iam-account $SA_EMAIL

gcloud iam roles list

gcloud projects get-iam-policy $PROJECT

gcloud projects get-iam-policy $PROJECT --flatten=bindings[].members --format=table(bindings.role) --filter=bindings.members:$SA_EMAIL
```

### Using gcloud to create and configure a service account

https://fabianlee.org/2021/01/30/gcp-using-gcloud-to-create-and-configure-a-service-account/

### Self made service account key

https://medium.com/@alexnikdanilin/how-to-use-self-made-service-account-key-with-expiration-date-on-google-cloud-platform-bf5a33c2685a