
## Types of Storage

- [Data storage](https://en.wikipedia.org/wiki/Data_storage)
- [Databases](Databases)
- [Object storage](Object-Storage)
- [File Storage](https://en.wikipedia.org/wiki/File_system)
- [Block Storage](https://en.wikipedia.org/wiki/Block-level_storage)
- [Network Attached Storage](https://en.wikipedia.org/wiki/Network-attached_storage)
- [Storage Area Network](https://en.wikipedia.org/wiki/Storage_area_network)



## Google Storage Products


https://cloud.google.com/products/storage

## Google Compute Engine Storage options

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



## Block Storage

Discuss what kinds of [block storage devices](https://www.ibm.com/cloud/learn/block-storage) you have in your computers.

### Differences between block and file storage 

https://www.atlantic.net/dedicated-server-hosting/what-is-block-storage/

### GCP Block storage resources

Block storage resources have different performance characteristics. Consider your [storage size and performance requirements](https://cloud.google.com/compute/docs/disks) to help you determine the correct block storage type for your instances.

### SCSI

Small Computer System Interface is a set of standards for physically connecting and transferring data between computers and peripheral devices. The SCSI standards define commands, protocols, electrical, optical and logical interfaces. The SCSI standard defines command sets for specific peripheral device types.


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

Redundant Array of Inexpensive Disks is a data storage virtualization technology that combines multiple physical disk drive components into one or more logical units for the purposes of data redundancy, performance improvement, or both. 

https://searchstorage.techtarget.com/definition/RAID

Discuss RAID-5 parity.

https://www.open-e.com/blog/how-does-raid-5-work/

#### Linux software RAID

https://www.thomas-krenn.com/en/wiki/Linux_Software_RAID_Information


### SSD

A solid-state drive (SSD) is a solid-state storage device that uses integrated circuit assemblies to store data persistently, typically using flash memory, and functioning as secondary storage in the hierarchy of computer storage. SSDs lack the physical spinning disks and movable read–write heads used in hard disk drives (HDDs) and floppy disks.


https://www.pcmag.com/news/ssd-vs-hdd-whats-the-difference

https://www.linux.org/threads/comparison-of-file-systems-for-an-ssd.28780/


### Linux Block devices

https://www.dell.com/support/kbdoc/en-us/000132092/ubuntu-linux-terms-for-your-hard-drive-and-devices-explained

#### /dev/sda9

/dev/ is the part in the Unix directory tree that contains all "device" files -- Unix traditionally treats just about everything you can access as a file to read from or write to.

[sd](https://man7.org/linux/man-pages/man4/sd.4.html) originally identified a SCSI device, but since the proliferation of USB (and other removable) data carriers, it became a catch-all for any block device (another Unix term; in this context, anything capable of carrying data) that wasn't already accessible via IDE. When SATA came around, the developers figured it'd be much easier and much more convenient for everyone to add it into the existing framework rather than write a whole new framework.

The letter immediately after sd signifies the order in which it was first found -- a,b,c...z, Aa...Az... etc. (Not that there are many situations in the real world where more than 26 discrete block devices are on the same bus...)

Finally, the number after that signifies the partition on the device. Note that because of the rather haphazard way PCs handle partitioning, there are only four "primary" partitions, so the numbering will be slightly off from the actual count. This isn't a terrible problem as the main purpose for the naming scheme is to have a unique and recognizable identifier for each partition found in this manner

/dev/sda9 means the ninth partition on the first drive.



#### Linux Logical Volume Manager (LVM)

LVM makes it easy to manage disk space. Especially when it comes to resizing partitions and adding another hard Drive to the system. LVM does not have redundancy built in. 

https://opensource.com/business/16/9/linux-users-guide-lvm

### GCP Persistent Disk

[Persistent Disks](https://cloud.google.com/persistent-disk) are reliable &  high-performance [block storage for virtual machine](https://www.youtube.com/watch?v=zovhVfou-DI) instances. 

https://cloud.google.com/compute/docs/disks/working-with-persistent-disks

Persistent Disk is designed for high durability. 

https://medium.com/google-cloud/persistent-disks-and-replication-9b9412fd9565

It stores data redundantly to ensure data integrity. Persistent disk performance scales automatically with size, so you can resize your existing persistent disks or add more persistent disks to an instance to meet your performance and storage space requirements.

https://cloud.google.com/compute/docs/disks/optimizing-pd-performance


### GCP Local SSD

[Local SSDs](https://cloud.google.com/local-ssd) are physically attached to the server that hosts your VM instance. This tight coupling offers superior performance, very high input/output operations per second (IOPS), and very low latency compared to other block storage options. Local SSDs are designed for temporary storage use cases such as caches or scratch processing space. Which makes them suitable for workloads like media rendering, data analytics, or high-performance computing.

## Storage Protocols

https://www.sciencedirect.com/topics/computer-science/storage-protocol


### NFS

[Network File System](NFS
) (NFS) is a distributed file system protocol originally developed by Sun Microsystems.


### NAS

[Network-attached storage](NAS
) (NAS) is a file-level (as opposed to block-level storage) computer data storage server connected to a computer network providing data access to a heterogeneous group of clients. NAS is specialized for serving files either by its hardware, software, or configuration. It is often manufactured as a computer appliance – a purpose-built specialized computer.

Google [Filestore](Filestore) uses NAS.



### NFS Appliance

https://www.netapp.com/atg/publications/publications-file-system-design-for-an-nfs-file-server-appliance-20000024/




### SAN

A storage area network (SAN) or storage network is a computer network which provides access to consolidated, block-level data storage.  A SAN typically is a dedicated network of storage devices not accessible through the local area network (LAN).

https://www.snia.org/education/storage_networking_primer/san/what_san


### Types of SAN

https://en.wikipedia.org/wiki/Storage_area_network#Network_protocols




## Object Storage

[Object storage](Object-Storage) is a flat structure in which files are broken into pieces and spread out among hardware. In object storage, the data is broken into discrete units called objects and is kept in a single repository, instead of being kept as files in folders or as blocks on servers.



### Ceph

[Ceph](Ceph) implements object, block and file storage.


## Google Compute Engine Disk Options


By default, each Compute Engine instance has a single boot persistent disk (PD) that contains the operating system. When your apps require additional storage space, you can add one or more additional storage options to your instance.


https://cloud.google.com/compute/disks-image-pricing#disk

https://cloud.google.com/compute/docs/disks

## Google Compute Engine Storage products

Overview and comparison of [various Storage services and products](https://cloud.google.com/products/storage)  on GCP.

Companies have a [wide range of options to choose from when storing data and selecting a database](https://www.youtube.com/watch?v=HuhTkfautDA) in the cloud. Listen to an overview of data storage options, discuss why you would choose one over the other.

Discuss how traditional [storage models compare to the cloud](https://cloud.google.com/compute/docs/disks) counterparts. 

## Cloud Volume

https://cloud.google.com/architecture/partners/netapp-cloud-volumes/


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

### Rclone

Similar to `gsutil rsync` [Rclone](https://github.com/rclone/rclone) ("rsync for cloud storage") is a command line program to sync files and directories to and from different cloud storage providers.


#### GCS and Rclone

https://rclone.org/googlecloudstorage/

### Case study ACME Corp

https://cloud.google.com/blog/products/storage-data-transfer/dr-in-google-cloud-with-vmware-engine-actifio-and-zerto

## Folders vs. buckets

https://www.theverge.com/platform/amp/22684730/students-file-folder-directory-structure-education-gen-z
