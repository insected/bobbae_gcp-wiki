[Filestore](https://cloud.google.com/filestore) instances are fully managed [NFS](https://en.wikipedia.org/wiki/Network_File_System) file servers on Google Cloud for use with applications running on Compute Engine virtual machines (VMs) instances or Google Kubernetes Engine clusters. Filestore  file shares can be [mounted using NFS clients](https://cloud.google.com/filestore/docs/mounting-fileshares).

## Quickstart

https://cloud.google.com/filestore/docs/quickstart-gcloud

## Backups and Monitoring

https://blog.thecloudside.com/managing-gcp-filestore-in-production-backups-monitoring-e08ffa09e7f6

## Comparison to AWS EFS

[Amazon EFS](https://docs.aws.amazon.com/efs/latest/ug/how-it-works.html) file system can be mounted through the Network File System versions 4.0 and 4.1 (NFSv4) protocol. We recommend using a current generation Linux NFSv4.1 client.

## Distributed File Systems

https://www.geeksforgeeks.org/what-is-dfsdistributed-file-system/

## Firestore Enterprise

https://cloud.google.com/blog/products/storage-data-transfer/google-cloud-announces-filestore-enterprise-for-business-critical-apps


## NetApp on Google Cloud

https://cloud.google.com/netapp

## Cloud Volumes ONTAP 

The [Cloud Volumes ONTAP HA solution](https://cloud.netapp.com/blog/gcp-cvo-blg-high-availability-architecture-on-gcp-with-cloud-volumes-ontap
) consists of a [high availability cluster](http://examcramnotes.blogspot.com/2019/08/cloud-volumes-ontap-fundamentals.html
) of two Cloud Volumes ONTAP instance groups and a mediator node, each located in a different availability zone within the same region, sharing a VPC.


## Performance

[Filestore](https://cloud.google.com/filestore) offers low latency for file operations. For workloads that are latency sensitive, like electronic design automation (EDA), media rendering, data analytics, or other metadata intensive applications, Filestore supports capacity up to 320 TB and throughput of 16 GB/s and 480K IOPS, with minimal variability in performance.


## Quickstart

https://cloud.google.com/filestore/docs/quickstart-console

## Types of Filestore

https://cloud.google.com/blog/products/storage-data-transfer/google-cloud-announces-filestore-enterprise-for-business-critical-apps