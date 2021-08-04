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

[Cloud Storage FUSE](https://cloud.google.com/storage/docs/gcs-fuse) is an open source FUSE adapter that allows you to mount Cloud Storage buckets as file systems on Linux or macOS systems. It also provides a way for applications to upload and download Cloud Storage objects using standard file system semantics. Cloud Storage FUSE can be run anywhere with connectivity to Cloud Storage, including Google Compute Engine VMs or on-premises systems.



## Minio

[Minio](Minio) is a High Performance Object Storage similar to s3 and GCS.


## Rclone

Similar to `gsutil rsync` [Rclone](https://github.com/rclone/rclone) ("rsync for cloud storage") is a command line program to sync files and directories to and from different cloud storage providers.


