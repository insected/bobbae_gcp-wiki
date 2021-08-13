

Kubernetes containers are stateless as a core principle, but data must still be managed, preserved, and made accessible to other services. 


https://kubernetes.io/docs/tutorials/stateless-application/

Stateless means that the container is running in isolation without any knowledge of past transactions, which makes it easy to replace, delete, or distribute the container. However, it also means that data will be lost for certain lifecycle events like restart or deletion.

## StatefulSets

https://kubernetes.io/docs/tutorials/stateful-application/basic-stateful-set/



## Kubernetes Storage Classes

[https://www.youtube.com/watch?v=qktFhjJmFhg](https://www.youtube.com/watch?v=qktFhjJmFhg)





A [StorageClass](https://kubernetes.io/docs/concepts/storage/storage-classes/) provides a way for administrators to describe the "classes" of storage they offer. Different classes might map to quality-of-service levels, or to backup policies, or to arbitrary policies determined by the cluster administrators. Kubernetes itself is unopinionated about what classes represent. This concept is sometimes called "profiles" in other storage systems.

https://kubernetes.io/docs/concepts/storage/storage-classes/


### Storage Provisioners

https://kubernetes.io/docs/concepts/storage/storage-classes/#provisioner

### ceph and Rook

Rook is a storage orchestration tool that provides a cloud-native, open source solution for a diverse set of storage providers. Rook uses the power of Kubernetes to turn a storage system into self-managing services that provide a seamless experience for saving Kubernetes application or deployment data.

Ceph is a highly scalable distributed-storage solution offering object, block, and file storage. Ceph clusters are designed to run on any hardware using the so-called CRUSH algorithm (Controlled Replication Under Scalable Hashing).

https://www.digitalocean.com/community/tutorials/how-to-set-up-a-ceph-cluster-within-kubernetes-using-rook

### Block Devices 

You may use Ceph Block Device images with Kubernetes v1.13 and later through ceph-csi, which dynamically provisions RBD images to back Kubernetes volumes and maps these RBD images as block devices (optionally mounting a file system contained within the image) on worker nodes running pods that reference an RBD-backed volume. Ceph stripes block device images as objects across the cluster, which means that large Ceph Block Device images have better performance than a standalone server.

https://docs.ceph.com/en/latest/rbd/rbd-kubernetes/

### Volumes

On-disk files in a container are ephemeral, which presents some problems for non-trivial applications when running in containers. One problem is the loss of files when a container crashes. The kubelet restarts the container but with a clean state. A second problem occurs when sharing files between containers running together in a Pod. 

Docker has a concept of volumes, though it is somewhat looser and less managed. A Docker volume is a directory on disk or in another container. Docker provides volume drivers, but the functionality is somewhat limited.

Kubernetes supports many types of volumes. A Pod can use any number of volume types simultaneously. Ephemeral volume types have a lifetime of a pod, but persistent volumes exist beyond the lifetime of a pod. When a pod ceases to exist, Kubernetes destroys ephemeral volumes; however, Kubernetes does not destroy persistent volumes. For any kind of volume in a given pod, data is preserved across container restarts.

At its core, a volume is a directory, possibly with some data in it, which is accessible to the containers in a pod. How that directory comes to be, the medium that backs it, and the contents of it are determined by the particular volume type used.


https://kubernetes.io/docs/concepts/storage/volumes/

### Snapshots

In Kubernetes, a VolumeSnapshot represents a snapshot of a volume on a storage system. This document assumes that you are already familiar with Kubernetes persistent volumes.


https://kubernetes.io/docs/concepts/storage/volume-snapshots/

### Dynamic Volume Provisioning

Dynamic volume provisioning allows storage volumes to be created on-demand. Without dynamic provisioning, cluster administrators have to manually make calls to their cloud or storage provider to create new storage volumes, and then create PersistentVolume objects to represent them in Kubernetes. The dynamic provisioning feature eliminates the need for cluster administrators to pre-provision storage. Instead, it automatically provisions storage when it is requested by users.


https://kubernetes.io/docs/concepts/storage/dynamic-provisioning/

### CSI

Container Storage Interface (CSI) defines a standard interface for container orchestration systems (like Kubernetes) to expose arbitrary storage systems to their container workloads.


https://kubernetes.io/docs/concepts/storage/volumes/#csi

### PVC Persistent Volume Claim

https://kubernetes.io/docs/concepts/storage/persistent-volumes/


### Volume snapshots

https://kubernetes.io/docs/concepts/storage/volume-snapshots/

### CSI Volume cloning

https://kubernetes.io/docs/concepts/storage/volume-pvc-datasource/

### Dynamic Volume Provisioning

https://kubernetes.io/docs/concepts/storage/dynamic-provisioning/

### Ephemeral Volumes

https://kubernetes.io/docs/concepts/storage/ephemeral-volumes/

### Volume Health Monitoring

https://kubernetes.io/docs/concepts/storage/volume-health-monitoring/


