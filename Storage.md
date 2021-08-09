[[https://blog.cartridgemonkey.com/wp-content/uploads/2012/03/Google2.jpg]]

Discuss different types of storage devices and methods.  What are block devices? What is a filesystem in the traditional sense, for example ext4 in Linux kernel?  What are networked file systems?  How do they compare to Google Cloud filesystem?  What is a SAN?  What are disk arrays, RAID, hard disk vs. SSD?

[Cloud Storage](https://cloud.google.com/storage/docs) allows world-wide storage and retrieval of any amount of data at any time. You can use Cloud Storage for a range of scenarios including serving website content, storing data for archival and disaster recovery, or distributing large data objects to users via direct download.


[What is Cloud Storage?](https://www.youtube.com/watch?v=VDBhvexAj8I)


[Different ways to upload your data.](https://www.youtube.com/watch?v=nmZxfuFIP08)



## GFS, Colossus

[The Google Filesystem](https://en.wikipedia.org/wiki/Google_File_System) Google File System (GFS or GoogleFS, not to be confused with the GFS Linux file system) is a proprietary distributed file system developed by Google to provide efficient, reliable access to data using large clusters of commodity hardware. The last version of [Google File System](https://research.google/pubs/pub51/) codenamed [Colossus](https://cloud.google.com/blog/products/storage-data-transfer/a-peek-behind-colossus-googles-file-system) was released in 2010.

In the [Big Data Chronicles](https://datafloq.com/read/big-data-history/239) and history, [the Google File System paper in 2003](https://research.google/pubs/pub51/) marked a seminal moment for software development. The Google File System paper started the Hadoop [Big Data](Big-Data) ecosystem.

<img src="https://storage.googleapis.com/gweb-cloudblog-publish/images/typical_cluster.max-2000x2000.jpg" width="500">

## Compute Engine Storage options

Compute Engine offers several types of [storage options](https://cloud.google.com/products/storage) for your instances. Each of the following storage options has unique price and performance characteristics:



*   [Zonal persistent disk](https://cloud.google.com/compute/docs/disks#pdspecs): Efficient, reliable block storage.
*   [Regional persistent disk](https://cloud.google.com/compute/docs/disks#repds): Regional block storage replicated in two zones.
*   [Local SSD](https://cloud.google.com/compute/docs/disks#localssds): High performance, transient, local block storage.
*   [Cloud Storage buckets](https://cloud.google.com/compute/docs/disks#gcsbuckets): Affordable object storage.
*   [Filestore](https://cloud.google.com/filestore/docs/mounting-fileshares): High performance file storage for Google Cloud users.

##  File Storage

File storage, also called file-level or file-based storage, is exactly what you think it might be: Data is stored as a single piece of information inside a folder, just like you’d organize pieces of paper inside a manila folder. When you need to access that piece of data, your computer needs to know the path to find it.  Data stored in files is organized and retrieved using a limited amount of metadata that tells the computer exactly where the file itself is kept. It’s like a library card catalog for data files.

Think of a closet full of file cabinets. Every document is arranged in some type of logical hierarchy—by cabinet, by drawer, by folder, then by piece of paper. This is where the term hierarchical storage comes from, and this is file storage. It is the oldest and most widely used data storage system for direct and network-attached storage systems, and it’s one that you’ve probably been using for decades. Any time you access documents saved in files on your personal computer, you use file storage. File storage has broad capabilities and can store just about anything. It’s great for storing an array of complex files and is fairly fast for users to navigate.

### NAS

Network-attached storage (NAS) is a file-level (as opposed to block-level storage) computer data storage server connected to a computer network providing data access to a heterogeneous group of clients. NAS is specialized for serving files either by its hardware, software, or configuration. It is often manufactured as a computer appliance – a purpose-built specialized computer.

### NFS

Network File System (NFS) is a distributed file system protocol originally developed by Sun Microsystems.
There are many versions: https://en.wikipedia.org/wiki/Network_File_System

### Many types of filesystems


https://en.wikipedia.org/wiki/List_of_file_systems

#### Linux Filesystems

The majority of modern Linux distributions default to the ext4 filesystem, just as previous Linux distributions defaulted to ext3, ext2, and—if you go back far enough—ext.

If you're new to Linux—or to filesystems—you might wonder what ext4 brings to the table that ext3 didn't. You might also wonder whether ext4 is still in active development at all, given the flurries of news coverage of alternate filesystems such as btrfs, xfs, and zfs.

https://opensource.com/article/18/4/ext4-filesystem

#### Flash file systems

Because of the [particular characteristics of flash memory](https://en.wikipedia.org/wiki/Flash_memory_controller), it is best used with either a controller to perform wear leveling and error correction or specifically designed flash file systems, which spread writes over the media and deal with the long erase times of NAND flash blocks. The basic concept behind flash file systems is: when the flash store is to be updated, the file system will write a new copy of the changed data over to a fresh block, remap the file pointers, then erase the old block later when it has time.

https://en.wikipedia.org/wiki/Flash_file_system


The earliest flash file system, managing an array of flash as a freely writable disk, was TrueFFS by M-Systems of Israel, presented as a software product in PC-Card Expo at Santa Clara, California, in July 1992 and patented in 1993.

Around 1994, the PCMCIA, an industry group, approved the Flash Translation Layer (FTL) specification, based on the design of M-Systems' TrueFFS. The specification was authored and jointly proposed by M-Systems and SCM Microsystems, who also provided the first working implementations of FTL.

JFFS was the first flash-specific file system for Linux, but it was quickly superseded by JFFS2, originally developed for NOR flash. Then YAFFS was released in 2002, dealing specifically with NAND flash, and JFFS2 was updated to support NAND flash too.

UBIFS has been merged since Linux 2.6.22[7] in 2008. UBIFS has been actively developed from its initial merge. UBIFS has documentation hosted at infradead.org along with JFFS2 and MTD drivers. Some initial comparison show UBIFS with compression faster than F2FS.

LogFS, another Linux flash-specific file system, is currently being developed to address the scalability issues of JFFS2.

F2FS (Flash-Friendly File System) was added to the Linux kernel 3.8.[10] Instead of being targeted at speaking directly to raw flash devices, F2FS is designed to be used on flash-based storage devices that already include a flash translation layer, such as SD cards.


## Block Storage

Block storage chops data into blocks and stores them as separate pieces. Each block of data is given a unique identifier, which allows a storage system to place the smaller pieces of data wherever is most convenient. That means that some data can be stored in a Linux® environment and some can be stored in a Windows unit.

Block storage is often configured to decouple the data from the user’s environment and spread it across multiple environments that can better serve the data. And then, when data is requested, the underlying storage software reassembles the blocks of data from these environments and presents them back to the user. It is usually deployed in storage-area network (SAN) environments and must be tied to a functioning server.

Because block storage doesn’t rely on a single path to data, it can be retrieved quickly. Each block lives on its own and can be partitioned so it can be accessed in a different operating system, which gives the user complete freedom to configure their data. It’s an efficient and reliable way to store data and is easy to use and manage. It works well with enterprises performing big transactions and those that deploy huge databases, meaning the more data you need to store, the better off you’ll be with block storage.

There are some downsides, though. Block storage can be expensive. It has limited capability to handle metadata, which means it needs to be dealt with in the application or database level—adding another thing for a developer or systems administrator to worry about.


https://www.ibm.com/cloud/learn/block-storage

### SCSI

Small Computer System Interface (SCSI, /ˈskʌzi/ SKUZ-ee)[1] is a set of standards for physically connecting and transferring data between computers and peripheral devices. The SCSI standards define commands, protocols, electrical, optical and logical interfaces. The SCSI standard defines command sets for specific peripheral device types; the presence of "unknown" as one of these types means that in theory it can be used as an interface to almost any device, but the standard is highly pragmatic and addressed toward commercial requirements. 


https://www.lifewire.com/small-computer-system-interface-scsi-2626002

### RAID

RAID (/reɪd/; "Redundant Array of Inexpensive Disks" or "Redundant Array of Independent Disks") is a data storage virtualization technology that combines multiple physical disk drive components into one or more logical units for the purposes of data redundancy, performance improvement, or both. 

https://searchstorage.techtarget.com/definition/RAID

#### Linux software RAID

https://www.thomas-krenn.com/en/wiki/Linux_Software_RAID_Information


### SSD

A solid-state drive (SSD) is a solid-state storage device that uses integrated circuit assemblies to store data persistently, typically using flash memory, and functioning as secondary storage in the hierarchy of computer storage. It is also sometimes called a solid-state device or a solid-state disk even though SSDs lack the physical spinning disks and movable read–write heads used in hard disk drives (HDDs) and floppy disks.


https://www.pcmag.com/news/ssd-vs-hdd-whats-the-difference

### SAN

A storage area network (SAN) or storage network is a computer network which provides access to consolidated, block-level data storage. SANs are primarily used to access data storage devices, such as disk arrays and tape libraries from servers so that the devices appear to the operating system as direct-attached storage. A SAN typically is a dedicated network of storage devices not accessible through the local area network (LAN).

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

LVM makes it easy to manage disk space. Especially when it comes to resizing partitions and adding another hard Drive to the system. LVM does not have redundancy built in. This means in a multi disk system if one disk fails you will have problems. LVM is only working using the automated scheme now.


https://opensource.com/business/16/9/linux-users-guide-lvm


## Object Storage

Object storage, also known as object-based storage, is a flat structure in which files are broken into pieces and spread out among hardware. In object storage, the data is broken into discrete units called objects and is kept in a single repository, instead of being kept as files in folders or as blocks on servers.

Object storage volumes work as modular units: each is a self-contained repository that owns the data, a unique identifier that allows the object to be found over a distributed system, and the metadata that describes the data. That metadata is important and includes details like age, privacies/securities, and access contingencies. Object storage metadata can also be extremely detailed, and is capable of storing information on where a video was shot, what camera was used, and what actors are featured in each frame. To retrieve the data, the storage operating system uses the metadata and identifiers, which distributes the load better and lets administrators apply policies that perform more robust searches.

Object storage requires a simple HTTP application programming interface (API), which is used by most clients in all languages. Object storage is cost efficient: you only pay for what you use. It can scale easily, making it a great choice for public cloud storage. It’s a storage system well suited for static data, and its agility and flat nature means it can scale to extremely large quantities of data. The objects have enough information for an application to find the data quickly and are good at storing unstructured data.

There are drawbacks, to be sure. Objects can’t be modified—you have to write the object completely at once. Object storage also doesn’t work well with traditional databases, because writing objects is a slow process and writing an app to use an object storage API isn’t as simple as using file storage.

https://www.netapp.com/data-storage/storagegrid/what-is-object-storage/

## Compute Engine Disk Options

Block storage resources have different performance characteristics. Consider your [storage size and performance requirements](https://cloud.google.com/compute/docs/disks) to help you determine the correct block storage type for your instances.



## Compute Engine Storage products

Overview and comparison of [various Storage services and products](https://cloud.google.com/products/storage)  on GCP.

Companies have a [wide range of options to choose from when storing data and selecting a database](https://www.youtube.com/watch?v=HuhTkfautDA) in the cloud. Listen to an overview of data storage options, discuss why you would choose one over the other.

Discuss how traditional [storage models compare to the cloud](https://cloud.google.com/compute/docs/disks) counterparts. 


## Cloud Storage

[This video walks you through](https://www.youtube.com/watch?v=TfOO-fSzTNA) how to upload a file and share it on Google Cloud Storage. 



How do  different [types of buckets impact](https://www.youtube.com/watch?v=nCTiVwnnEhQ) your performance? 

### Basic gsutil examples

https://cloud.google.com/storage/docs/working-with-big-data

### Using buckets to host a static website

https://cloud.google.com/storage/docs/hosting-static-website

https://cloud.google.com/storage/docs/static-website

### GCS Tutorials

https://cloud.google.com/architecture#/?q=cloud_storage


## Storage Classes

The [storage class](https://cloud.google.com/storage/docs/storage-classes) you set for an object affects the object's availability and [pricing model](https://cloud.google.com/storage/pricing).



## Persistent Disk

[Persistent Disks](https://cloud.google.com/persistent-disk) are reliable &  high-performance [block storage for virtual machine](https://www.youtube.com/watch?v=zovhVfou-DI) instances. Persistent Disk is designed for high durability. It stores data redundantly to ensure data integrity. Persistent disk performance scales automatically with size, so you can resize your existing persistent disks or add more persistent disks to an instance to meet your performance and storage space requirements.


## Local SSD

[Local SSDs](https://cloud.google.com/local-ssd) are physically attached to the server that hosts your VM instance. This tight coupling offers superior performance, very high input/output operations per second (IOPS), and very low latency compared to other block storage options. Local SSDs are designed for temporary storage use cases such as caches or scratch processing space. Which makes them suitable for workloads like media rendering, data analytics, or high-performance computing.

## Filestore

[Filestore](Filestore) instances are fully managed [NFS](https://en.wikipedia.org/wiki/Network_File_System) [file servers](https://www.youtube.com/watch?v=8rS8O2RiT80) on Google Cloud (GCP) for use with applications running on Compute Engine virtual machines (VMs) instances or Google Kubernetes Engine clusters.



You can create and manage [Filestore](https://cloud.google.com/filestore/docs) instances by using the Google Cloud Console or the gcloud command-line tool, and interact with the NFS file share on the instance by using standard operating system commands.




## Backups

[Filestore Backups](https://cloud.google.com/blog/products/storage-data-transfer/introducing-filestore-backups)  eases migration of file-based apps to cloud


## Cloud Storage Connector

The [Cloud Storage](https://cloud.google.com/storage) [connector](https://cloud.google.com/dataproc/docs/concepts/connectors/cloud-storage) is an [open source Java library](https://github.com/GoogleCloudDataproc/hadoop-connectors/tree/master/gcs) that lets you run [Apache Hadoop](https://hadoop.apache.org/) or [Apache Spark](https://spark.apache.org/) jobs directly on data in Cloud Storage, and offers a number of benefits over choosing the Hadoop Distributed File System (HDFS).


## Cloud Storage FUSE

[Cloud Storage FUSE](https://cloud.google.com/storage/docs/gcs-fuse) is an open source [FUSE](https://en.wikipedia.org/wiki/Filesystem_in_Userspace) adapter that allows you to mount Cloud Storage buckets as file systems on Linux or macOS systems. It also provides a way for applications to upload and download Cloud Storage objects using standard file system semantics. Cloud Storage FUSE can be run anywhere with connectivity to Cloud Storage, including Google Compute Engine VMs or on-premises systems.

## Encryption at Rest


Google uses several layers of encryption to protect customer data at rest in Google Cloud products.

Google Cloud encrypts all customer content stored at rest, without any action required from the customer, using one or more encryption mechanisms.

Data for storage is split into chunks, and each chunk is encrypted with a unique data encryption key. These data encryption keys are stored with the data, encrypted with ("wrapped" by) key encryption keys that are exclusively stored and used inside Google's central Key Management Service. Google's Key Management Service is redundant and globally distributed.

All data stored in Google Cloud is encrypted at the storage level using AES256, with the exception of a small number of Persistent Disks created before 2015 that use AES128.

Google uses a common cryptographic library, Tink, which incorporates our FIPS 140-2 validated module, BoringCrypto, to implement encryption consistently across almost all Google Cloud products. Consistent use of a common library means that only a small team of cryptographers needs to implement and maintain this tightly controlled and reviewed code.

https://cloud.google.com/security/encryption/default-encryption


## Minio

[Minio](Minio) is a High Performance Object Storage similar to s3 and GCS.


## Rclone

Similar to `gsutil rsync` [Rclone](https://github.com/rclone/rclone) ("rsync for cloud storage") is a command line program to sync files and directories to and from different cloud storage providers.

### GCS and Rclone

https://rclone.org/googlecloudstorage/

