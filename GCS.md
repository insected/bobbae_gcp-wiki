[Google Cloud Storage](https://cloud.google.com/storage/docs) allows world-wide storage and retrieval of any amount of data at any time. You can use [Cloud Storage](https://www.youtube.com/watch?v=VDBhvexAj8I) for a range of scenarios including serving website content, storing data for archival and disaster recovery, or distributing large data objects to users via direct [upload](https://www.youtube.com/watch?v=TfOO-fSzTNA) and download.

## Naming

### Bucket naming

https://cloud.google.com/storage/docs/naming-buckets

### Object naming

https://cloud.google.com/storage/docs/naming-objects

## Data encryption

Cloud Storage always [encrypts](https://cloud.google.com/storage/docs/encryption) your data on the server side, before it is written to disk, at no additional charge. 


## Storage classes

The storage class you set for an object affects the object's availability and pricing model.

https://cloud.google.com/storage/docs/storage-classes

Different [types of buckets can impact](https://www.youtube.com/watch?v=nCTiVwnnEhQ) your performance.

## Using gsutil


If you have a large number of files to upload you can use the gsutil -m option, to perform a parallel (multi-threaded/multi-processing) copy. To recursively copy subdirectories, use the -R flag of the cp command. 

https://cloud.google.com/storage/docs/working-with-big-data

## Using buckets to host a static website

You can use Cloud Storage bucket to host a static website for a domain you own.

Static web pages can contain client-side technologies such as HTML, CSS, and JavaScript. They cannot contain dynamic content such as server-side scripts like PHP.

https://cloud.google.com/storage/docs/hosting-static-website

## Composite objects

https://cloud.google.com/storage/docs/composite-objects

## Metadata

https://cloud.google.com/storage/docs/viewing-editing-metadata


## Pub/Sub notifications for GCS

https://cloud.google.com/storage/docs/pubsub-notifications

## Access control

https://cloud.google.com/storage/docs/access-control

## Access logs

https://cloud.google.com/storage/docs/access-logs

## Consistency

https://cloud.google.com/storage/docs/consistency

### Eventual consistency

https://cloud.google.com/storage/docs/consistency#eventually_consistent_operations

## GCS Tutorials

https://cloud.google.com/storage/docs/tutorials

## Storage Classes

The [storage class](https://cloud.google.com/storage/docs/storage-classes) you set for an object affects the object's availability and [pricing model](https://cloud.google.com/storage/pricing).

## Logging & Monitoring on Google Cloud Storage Buckets


https://medium.com/@snehalsb/logging-monitoring-alerting-events-on-google-cloud-storage-buckets-4952bdab5f83

## Cloud Storage Connector

The [Cloud Storage](https://cloud.google.com/storage) [connector](https://cloud.google.com/dataproc/docs/concepts/connectors/cloud-storage) is an [open source Java library](https://github.com/GoogleCloudDataproc/hadoop-connectors/tree/master/gcs) that lets you run [Apache Hadoop](https://hadoop.apache.org/) or [Apache Spark](https://spark.apache.org/) jobs directly on data in Cloud Storage, and offers a number of benefits over choosing the Hadoop Distributed File System (HDFS).


## Cloud Storage FUSE

[Cloud Storage FUSE](https://cloud.google.com/storage/docs/gcs-fuse) is an open source [Filesystem in user space](https://en.wikipedia.org/wiki/Filesystem_in_Userspace) adapter that allows you to mount Cloud Storage buckets as file systems on Linux or macOS systems. It also provides a way for applications to upload and download Cloud Storage objects using standard file system semantics. 

### Using FUSE

https://cloud.google.com/blog/products/ai-machine-learning/cloud-storage-file-system-ai-training

### s5cmd

https://blog.searce.com/improve-data-transfer-speeds-between-your-vm-and-google-cloud-storage-3567a45f6dc


## Google Storage Products


https://cloud.google.com/products/storage


## GFS, Colossus

[The Google Filesystem](https://en.wikipedia.org/wiki/Google_File_System) Google File System (GFS or GoogleFS, not to be confused with the GFS Linux file system) is a proprietary distributed file system developed by Google to provide efficient, reliable access to data using large clusters of commodity hardware. The last version of [Google File System](https://research.google/pubs/pub51/) codenamed [Colossus](https://cloud.google.com/blog/products/storage-data-transfer/a-peek-behind-colossus-googles-file-system) was released in 2010.

In the [Big Data Chronicles](https://datafloq.com/read/big-data-history/239) and history, [the Google File System paper in 2003](https://research.google/pubs/pub51/) marked a seminal moment for software development. The Google File System paper started the Hadoop [Big Data](Big-Data) ecosystem.

<!--
<img src="https://storage.googleapis.com/gweb-cloudblog-publish/images/typical_cluster.max-2000x2000.jpg" width="500">
-->

With Colossus, a single cluster is scalable to exabytes of storage and tens of thousands of machines. In the example above, for example, we have instances accessing Cloud Storage from Compute Engine VMs, YouTube serving nodes, and Ads MapReduce nodes—all of which are able to share the same underlying file system to complete requests. The key ingredient is having a shared storage pool that is managed by the Colossus control plane, providing the illusion that each has its own isolated file system. 

Disaggregation of resources drives more efficient use of valuable resources and lowers costs across all workloads. For instance, it’s possible to provision for the peak demand of low latency workloads, like a YouTube video, and then run batch analytic workloads more cheaply by having them fill in the gaps of otherwise idle time.

## Object versioning

Object Versioning retains a noncurrent object version when the live object version gets replaced or deleted. Enabling Object Versioning increases storage costs, which can be partially mitigated by configuring Object Lifecycle Management to delete older object versions.

https://cloud.google.com/storage/docs/object-versioning

## Object Lifecycle Management


You can assign a lifecycle management configuration to a bucket. The configuration contains a set of rules which apply to current and future objects in the bucket. When an object meets the criteria of one of the rules, Cloud Storage automatically performs a specified action on the object. 

https://cloud.google.com/storage/docs/lifecycle

## Retention policies and locks

Bucket Lock feature allows you to configure a data retention policy for a Cloud Storage bucket that governs how long objects in the bucket must be retained. The feature also allows you to lock the data retention policy, permanently preventing the policy from being reduced or removed.

https://cloud.google.com/storage/docs/bucket-lock


## Object holds

While an object has a hold placed on it, the object cannot be deleted or replaced.


https://cloud.google.com/storage/docs/object-holds

## CORS

https://cloud.google.com/storage/docs/cross-origin

## s3

### Minio

[Minio](Minio) is [s3](S3) compatible object storage.


### Gcloud  Storage transfers

https://cloud.google.com/blog/products/storage-data-transfer/new-gcloud-storage-enables-super-fast-data-transfers

## Use cases

### Hosting a static website

https://cloud.google.com/storage/docs/hosting-static-website

### Streaming data from Cloud Storage into BigQuery using Cloud Functions

https://cloud.google.com/architecture/streaming-data-from-cloud-storage-into-bigquery-using-cloud-functions


### Transferring data from Amazon S3 to Cloud Storage using VPC Service Controls and Storage Transfer Service


https://cloud.google.com/architecture/transferring-data-from-amazon-s3-to-cloud-storage-using-vpc-service-controls-and-storage-transfer-service


### Finding duplicate objects in GCS buckets

https://towardsdev.com/how-to-find-duplicate-objects-in-our-google-cloud-storage-gcs-buckets-6f85ac7dbdf0


### Replication using Cloud Functions
https://medium.com/@Dean_Pratt/secret-sauce-google-cloud-functions-for-autonomous-global-storage-synchronization-60d5134ff6c2


### upload files to GCS using browser JavaScript 

https://dev.to/akirakashihara/how-to-upload-files-to-google-cloud-storage-using-javascript-on-only-the-browser-11ei

