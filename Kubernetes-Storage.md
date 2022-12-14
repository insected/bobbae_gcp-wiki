

Kubernetes containers are stateless as a core principle, but data must still be managed, preserved, and made accessible to other services. 


https://kubernetes.io/docs/tutorials/stateless-application/

Stateless means that the container is running in isolation without any knowledge of past transactions, which makes it easy to replace, delete, or distribute the container. However, it also means that data will be lost for certain lifecycle events like restart or deletion.

## StatefulSets

https://kubernetes.io/docs/tutorials/stateful-application/basic-stateful-set/

### Deploying Cassandra as a StatefulSet

https://kubernetes.io/docs/tutorials/stateful-application/cassandra/

### Multi Datacenter Cassandra clusters using K8ssandra 

https://medium.com/building-the-open-data-stack/set-up-multi-datacenter-cassandra-clusters-in-gke-with-k8ssandra-and-cloud-dns-5cb389b1e776

### Running Zookeeper

https://kubernetes.io/docs/tutorials/stateful-application/zookeeper/

## Kubernetes Storage Classes

[https://www.youtube.com/watch?v=qktFhjJmFhg](https://www.youtube.com/watch?v=qktFhjJmFhg)





A [StorageClass](https://kubernetes.io/docs/concepts/storage/storage-classes/) provides a way for administrators to describe the "classes" of storage they offer. Different classes might map to quality-of-service levels, or to backup policies, or to arbitrary policies determined by the cluster administrators. Kubernetes itself is unopinionated about what classes represent. This concept is sometimes called "profiles" in other storage systems.

Each StorageClass contains the fields provisioner, parameters, and reclaimPolicy, which are used when a PersistentVolume belonging to the class needs to be dynamically provisioned.

The name of a StorageClass object is significant, and is how users can request a particular class. Administrators set the name and other parameters of a class when first creating StorageClass objects, and the objects cannot be updated once they are created.

Administrators can specify a default StorageClass only for PVCs that don't request any particular class to bind to: see the [PersistentVolumeClaim](https://kubernetes.io/docs/concepts/storage/persistent-volumes/#persistentvolumeclaims) for details.

https://kubernetes.io/docs/concepts/storage/storage-classes/




## Storage Provisioners

https://kubernetes.io/docs/concepts/storage/storage-classes/#provisioner


## Kubernetes Block Storage Solutions

### GCE PD

https://kubernetes.io/docs/concepts/storage/storage-classes/#gce-pd

### AWS EBS

https://kubernetes.io/docs/concepts/storage/storage-classes/#aws-ebs

### Azure Disk

https://kubernetes.io/docs/concepts/storage/storage-classes/#azure-disk

### ceph and Rook

[Rook](https://rook.io/
) is a storage orchestration tool that provides a cloud-native, open source solution for a diverse set of storage providers. Rook uses the power of Kubernetes to turn a storage system into self-managing services that provide a seamless experience for saving Kubernetes application or deployment data. Rook can use [NFS](NFS), [Cassandra](https://cassandra.apache.org/_/index.html) or [Ceph](Ceph).


[Ceph](Ceph) is a highly scalable distributed-storage solution offering object, block, and file storage. Ceph clusters are designed to run on any hardware using the so-called CRUSH algorithm (Controlled Replication Under Scalable Hashing).

https://www.digitalocean.com/community/tutorials/how-to-set-up-a-ceph-cluster-within-kubernetes-using-rook

### Block Devices 

You may use Ceph Block Device images with Kubernetes v1.13 and later through ceph-csi, which dynamically provisions RBD images to back Kubernetes volumes and maps these RBD images as block devices (optionally mounting a file system contained within the image) on worker nodes running pods that reference an RBD-backed volume. Ceph stripes block device images as objects across the cluster, which means that large Ceph Block Device images have better performance than a standalone server.

https://docs.ceph.com/en/latest/rbd/rbd-kubernetes/

### Longhorn

Cloud native distributed block storage for Kubernetes by [Rancher](https://rancher.com/).

https://longhorn.io/

### Linstor

[LINSTOR](https://linbit.com/linstor/
) has a container storage interface (CSI) driver for Kubernetes and is compatible with OpenShift. LINSTOR can also be used independently of a cloud, virtualization, or container platform to manage large [DRBD](https://linbit.com/drbd/) clusters. 

DRBD????? software is a distributed replicated storage system for the Linux platform. It is implemented as a kernel driver, several userspace management applications, and some shell scripts. 

DRBD is traditionally used in high availability (HA) computer clusters, but beginning with DRBD version 9, it can also be used to create larger software defined storage pools with a focus on cloud integration.


### OpenEBS


[OpenEBS](https://openebs.io/
) builds on Kubernetes to enable Stateful applications to easily access Dynamic Local PVs or Replicated PVs. By using the [Container Attached Storage pattern](https://docs.openebs.io/docs/next/k8s-storage.html
) users report lower costs, easier management, and more control for their teams.


https://docs.openebs.io/


### Robin

https://robin.io/

### Portworx

https://portworx.com/

### StorageOS

https://storageos.com/

### Zenko

https://www.zenko.io/

## Kubernetes Storage Solutions Comparisons

https://vitobotta.com/2019/08/06/kubernetes-storage-openebs-rook-longhorn-storageos-robin-portworx/

### Performance comparisons

https://medium.com/volterra-io/kubernetes-storage-performance-comparison-v2-2020-updated-1c0b69f0dcf4

## Volumes

On-disk files in a container are ephemeral, which presents some problems for non-trivial applications when running in containers. One problem is the loss of files when a container crashes. The [kubelet](https://kubernetes.io/docs/reference/command-line-tools-reference/kubelet/) restarts the container but with a clean state. A second problem occurs when sharing files between containers running together in a Pod. 

Docker has a concept of [volumes](https://docs.docker.com/storage/volumes/), though it is somewhat looser and less managed. A Docker volume is a directory on disk or in another container. Docker provides volume drivers, but the functionality is somewhat limited.

Kubernetes supports many types of [volumes](https://kubernetes.io/docs/concepts/storage/volumes/
). A Pod can use any number of volume types simultaneously. Ephemeral volume types have a lifetime of a pod, but persistent volumes exist beyond the lifetime of a pod. When a pod ceases to exist, Kubernetes destroys ephemeral volumes; however, Kubernetes does not destroy persistent volumes. For any kind of volume in a given pod, data is preserved across container restarts.

At its core, a volume is a directory, possibly with some data in it, which is accessible to the containers in a pod. How that directory comes to be, the medium that backs it, and the contents of it are determined by the particular volume type used.




### CSI

[Container Storage Interface](https://kubernetes.io/docs/concepts/storage/volumes/#csi
) (CSI) defines a standard interface for container orchestration systems (like Kubernetes) to expose arbitrary storage systems to their container workloads.



### PVC Persistent Volume Claim

https://kubernetes.io/docs/concepts/storage/persistent-volumes/

### Volume Mode


https://kubernetes.io/docs/concepts/storage/persistent-volumes/#volume-mode

Discuss the block or filesystem providers mapped to Volume which uses filesystem volume mode. Volume is block level concept. What does it mean to have volume type of filesystem?  Some block providers can be used for raw block volumes.  



### Raw Block Volume

https://kubernetes.io/docs/concepts/storage/persistent-volumes/#raw-block-volume-support


### PV Access Modes

https://kubernetes.io/docs/concepts/storage/persistent-volumes/#access-modes

### Dynamic Volume Provisioning

[Dynamic volume provisioning](https://kubernetes.io/docs/concepts/storage/dynamic-provisioning/
) allows storage volumes to be created on-demand. Without dynamic provisioning, cluster administrators have to manually make calls to their cloud or storage provider to create new storage volumes, and then create PersistentVolume objects to represent them in Kubernetes. The dynamic provisioning feature eliminates the need for cluster administrators to pre-provision storage. Instead, it automatically provisions storage when it is requested by users.





### Volume snapshots

https://kubernetes.io/docs/concepts/storage/volume-snapshots/

### CSI Volume cloning

https://kubernetes.io/docs/concepts/storage/volume-pvc-datasource/

### CSI GCS

https://github.com/ofek/csi-gcs

### Dynamic Volume Provisioning

https://kubernetes.io/docs/concepts/storage/dynamic-provisioning/

### Ephemeral Volumes

https://kubernetes.io/docs/concepts/storage/ephemeral-volumes/

### Volume Health Monitoring

https://kubernetes.io/docs/concepts/storage/volume-health-monitoring/

## FlexVolume

### Kubernetes Definition

[FlexVolume](https://github.com/kubernetes/community/blob/master/contributors/devel/sig-storage/flexvolume.md
) is an out-of-tree plugin interface that has existed in Kubernetes since version 1.2 (before CSI). It uses an exec-based model to interface with drivers. The [FlexVolume](https://kubernetes.io/docs/concepts/storage/volumes/#flexvolume
) driver binaries must be installed in a pre-defined volume plugin path on each node and in some cases the control plane nodes as well.

https://github.com/kubernetes/examples/tree/master/staging/volumes/flexvolume

### NetApp

https://library.netapp.com/ecmdocs/ECMP1368017/html/GUID-4DF6A167-6C98-4E48-8F5C-41E73A506139.html


## Databases


https://cloud.google.com/blog/products/databases/to-run-or-not-to-run-a-database-on-kubernetes-what-to-consider


### k8ssandra

https://k8ssandra.io/


### PostgreSQL




https://github.com/CrunchyData/postgres-operator


### Mongodb Atlas

https://github.com/mongodb/mongodb-atlas-kubernetes


### redis

https://github.com/ot-container-kit/redis-operator


### CockroachDB


https://www.cockroachlabs.com/product/kubernetes/



