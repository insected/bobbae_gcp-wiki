
Namespaces are a feature of the Linux kernel that partitions kernel resources such that one set of processes sees one set of resources while another set of processes sees a different set of resources. The feature works by having the same namespace for a set of resources and processes, but those namespaces refer to distinct resources. Resources may exist in multiple spaces. Examples of such resources are process IDs, hostnames, user IDs, file names, and some names associated with network access, and interprocess communication.



### Linux namespaces

Namespaces are a fundamental aspect of containers on Linux.

The term "namespace" is often used for a type of namespace (e.g. process ID) as well as for a particular space of names.

A Linux system starts out with a single namespace of each type, used by all processes. Processes can create additional namespaces and join different namespaces.

[https://www.youtube.com/watch?v=kl8roLaLy-g](https://www.youtube.com/watch?v=kl8roLaLy-g)

### Network namespaces and how they are used in containers

[https://www.youtube.com/watch?v=j_UUnlVC2Ss&list=TLPQMTQxMDIwMjD4ry4yOmhx2w&index=2](https://www.youtube.com/watch?v=j_UUnlVC2Ss&list=TLPQMTQxMDIwMjD4ry4yOmhx2w&index=2)


