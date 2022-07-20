https://en.wikipedia.org/wiki/Computer_data_storage

## Types of Storage

- [Data storage](https://en.wikipedia.org/wiki/Data_storage)
- [Databases](Databases)
- [Object storage](Object-Storage)
- [File Storage](File-system)
- [Block Storage](https://en.wikipedia.org/wiki/Block-level_storage)
- [Network Attached Storage](NAS)
- [Storage Area Network](https://en.wikipedia.org/wiki/Storage_area_network)



## Google Cloud Storage Products


https://cloud.google.com/products/storage

## Google Cloud Compute Engine Storage options

Compute Engine offers several types of [storage options](https://cloud.google.com/products/storage) for your instances. Each of the following storage options has unique price and performance characteristics:



*   [Zonal persistent disk](https://cloud.google.com/compute/docs/disks#pdspecs): Efficient, reliable block storage.
*   [Regional persistent disk](https://cloud.google.com/compute/docs/disks#repds): Regional block storage replicated in two zones.
*   [Local SSD](https://cloud.google.com/compute/docs/disks#localssds): High performance, transient, local block storage.
*   [Cloud Storage buckets](https://cloud.google.com/compute/docs/disks#gcsbuckets): Affordable object storage.
*   [Filestore](https://cloud.google.com/filestore/docs/mounting-fileshares): High performance file storage for Google Cloud users.



### Increasing disk space of VM instance without down time

https://gridpane.com/kb/how-to-increase-the-disk-space-of-your-google-vm-instance-with-no-downtime/

## File Systems

[File System](File-System) is a hierarchical storage methodology used to organize and store data on a computer system.

## Kubernetes Storage
[Kubernetes Storage](Kubernetes-Storage) is by default not persistent per pod but there are extensive methods to provide persistent storage features.

https://www.cncf.io/blog/2020/04/28/a-complete-storage-guide-for-your-kubernetes-storage-problems/

## Block Storage

Discuss what kinds of [block storage devices](https://www.ibm.com/cloud/learn/block-storage) you have in your computers.

### Differences between block and file storage 

https://www.atlantic.net/dedicated-server-hosting/what-is-block-storage/

### GCP Block storage resources

Block storage resources have different performance characteristics. Consider your [storage size and performance requirements](https://cloud.google.com/compute/docs/disks) to help you determine the correct block storage type for your instances.

### SCSI

[Small Computer System Interface](https://en.wikipedia.org/wiki/SCSI) is a set of standards for physically connecting and transferring data between computers and peripheral devices. The SCSI standards define commands, protocols, electrical, optical and logical interfaces. The SCSI standard defines command sets for specific peripheral device types.


https://www.lifewire.com/small-computer-system-interface-scsi-2626002

#### SCSI Hard drives

https://www.servermonkey.com/blog/servers-101-hdd-interface-comparison-sata-vs-scsi-vs-sas.html

#### Disk arrays

https://en.wikipedia.org/wiki/Disk_array


### Types of Hard drives

https://ttrdatarecovery.com/types-of-hard-drives-user-guide/

### Disk scheduling

#### Elevator Algorithm

https://wikipedia.org/wiki/Elevator_algorithm

#### SCAN

https://www.geeksforgeeks.org/scan-elevator-disk-scheduling-algorithms/

#### C-SCAN

https://www.geeksforgeeks.org/c-scan-disk-scheduling-algorithm/

### RAID

[Redundant Array of Inexpensive Disks](https://en.wikipedia.org/wiki/RAID) is a data storage virtualization technology that combines multiple physical disk drive components into one or more logical units for the purposes of data redundancy, performance improvement, or both. 


Discuss RAID-5 parity.

https://www.open-e.com/blog/how-does-raid-5-work/

#### Linux software RAID

https://www.thomas-krenn.com/en/wiki/Linux_Software_RAID_Information


### SSD

A [solid-state drive](https://en.wikipedia.org/wiki/Solid-state_drive) (SSD) is a solid-state storage device that uses integrated circuit assemblies to store data persistently, typically using flash memory, and functioning as secondary storage in the hierarchy of computer storage. SSDs lack the physical spinning disks and movable read–write heads used in hard disk drives (HDDs) and floppy disks.

#### SSD vs HDD

https://www.pcmag.com/news/ssd-vs-hdd-whats-the-difference

#### Compare various Filesystems for SSD

https://www.linux.org/threads/comparison-of-file-systems-for-an-ssd.28780/


### Linux Block devices

https://www.dell.com/support/kbdoc/en-us/000132092/ubuntu-linux-terms-for-your-hard-drive-and-devices-explained

#### /dev/sda9

/dev/ is the part in the Unix directory tree that contains all "device" files -- Unix traditionally treats just about everything you can access as a file to read from or write to.

[sd](https://man7.org/linux/man-pages/man4/sd.4.html) originally identified a [SCSI](https://en.wikipedia.org/wiki/SCSI) device, but since the proliferation of [USB](https://en.wikipedia.org/wiki/USB) (and other removable) data carriers, it became a catch-all for any [block device](https://en.wikipedia.org/wiki/Device_file#BLOCKDEV) (another Unix term; in this context, anything capable of carrying data) that wasn't already accessible via [IDE](https://en.wikipedia.org/wiki/Parallel_ATA#IDE_and_ATA-1). When [SATA](https://en.wikipedia.org/wiki/Serial_ATA) came around, the developers figured it'd be much easier and much more convenient for everyone to add it into the existing framework rather than write a whole new framework.

/dev/sda9 means the ninth partition on the first drive.



#### Linux Logical Volume Manager (LVM)

[LVM](https://en.wikipedia.org/wiki/Logical_volume_management) makes it easy to manage disk space. Especially when it comes to resizing partitions and adding another hard drive to the system. LVM does not have redundancy built-in. 

https://opensource.com/business/16/9/linux-users-guide-lvm

### GCP Persistent Disk

[Persistent Disks](https://cloud.google.com/persistent-disk) are reliable and  high-performance [block storage for virtual machine](https://www.youtube.com/watch?v=zovhVfou-DI) instances. 

It stores data [redundantly](https://medium.com/google-cloud/persistent-disks-and-replication-9b9412fd9565
) to ensure data integrity. Persistent [disk performance](https://cloud.google.com/compute/docs/disks/optimizing-pd-performance
) scales automatically with size, so you can resize your existing persistent disks or add more persistent disks to an instance to meet your performance and storage [space requirements](https://cloud.google.com/compute/docs/disks/working-with-persistent-disks
).



### GCP Local SSD

[Local SSD](https://cloud.google.com/local-ssd) is physically attached to the server that hosts your VM instance. This tight coupling offers superior performance, very high input/output operations per second (IOPS), and very low latency compared to other block storage options. Local SSDs are designed for temporary storage use cases such as caches or scratch processing space. Which makes them suitable for workloads like media rendering, data analytics, or high-performance computing.


https://cloud.google.com/blog/products/storage-data-transfer/n2-vms-run-low-latency-io-intensive-workloads-with-9tb-ssd

### GCSFUSE

https://cloud.google.com/storage/docs/gcs-fuse

https://github.com/GoogleCloudPlatform/gcsfuse

## Storage Protocols

https://www.sciencedirect.com/topics/computer-science/storage-protocol


### NFS

[Network File System](NFS
) (NFS) is a distributed file system protocol originally developed by Sun Microsystems.

### Filestore

https://cloud.google.com/filestore

### NAS

[Network-attached storage](NAS
) (NAS) is a file-level (as opposed to block-level storage) computer data storage server connected to a computer network providing data access to a heterogeneous group of clients. NAS is specialized for serving files either by its hardware, software, or configuration. It is often manufactured as a computer appliance – a purpose-built specialized computer.

Google [Filestore](Filestore) uses [NAS](NAS).



### NFS Appliance

https://www.netapp.com/atg/publications/publications-file-system-design-for-an-nfs-file-server-appliance-20000024/

### WAFL
https://www.netapp.com/atg/publications/publications-file-system-design-for-an-nfs-file-server-appliance-20000024/


### SAN

A [storage area network](https://en.wikipedia.org/wiki/Storage_area_network) (SAN) or storage network is a computer network which provides access to consolidated, block-level data storage.  A SAN typically is a dedicated network of storage devices not accessible through the local area network (LAN).

https://www.snia.org/education/storage_networking_primer/san/what_san


### Types of SAN

https://en.wikipedia.org/wiki/Storage_area_network#Network_protocols




## Object Storage

[Object storage](Object-Storage) is a flat structure in which files are broken into pieces and spread out among hardware. In object storage, the data is broken into discrete units called objects and is kept in a single repository, instead of being kept as files in folders or as blocks on servers.



### Ceph

[Ceph](Ceph) implements object, block and file storage.


## Google Compute Engine Disk Options


By default, each Compute Engine instance has a single boot persistent disk (PD) that contains the operating system. When your apps require additional [storage space](https://cloud.google.com/compute/docs/disks
), you can [add one or more](https://cloud.google.com/compute/disks-image-pricing#disk
) additional storage options to your instance.




## Google Compute Engine Storage products

Overview and comparison of [various Storage services and products](https://cloud.google.com/products/storage)  on GCP.

Companies have a [wide range of options to choose from when storing data and selecting a database](https://www.youtube.com/watch?v=HuhTkfautDA) in the cloud. Listen to an overview of data storage options, discuss why you would choose one over the other.

Discuss how traditional [storage models compare to the cloud](https://cloud.google.com/compute/docs/disks) counterparts. 

## Cloud Volume

https://cloud.google.com/architecture/partners/netapp-cloud-volumes/

### Cloud Volume Service
https://cloud.netapp.com/cloud-volumes-service-for-gcp

## Security

Various [security](Security) precautions [need to be taken](https://cloud.google.com/storage/docs/gsutil/addlhelp/SecurityandPrivacyConsiderations) to protect [data security](https://cloud.google.com/blog/products/storage-data-transfer/google-cloud-storage-best-practices-to-help-ensure-data-privacy-and-security).

### Data governance

From when the data is ingested to when it can be used for valuable insights and information, management and [data governance](Data-governance) should be considered with the utmost importance for any organization.


### Encryption at Rest



Google Cloud [encrypts all customer content stored at rest](Encryption-at-Rest), without any action required from the customer, using one or more encryption mechanisms.

## Disaster Recovery and Backup

### Filestore Enterprise

https://cloud.google.com/blog/products/storage-data-transfer/google-cloud-announces-filestore-enterprise-for-business-critical-apps

### Backup for GKE

https://cloud.google.com/blog/products/storage-data-transfer/google-cloud-launches-backups-for-gke


### GCS and rsync

https://cloud.google.com/storage/docs/gsutil/commands/rsync


### Rclone

Similar to `gsutil rsync` [Rclone](https://github.com/rclone/rclone) ("rsync for cloud storage") is a command line program to sync files and directories to and from different cloud storage providers.

#### GCS and Rclone

https://rclone.org/googlecloudstorage/

#### GCS sync using Cloud Scheduler and Cloud Run

https://github.com/salrashid123/gcp_rclone


### Case study ACME Corp

https://cloud.google.com/blog/products/storage-data-transfer/dr-in-google-cloud-with-vmware-engine-actifio-and-zerto


### Secure Tertiary Data Backup (STDB)

https://cloud.google.com/blog/topics/financial-services/stdb-on-google-cloud

## Folders vs. buckets and generation gap


https://futurism.com/the-byte/gen-z-kids-file-systems

## Backblaze Storage Pods

https://www.backblaze.com/b2/storage-pod.html

