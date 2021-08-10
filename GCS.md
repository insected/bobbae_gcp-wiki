[Cloud Storage](https://cloud.google.com/storage/docs) allows world-wide storage and retrieval of any amount of data at any time. You can use Cloud Storage for a range of scenarios including serving website content, storing data for archival and disaster recovery, or distributing large data objects to users via direct download.


[What is Cloud Storage?](https://www.youtube.com/watch?v=VDBhvexAj8I)


[Different ways to upload your data.](https://www.youtube.com/watch?v=nmZxfuFIP08)

## Google Storage Products


https://cloud.google.com/products/storage


## GFS, Colossus

[The Google Filesystem](https://en.wikipedia.org/wiki/Google_File_System) Google File System (GFS or GoogleFS, not to be confused with the GFS Linux file system) is a proprietary distributed file system developed by Google to provide efficient, reliable access to data using large clusters of commodity hardware. The last version of [Google File System](https://research.google/pubs/pub51/) codenamed [Colossus](https://cloud.google.com/blog/products/storage-data-transfer/a-peek-behind-colossus-googles-file-system) was released in 2010.

In the [Big Data Chronicles](https://datafloq.com/read/big-data-history/239) and history, [the Google File System paper in 2003](https://research.google/pubs/pub51/) marked a seminal moment for software development. The Google File System paper started the Hadoop [Big Data](Big-Data) ecosystem.

<img src="https://storage.googleapis.com/gweb-cloudblog-publish/images/typical_cluster.max-2000x2000.jpg" width="500">

With Colossus, a single cluster is scalable to exabytes of storage and tens of thousands of machines. In the example above, for example, we have instances accessing Cloud Storage from Compute Engine VMs, YouTube serving nodes, and Ads MapReduce nodes—all of which are able to share the same underlying file system to complete requests. The key ingredient is having a shared storage pool that is managed by the Colossus control plane, providing the illusion that each has its own isolated file system. 

Disaggregation of resources drives more efficient use of valuable resources and lowers costs across all workloads. For instance, it’s possible to provision for the peak demand of low latency workloads, like a YouTube video, and then run batch analytic workloads more cheaply by having them fill in the gaps of otherwise idle time.
