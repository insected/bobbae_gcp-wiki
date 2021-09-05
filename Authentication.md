[Authentication](https://cloud.google.com/docs/authentication) determines who you are, [authorization](IAM) determines what you can do, and [auditing logs](https://cloud.google.com/logging/docs/audit) what you did.


## Principals

A principal is an entity, also known as an identity, that can be granted access to a resource. Google Cloud APIs support two types of principals: user accounts and service accounts.

https://cloud.google.com/docs/authentication#principals

## Applications

[Application credentials](https://console.cloud.google.com/apis/credentials/) provide the required information about the caller making a request to a Google Cloud API. 

https://cloud.google.com/docs/authentication#applications

### Best practices

Best practices to securely authenticate applications in Google Cloud.

https://cloud.google.com/docs/authentication/best-practices-applications

### Authenticating as a service account 


https://cloud.google.com/docs/authentication/production

## Authentication Strategies

Google Cloud APIs support multiple authentication flows for different runtime environments. 

https://cloud.google.com/docs/authentication#strategies

### OAuth 2.0

https://tools.ietf.org/html/rfc6749

### OpenAPI

#### Using Okta to authenticate users.

https://cloud.google.com/endpoints/docs/openapi/authenticating-users-okta

#### Using Auth0 to authenticate users

https://cloud.google.com/endpoints/docs/openapi/authenticating-users-auth0

#### Using Firebase to authenticate users

https://cloud.google.com/endpoints/docs/openapi/authenticating-users-firebase

#### Using Google ID tokens to authenticate users

https://cloud.google.com/endpoints/docs/openapi/authenticating-users-google-id

## Active Directory


Managed Service for Microsoft Active Directory (AD) is a highly available, hardened Google Cloud service running actual [Microsoft AD](Active-Directory) that enables you to manage authentication and authorization for your AD-dependent workloads, automate AD server maintenance and security configuration, and connect your on-premises AD domain to the cloud.

https://cloud.google.com/managed-microsoft-ad


## Examples

https://cloud.google.com/docs/authentication#examples
