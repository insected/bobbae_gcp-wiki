
[Access Control](Access-Control) is a mechanism you can use to define who has access to resources.

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
