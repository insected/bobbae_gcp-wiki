
[Access Control](Access-Control) is a mechanism you can use to define who has access to resources.


### Identity-Aware Proxy

[Identity-Aware Proxy](https://cloud.google.com/iap/docs) (IAP) lets you manage access to applications running in the App Engine standard environment, App Engine flexible environment, Compute Engine, and GKE.

IAP establishes a central authorization layer for applications accessed by HTTPS, so you can adopt an application-level access control model instead of using network-level firewalls. When you turn on IAP, you must also use [signed headers](https://cloud.google.com/iap/docs/signed-headers-howto) or the App Engine standard environment [Users API](https://cloud.google.com/appengine/docs/standard#users) to secure your app.


Identity Aware Proxy enables you to configure secure controlled access to your applications so you can enforce "who can see what" access control at the application layer.  You don't need client software, remote access VPNs, firewalls, network configurations. 

[https://www.youtube.com/watch?v=XqMY-rPk3MY](https://www.youtube.com/watch?v=XqMY-rPk3MY)



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


#### Tailscale

https://tailscale.com/kb/1018/acls/
