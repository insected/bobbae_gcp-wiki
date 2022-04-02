[Authentication](https://cloud.google.com/docs/authentication) determines who you are, [authorization](IAM) determines what you can do, and [auditing logs](https://cloud.google.com/logging/docs/audit) what you did.


## Principals

A principal is an entity, also known as an identity, that can be granted access to a resource. Google Cloud APIs support two types of principals: user accounts and [service accounts](Service-accounts).

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

Google Cloud APIs support [multiple authentication flows](https://cloud.google.com/docs/authentication#strategies
) for different runtime environments. 

### IAP
[IAP](IAP) lets you establish a central authorization layer for applications accessed by HTTPS, so you can use an application-level access control model instead of relying on network-level firewalls.




### OAuth 2.0

https://tools.ietf.org/html/rfc6749

https://developer.okta.com/blog/2019/10/21/illustrated-guide-to-oauth-and-oidc

### OpenAPI

[Cloud Endpoints](Endpoints) supports APIs that are described using version 2.0 of the OpenAPI specification.

https://cloud.google.com/endpoints/docs/openapi/openapi-overview

### Using Okta to authenticate users.

https://cloud.google.com/endpoints/docs/openapi/authenticating-users-okta

### Using Auth0 to authenticate users

https://cloud.google.com/endpoints/docs/openapi/authenticating-users-auth0

### Using Firebase to authenticate users

https://cloud.google.com/endpoints/docs/openapi/authenticating-users-firebase

### Using Google ID tokens to authenticate users

https://cloud.google.com/endpoints/docs/openapi/authenticating-users-google-id

## Active Directory


[Managed Service for Microsoft Active Directory](https://cloud.google.com/managed-microsoft-ad
) (AD) is a highly available, hardened Google Cloud service running actual [Microsoft AD](Active-Directory) that enables you to manage authentication and authorization for your AD-dependent workloads, automate AD server maintenance and security configuration, and connect your on-premises AD domain to the cloud.




## Access control and Authentication Options

[Access control for Google Cloud APIs](https://cloud.google.com/storage/docs/access-control) encompasses authentication, authorization, and auditing. 


[Service accounts](Service-accounts) are managed by [IAM](IAM) and are intended for scenarios where your application needs to access resources or perform actions on its own, such as running App Engine apps or interacting with Compute Engine instances. 


[https://cloud.google.com/blog/products/identity-security/identity-and-authentication-the-google-cloud-way](https://cloud.google.com/blog/products/identity-security/identity-and-authentication-the-google-cloud-way)


## Authentication between services

https://cloud.google.com/endpoints/docs/openapi/service-account-authentication

## Tokens

### JWT

[JSON Web Tokens](https://jwt.io/) are an open, industry standard RFC 7519 method for representing claims securely between two parties.

### PASETO

https://developer.okta.com/blog/2019/10/17/a-thorough-introduction-to-paseto

## Examples

https://cloud.google.com/docs/authentication#examples

