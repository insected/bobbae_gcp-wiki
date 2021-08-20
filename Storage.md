
Discuss different types of storage devices and methods.  What are block devices? What is a filesystem in the traditional sense, for example ext4 in Linux kernel?  What are networked file systems?  How do they compare to Google Cloud filesystem?  What is a SAN?  What are disk arrays, RAID, hard disk vs. SSD?


## Google Storage Products


https://cloud.google.com/products/storage

## Google Compute Engine Storage options

Compute Engine offers several types of [storage options](https://cloud.google.com/products/storage) for your instances. Each of the following storage options has unique price and performance characteristics:



*   [Zonal persistent disk](https://cloud.google.com/compute/docs/disks#pdspecs): Efficient, reliable block storage.
*   [Regional persistent disk](https://cloud.google.com/compute/docs/disks#repds): Regional block storage replicated in two zones.
*   [Local SSD](https://cloud.google.com/compute/docs/disks#localssds): High performance, transient, local block storage.
*   [Cloud Storage buckets](https://cloud.google.com/compute/docs/disks#gcsbuckets): Affordable object storage.
*   [Filestore](https://cloud.google.com/filestore/docs/mounting-fileshares): High performance file storage for Google Cloud users.

## Types of Storage

- Databases
- Object storage
- File Storage
- Block Storage
- Network Attached Storage
- Storage Area Network




## File Storage

Discuss filesystems you have on computers.  Windows NTFS. MacOS APFS. Linux ext4.

https://www.redhat.com/en/topics/data-storage/file-block-object-storage

## Storage Protocols

https://www.sciencedirect.com/topics/computer-science/storage-protocol


## NAS

Network-attached storage (NAS) is a file-level (as opposed to block-level storage) computer data storage server connected to a computer network providing data access to a heterogeneous group of clients. NAS is specialized for serving files either by its hardware, software, or configuration. It is often manufactured as a computer appliance – a purpose-built specialized computer.


https://www.redhat.com/en/topics/data-storage/network-attached-storage

### NFS

Network File System (NFS) is a distributed file system protocol originally developed by Sun Microsystems.

https://en.wikipedia.org/wiki/Network_File_System


### NFS Appliance

https://www.netapp.com/atg/publications/publications-file-system-design-for-an-nfs-file-server-appliance-20000024/




## Many types of filesystems


https://en.wikipedia.org/wiki/List_of_file_systems

### Linux Filesystems

The majority of modern Linux distributions default to the ext4 filesystem, just as previous Linux distributions defaulted to ext3, ext2, and—if you go back far enough—ext.

https://www.tutorialspoint.com/unix/unix-file-system.htm

If you're new to Linux—or to filesystems—you might wonder what ext4 brings to the table that ext3 didn't. 

https://opensource.com/article/18/4/ext4-filesystem

You might also wonder whether ext4 is still in active development at all, given the flurries of news coverage of alternate filesystems such as btrfs, xfs, and zfs.

https://www.salvagedata.com/btrfs-zfs-xfs-ext4-how-are-they-different/

### Elevator Algorithm

https://en.m.wikipedia.org/wiki/Elevator_algorithm

### Flash file systems

Because of the [particular characteristics of flash memory](https://en.wikipedia.org/wiki/Flash_memory_controller), it is best used with either a controller to perform wear leveling and error correction or specifically designed flash file systems, which spread writes over the media and deal with the long erase times of NAND flash blocks. 


https://en.wikipedia.org/wiki/Flash_file_system


The earliest flash file system, managing an array of flash as a freely writable disk, was TrueFFS by M-Systems of Israel, presented as a software product in PC-Card Expo at Santa Clara, California, in July 1992 and patented in 1993.



Around 1994, the PCMCIA, an industry group, approved the Flash Translation Layer (FTL) specification, based on the design of M-Systems' TrueFFS. The specification was authored and jointly proposed by M-Systems and SCM Microsystems, who also provided the first working implementations of FTL.

https://www.sciencedirect.com/topics/computer-science/flash-translation-layer

JFFS was the first flash-specific file system for Linux, but it was quickly superseded by JFFS2, originally developed for NOR flash. Then YAFFS was released in 2002, dealing specifically with NAND flash, and JFFS2 was updated to support NAND flash too.

https://www.embedded.com/flash-101-nand-flash-vs-nor-flash/

UBIFS has been merged since Linux 2.6.22[7] in 2008. UBIFS has been actively developed from its initial merge. UBIFS has documentation hosted at infradead.org along with JFFS2 and MTD drivers. Some initial comparison show UBIFS with compression faster than F2FS.

LogFS, another Linux flash-specific file system, is currently being developed to address the scalability issues of JFFS2.

F2FS (Flash-Friendly File System) was added to the Linux kernel 3.8.[10] Instead of being targeted at speaking directly to raw flash devices, F2FS is designed to be used on flash-based storage devices that already include a flash translation layer, such as SD cards.



Are these flash filesystems used on common SSD drives?

https://www.addictivetips.com/ubuntu-linux-tips/best-ssd-friendly-file-systems-on-linux/

#### TRIM

https://en.wikipedia.org/wiki/Trim_(computing)

#### NVMe


https://en.m.wikipedia.org/wiki/NVM_Express


## GCP Filestore

[Filestore](Filestore) instances are fully managed [NFS](https://en.wikipedia.org/wiki/Network_File_System) [file servers](https://www.youtube.com/watch?v=8rS8O2RiT80) on Google Cloud (GCP) for use with applications running on Compute Engine virtual machines (VMs) instances or Google Kubernetes Engine clusters.



You can create and manage [Filestore](https://cloud.google.com/filestore/docs) instances by using the Google Cloud Console or the gcloud command-line tool, and interact with the NFS file share on the instance by using standard operating system commands.




### Backups

[Filestore Backups](https://cloud.google.com/blog/products/storage-data-transfer/introducing-filestore-backups)  eases migration of file-based apps to cloud

## Block Storage

Discuss block storage devices you have in your computers.


https://www.ibm.com/cloud/learn/block-storage


### GCP Block storage resources

Block storage resources have different performance characteristics. Consider your [storage size and performance requirements](https://cloud.google.com/compute/docs/disks) to help you determine the correct block storage type for your instances.



### SCSI

Small Computer System Interface is a set of standards for physically connecting and transferring data between computers and peripheral devices. The SCSI standards define commands, protocols, electrical, optical and logical interfaces. The SCSI standard defines command sets for specific peripheral device types.


https://www.lifewire.com/small-computer-system-interface-scsi-2626002

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

### SAN

A storage area network (SAN) or storage network is a computer network which provides access to consolidated, block-level data storage.  A SAN typically is a dedicated network of storage devices not accessible through the local area network (LAN).

https://www.snia.org/education/storage_networking_primer/san/what_san


### Types of SAN

https://en.wikipedia.org/wiki/Storage_area_network#Network_protocols


### Linux Block devices

https://www.dell.com/support/kbdoc/en-us/000132092/ubuntu-linux-terms-for-your-hard-drive-and-devices-explained

#### /dev/sda9

/dev/ is the part in the Unix directory tree that contains all "device" files -- Unix traditionally treats just about everything you can access as a file to read from or write to.

sd originally identified a SCSI device, but since the proliferation of USB (and other removable) data carriers, it became a catch-all for any block device (another Unix term; in this context, anything capable of carrying data) that wasn't already accessible via IDE. When SATA came around, the developers figured it'd be much easier and much more convenient for everyone to add it into the existing framework rather than write a whole new framework.

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

## Object Storage

Object storage, also known as object-based storage, is a flat structure in which files are broken into pieces and spread out among hardware. In object storage, the data is broken into discrete units called objects and is kept in a single repository, instead of being kept as files in folders or as blocks on servers.

Object storage volumes work as modular units: each is a self-contained repository that owns the data, a unique identifier that allows the object to be found over a distributed system, and the metadata that describes the data. That metadata is important and includes details like age, privacies/securities, and access contingencies. Object storage metadata can also be extremely detailed, and is capable of storing information on where a video was shot, what camera was used, and what actors are featured in each frame. To retrieve the data, the storage operating system uses the metadata and identifiers, which distributes the load better and lets administrators apply policies that perform more robust searches.

Object storage requires a simple HTTP application programming interface (API), which is used by most clients in all languages. Object storage is cost efficient: you only pay for what you use. It can scale easily, making it a great choice for public cloud storage. It’s a storage system well suited for static data, and its agility and flat nature means it can scale to extremely large quantities of data. The objects have enough information for an application to find the data quickly and are good at storing unstructured data.

There are drawbacks, to be sure. Objects can’t be modified—you have to write the object completely at once. Object storage also doesn’t work well with traditional databases, because writing objects is a slow process and writing an app to use an object storage API isn’t as simple as using file storage.

https://www.netapp.com/data-storage/storagegrid/what-is-object-storage/

### Google Cloud Storage

[GCS](  GCS  ) is the Object storage for companies of all sizes. Store any amount of data. Retrieve it as often as you’d like.

https://cloud.google.com/storage

### AWS s3



Amazon S3 or Amazon Simple Storage Service is a service offered by Amazon Web Services (AWS) that provides object storage through a web service interface. Amazon S3 uses the same scalable storage infrastructure that Amazon.com uses to run its global e-commerce network. Amazon S3 can be employed to store any type of object, which allows for uses like storage for Internet applications, backup and recovery, disaster recovery, data archives, data lakes for analytics, and hybrid cloud storage.



#### Minio

[Minio](Minio) is a High Performance Object Storage similar to s3 and GCS.


#### b2

https://www.backblaze.com/b2/cloud-storage.html

#### s3 alternatives

https://www.coralnodes.com/amazon-s3-alternatives/


### Azure Blob Storage

Azure Blob Storage helps you create data lakes for your analytics needs, and provides storage to build powerful cloud-native and mobile apps. Optimize costs with tiered storage for your long-term data, and flexibly scale up for high-performance computing and machine learning workloads.

### IBM Cloud Object Storage

IBM Cloud Object Storage supports exponential data growth and cloud-native workloads with built-in high-speed file transfer capabilities, cross-region offerings and integrated services. The IBM [Aspera](https://www.ibm.com/cloud/object-storage/aspera) high-speed data transfer option makes it easy to transfer data, and flexible storage class tiers help manage costs while meeting data access needs.

https://www.ibm.com/cloud/object-storage


### Ceph

Ceph implements object, block and file storage.

https://ceph.io/en/discover/technology/

#### Ceph Object storage

The Ceph RGW object storage service provides  S3 API compatibility with a robust set of security, tiering, and interoperability features. 


https://docs.ceph.com/en/latest/architecture/#ceph-object-storage


#### Ceph Block storage

Ceph RBD (RADOS Block Device) block storage stripes virtual disks over objects within a Ceph storage cluster, distributing data and workload across all available devices for extreme scalability and performance. RBD disk images are [thinly provisioned](https://searchstorage.techtarget.com/definition/thin-provisioning), support both read-only snapshots and writable clones, and can be asynchronously mirrored to remote Ceph clusters in other data centers for disaster recovery or backup, making Ceph RBD the leading choice for block storage in public/private cloud and virtualization environments.

https://docs.ceph.com/en/latest/architecture/#ceph-block-device

#### Ceph File Storage



The Ceph File System (CephFS) is a robust, fully-featured POSIX-compliant distributed filesystem as a service with snapshots, quotas, and multi-cluster mirroring capabilities. CephFS files are striped across objects stored by Ceph for extreme scale and performance. Linux systems can mount CephFS filesystems natively, via a FUSE-based client, or via an NFSv4 gateway.


https://docs.ceph.com/en/latest/architecture/#ceph-file-system





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




## Encryption at Rest


Google uses several layers of encryption to protect customer data at rest in Google Cloud products.

Google Cloud encrypts all customer content stored at rest, without any action required from the customer, using one or more encryption mechanisms.

Data for storage is split into chunks, and each chunk is encrypted with a unique data encryption key. These data encryption keys are stored with the data, encrypted with ("wrapped" by) key encryption keys that are exclusively stored and used inside Google's central Key Management Service. Google's Key Management Service is redundant and globally distributed.

All data stored in Google Cloud is encrypted at the storage level using AES256, with the exception of a small number of Persistent Disks created before 2015 that use AES128.

Google uses a common cryptographic library, Tink, which incorporates our FIPS 140-2 validated module, BoringCrypto, to implement encryption consistently across almost all Google Cloud products. Consistent use of a common library means that only a small team of cryptographers needs to implement and maintain this tightly controlled and reviewed code.

https://cloud.google.com/security/encryption/default-encryption

## Rclone

Similar to `gsutil rsync` [Rclone](https://github.com/rclone/rclone) ("rsync for cloud storage") is a command line program to sync files and directories to and from different cloud storage providers.

### GCS and Rclone

https://rclone.org/googlecloudstorage/

