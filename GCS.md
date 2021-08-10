[Google Cloud Storage](https://cloud.google.com/storage/docs) allows world-wide storage and retrieval of any amount of data at any time. You can use Cloud Storage for a range of scenarios including serving website content, storing data for archival and disaster recovery, or distributing large data objects to users via direct download.

GCS is a RESTful online file storage web service for storing and accessing data on Google Cloud Platform infrastructure. The service combines the performance and scalability of Google's cloud with advanced security and sharing capabilities.

[What is Cloud Storage?](https://www.youtube.com/watch?v=VDBhvexAj8I)


[Different ways to upload your data.](https://www.youtube.com/watch?v=nmZxfuFIP08)



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



## Cloud Storage Connector

The [Cloud Storage](https://cloud.google.com/storage) [connector](https://cloud.google.com/dataproc/docs/concepts/connectors/cloud-storage) is an [open source Java library](https://github.com/GoogleCloudDataproc/hadoop-connectors/tree/master/gcs) that lets you run [Apache Hadoop](https://hadoop.apache.org/) or [Apache Spark](https://spark.apache.org/) jobs directly on data in Cloud Storage, and offers a number of benefits over choosing the Hadoop Distributed File System (HDFS).


## Cloud Storage FUSE

[Cloud Storage FUSE](https://cloud.google.com/storage/docs/gcs-fuse) is an open source [FUSE](https://en.wikipedia.org/wiki/Filesystem_in_Userspace) adapter that allows you to mount Cloud Storage buckets as file systems on Linux or macOS systems. It also provides a way for applications to upload and download Cloud Storage objects using standard file system semantics. Cloud Storage FUSE can be run anywhere with connectivity to Cloud Storage, including Google Compute Engine VMs or on-premises systems.





## Google Storage Products


https://cloud.google.com/products/storage


## GFS, Colossus

[The Google Filesystem](https://en.wikipedia.org/wiki/Google_File_System) Google File System (GFS or GoogleFS, not to be confused with the GFS Linux file system) is a proprietary distributed file system developed by Google to provide efficient, reliable access to data using large clusters of commodity hardware. The last version of [Google File System](https://research.google/pubs/pub51/) codenamed [Colossus](https://cloud.google.com/blog/products/storage-data-transfer/a-peek-behind-colossus-googles-file-system) was released in 2010.

In the [Big Data Chronicles](https://datafloq.com/read/big-data-history/239) and history, [the Google File System paper in 2003](https://research.google/pubs/pub51/) marked a seminal moment for software development. The Google File System paper started the Hadoop [Big Data](Big-Data) ecosystem.

<img src="https://storage.googleapis.com/gweb-cloudblog-publish/images/typical_cluster.max-2000x2000.jpg" width="500">

With Colossus, a single cluster is scalable to exabytes of storage and tens of thousands of machines. In the example above, for example, we have instances accessing Cloud Storage from Compute Engine VMs, YouTube serving nodes, and Ads MapReduce nodes—all of which are able to share the same underlying file system to complete requests. The key ingredient is having a shared storage pool that is managed by the Colossus control plane, providing the illusion that each has its own isolated file system. 

Disaggregation of resources drives more efficient use of valuable resources and lowers costs across all workloads. For instance, it’s possible to provision for the peak demand of low latency workloads, like a YouTube video, and then run batch analytic workloads more cheaply by having them fill in the gaps of otherwise idle time.
