
## Storage


### Introduction

Cloud Storage allows world-wide storage and retrieval of any amount of data at any time. You can use Cloud Storage for a range of scenarios including serving website content, storing data for archival and disaster recovery, or distributing large data objects to users via direct download.

[https://cloud.google.com/storage/docs](https://cloud.google.com/storage/docs)

What is Cloud Storage?

[https://www.youtube.com/watch?v=VDBhvexAj8I](https://www.youtube.com/watch?v=VDBhvexAj8I)

Different ways to upload your data.

[https://www.youtube.com/watch?v=nmZxfuFIP08](https://www.youtube.com/watch?v=nmZxfuFIP08)


#### GFS, Colossus

[https://en.wikipedia.org/wiki/Google_File_System](https://en.wikipedia.org/wiki/Google_File_System)


### Storage options

Compute Engine offers several types of storage options for your instances. Each of the following storage options has unique price and performance characteristics:



*   [Zonal persistent disk](https://cloud.google.com/compute/docs/disks#pdspecs): Efficient, reliable block storage.
*   [Regional persistent disk](https://cloud.google.com/compute/docs/disks#repds): Regional block storage replicated in two zones.
*   [Local SSD](https://cloud.google.com/compute/docs/disks#localssds): High performance, transient, local block storage.
*   [Cloud Storage buckets](https://cloud.google.com/compute/docs/disks#gcsbuckets): Affordable object storage.
*   [Filestore](https://cloud.google.com/filestore/docs/mounting-fileshares): High performance file storage for Google Cloud users.

[https://cloud.google.com/products/storage](https://cloud.google.com/products/storage)


#### Disk Options

[https://cloud.google.com/compute/docs/disks](https://cloud.google.com/compute/docs/disks)


#### Storage products

Overview and comparison of various Storage services and products on GCP.

[https://cloud.google.com/products/storage](https://cloud.google.com/products/storage)

Companies have a wide range of options to choose from when storing data and selecting a database in the cloud. Listen to an overview of data storage options, discuss why you would choose one over the other.

[https://www.youtube.com/watch?v=HuhTkfautDA](https://www.youtube.com/watch?v=HuhTkfautDA)


### Cloud Storage

This video walks you through how to upload a file and share it on Google Cloud Storage. 

[https://www.youtube.com/watch?v=TfOO-fSzTNA](https://www.youtube.com/watch?v=TfOO-fSzTNA)

How do  different types of buckets impact your performance? 

[https://www.youtube.com/watch?v=nCTiVwnnEhQ](https://www.youtube.com/watch?v=nCTiVwnnEhQ)


#### Storage Classes

The storage class you set for an object affects the object's availability and [pricing model](https://cloud.google.com/storage/pricing).

[https://cloud.google.com/storage/docs/storage-classes](https://cloud.google.com/storage/docs/storage-classes)


### Persistent Disk

Reliable, high-performance block storage for virtual machine instances.

[https://www.youtube.com/watch?v=zovhVfou-DI](https://www.youtube.com/watch?v=zovhVfou-DI)


### Filestore

Filestore instances are fully managed [NFS](https://en.wikipedia.org/wiki/Network_File_System) file servers on Google Cloud (GCP) for use with applications running on Compute Engine virtual machines (VMs) instances or Google Kubernetes Engine clusters.

[https://www.youtube.com/watch?v=8rS8O2RiT80](https://www.youtube.com/watch?v=8rS8O2RiT80)

You can create and manage Filestore instances by using the Google Cloud Console or the gcloud command-line tool, and interact with the NFS file share on the instance by using standard operating system commands.

[https://cloud.google.com/filestore/docs](https://cloud.google.com/filestore/docs)

### NAS, SAN, DAS, etc.

https://cloud.google.com/docs/compare/data-centers/storage

#### Backups

[https://cloud.google.com/blog/products/storage-data-transfer/introducing-filestore-backups](https://cloud.google.com/blog/products/storage-data-transfer/introducing-filestore-backups)


### Cloud Storage Connector

The [Cloud Storage](https://cloud.google.com/storage) connector is an [open source Java library](https://github.com/GoogleCloudDataproc/hadoop-connectors/tree/master/gcs) that lets you run [Apache Hadoop](https://hadoop.apache.org/) or [Apache Spark](https://spark.apache.org/) jobs directly on data in Cloud Storage, and offers a number of benefits over choosing the Hadoop Distributed File System (HDFS).

[https://cloud.google.com/dataproc/docs/concepts/connectors/cloud-storage](https://cloud.google.com/dataproc/docs/concepts/connectors/cloud-storage)

### Cloud Storage FUSE

Cloud Storage FUSE is an open source FUSE adapter that allows you to mount Cloud Storage buckets as file systems on Linux or macOS systems. It also provides a way for applications to upload and download Cloud Storage objects using standard file system semantics. Cloud Storage FUSE can be run anywhere with connectivity to Cloud Storage, including Google Compute Engine VMs or on-premises systems.

https://cloud.google.com/storage/docs/gcs-fuse

### Minio

MinIO is a High Performance Object Storage similar to s3 and GCS.

[Minio](Minio)

### Rclone

Similar to `gsutil rsync` Rclone ("rsync for cloud storage") is a command line program to sync files and directories to and from different cloud storage providers.

https://github.com/rclone/rclone
