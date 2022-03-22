
[Access Control](https://cloud.google.com/s/results/?q=access%20control) is a mechanism you can use to define who has access to resources.


### IAM

[Identity and Access Management](IAM)  lets administrators authorize who can take action on specific resources, giving you full control and visibility. 



### Context-Aware Access

Based on the [BeyondCorp](https://cloud.google.com/beyondcorp) security model, [Context-Aware Access](Context-Aware-Access) is an approach that utilizes a variety of Google Cloud offerings to enforce granular access control based on a user's identity and context of the request.




### Identity-Aware Proxy

[Identity-Aware Proxy](https://cloud.google.com/iap/docs) (IAP) lets you manage access to applications running in the App Engine standard environment, App Engine flexible environment, Compute Engine, and GKE.

IAP establishes a central authorization layer for applications accessed by HTTPS, so you can adopt an application-level access control model instead of using network-level firewalls. When you turn on IAP, you must also use [signed headers](https://cloud.google.com/iap/docs/signed-headers-howto) or the App Engine standard environment [Users API](https://cloud.google.com/appengine/docs/standard#users) to secure your app.



[https://www.youtube.com/watch?v=XqMY-rPk3MY](https://www.youtube.com/watch?v=XqMY-rPk3MY)

#### Use IAP to ssh into internal IP VM

https://lunajacob.medium.com/utilizing-gcps-identity-aware-proxy-to-ssh-into-internal-ip-only-vm-s-237bca0123c

#### Accessing GKE via IAP

https://medium.com/google-cloud/accessing-gke-private-clusters-through-iap-14fedad694f8

#### Secure access to web apps with IAP

https://medium.com/andcloudio/secure-access-to-web-apps-with-identity-aware-proxy-14b858d9c068

#### Alternatives to IAP

https://www.strongdm.com/blog/alternatives-to-google-cloud-identity-aware-proxy-iap

#### Programmatic authentication under IAP

https://engineering.wingify.com/posts/programmatic-authentication-under-iap/

#### Serving and securing internal applications that can be accessed anywhere without the need for a VPN

https://bravenewgeek.com/tag/identity-aware-proxy/


### Device Identity

The Cloud Identity Groups API allows you to create and manage different types of devices within your organization.


https://cloud.google.com/identity/docs/concepts/overview-devices

### Groups Identity

A group is a collection of entities, where each entity can be either another group or a user. 

https://cloud.google.com/identity/docs/groups


### Access Context Manager

[Access Context Manager](https://cloud.google.com/access-context-manager/docs/overview) allows Google Cloud organization administrators to define fine-grained, attribute based access control for projects and resources in Google Cloud.

Administrators first define an access policy, which is an organization-wide container for access levels and service perimeters.

Access levels describe the necessary requirements for requests to be honored. 



### SASE

[Secure access service edge](https://www.cloudflare.com/learning/access-management/what-is-sase/), or SASE, is a cloud-based security model which bundles software-defined networking with network security functions and delivers them from a single service provider. 

SASE brings network security services and access control closer to the end user by shifting those key processes to the cloud, and operates on a global network in order to minimize latency while doing so.





### ACL


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


#### Tailscale ACL

https://tailscale.com/kb/1018/acls/
