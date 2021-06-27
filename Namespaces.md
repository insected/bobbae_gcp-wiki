
[Namespaces](https://en.wikipedia.org/wiki/Linux_namespaces) are a feature of the Linux kernel that partitions kernel resources such that one set of processes sees one set of resources while another set of processes sees a different set of resources. The feature works by having the same [namespace](https://lwn.net/Articles/531114/) for a set of resources and processes, but those namespaces refer to distinct resources. Resources may exist in multiple spaces. Examples of such resources are process IDs, hostnames, user IDs, file names, and some names associated with network access, and interprocess communication.



### Linux namespaces

Namespaces are a fundamental aspect of containers on Linux.

The term "namespace" is often used for a type of namespace (e.g. process ID) as well as for a particular space of names.

A Linux system starts out with a single namespace of each type, used by all processes. Processes can create additional namespaces and join different namespaces.

[https://www.youtube.com/watch?v=kl8roLaLy-g](https://www.youtube.com/watch?v=kl8roLaLy-g)

### Network namespaces and how they are used in containers

[https://www.youtube.com/watch?v=j_UUnlVC2Ss&list=TLPQMTQxMDIwMjD4ry4yOmhx2w&index=2](https://www.youtube.com/watch?v=j_UUnlVC2Ss&list=TLPQMTQxMDIwMjD4ry4yOmhx2w&index=2)


## Kubernetes Namespaces

Kubernetes [Namespaces](https://kubernetes.io/docs/concepts/overview/working-with-objects/namespaces/) are intended for use in environments with many users spread across multiple teams, or projects. For clusters with a few to tens of users, you should not need to create or think about namespaces at all. Start using namespaces when you need the features they provide.

Namespaces provide a scope for names. Names of resources need to be unique within a namespace, but not across namespaces. Namespaces cannot be nested inside one another and each Kubernetes resource can only be in one namespace.

Kubernetes namespaces are comparable to Linux namespaces. However, Kubernetes manages namespaces in a declarative style. The simple clean-up process is central to managing operations at scale and the cluster management add-ons such as role-based access control (RBAC), making namespaces even more powerful.

## GCP Namespaces

Google Cloud supports organizing resources at the Project, Folder, and Organization levels. You can add Annotations to your Config Connector Namespaces to map resources to a Project, a Folder or Organization.

[Config Connector](https://cloud.google.com/config-connector/docs/overview) creates Google Cloud resources using Kubernetes configuration. These resources are organized in Kubernetes Namespaces.

Config Connector is a Kubernetes addon that allows you to manage Google Cloud resources through Kubernetes.

Config Connector can use the annotations on the resource's [Namespace](https://cloud.google.com/config-connector/docs/concepts/namespaces-and-projects)  to determine what project, folder, or organization to create the resources in. The Namespace's annotation will only be applied if the resource configuration does not already specify where to create the resource. 



