- [Migration](#migration)
  * [Introduction](#introduction)
  * [BigQuery Data Transfer Service](#bigquery-data-transfer-service)
  * [Migrate for Compute Engine](#migrate-for-compute-engine)
    + [Velostrata](#velostrata)
    + [How to move thousands of VMs to GCP](#how-to-move-thousands-of-vms-to-gcp)
  * [Cloud Storage Transfer Service](#cloud-storage-transfer-service)
  * [Migrate for Anthos](#migrate-for-anthos)
    + [Migrating enterprise workloads using Migrate for Anthos](#migrating-enterprise-workloads-using-migrate-for-anthos)
  * [Transfer Appliance](#transfer-appliance)
  * [Cloud Data Transfer](#cloud-data-transfer)
  * [Storage Transfer Service](#storage-transfer-service)
  * [Database Migration Service](#database-migration-service)
  * [All Google Cloud Migration Guides](#all-google-cloud-migration-guides)
  * [Big Data Transfer over WAN](#big-data-transfer-over-wan)
  * [Netapp](#netapp)
    + [Trident](#trident)
    + [Cloud Volumes Service](#cloud-volumes-service)
  * [AWS to GCP Data migration](#aws-to-gcp-data-migration)

<small><i><a href='http://ecotrust-canada.github.io/markdown-toc/'>Table of contents generated with markdown-toc</a></i></small>


## Migration


### Introduction

A video on Cloud Migration.

[https://www.youtube.com/watch?v=Bt_cWJrdfS8](https://www.youtube.com/watch?v=Bt_cWJrdfS8)

[https://cloud.google.com/solutions/migration-to-gcp-getting-started](https://cloud.google.com/solutions/migration-to-gcp-getting-started)


### BigQuery Data Transfer Service

The BigQuery Data Transfer Service automates data movement into BigQuery on a scheduled, managed basis. Your analytics team can lay the foundation for a BigQuery data warehouse without writing a single line of code.

[https://cloud.google.com/bigquery-transfer/docs/transfer-service-overview](https://cloud.google.com/bigquery-transfer/docs/transfer-service-overview)


### Migrate for Compute Engine

Google Cloud Migrate for Compute Engine (formerly Velostrata) migrates VMs from your on-premises data center, AWS, or Azure into Compute Engine.

[https://cloud.google.com/migrate/compute-engine/docs](https://cloud.google.com/migrate/compute-engine/docs)

#### General VM Migration issues
Compute Engine enables [Live Migration](https://cloudplatform.googleblog.com/2015/03/Google-Compute-Engine-uses-Live-Migration-technology-to-service-infrastructure-without-application-downtime.html) which can allow your instances migrated automatically when the physical hardware requires maintenance.

As with standard hypervisor suites, Compute Engine also allows you to take live snapshots of VM instances. You can use these snapshots to create new instances within a zone or move an instance to a different zone.

If your Compute Engine VM instance is terminated due to issues with the underlying physical host, the instance will recover automatically on a different host within the same zone. You can also elect to have your machines stay down by turning off automatic restart.


#### Velostrata

Velostrata gets enterprise applications running in Google Cloud within minutes, while data migrates transparently in the background. With Velostrata, enterprises can validate, run, and migrate applications into Google Cloud without rewriting them, modifying the image, or changing management processes.

[https://cloud.google.com/blog/products/velostrata](https://cloud.google.com/blog/products/velostrata)


#### How to move thousands of VMs to GCP

[https://www.youtube.com/watch?v=WD454APAPV8](https://www.youtube.com/watch?v=WD454APAPV8)


### Cloud Storage Transfer Service

Storage Transfer Service allows you to quickly import online data into Cloud Storage. You can also set up a repeating schedule for transferring data, as well as transfer data within Cloud Storage, from one bucket to another.

[https://cloud.google.com/storage-transfer/docs](https://cloud.google.com/storage-transfer/docs)


### Migrate for Anthos

With Migrate for Anthos, you can migrate your VMs from [supported source platforms](https://cloud.google.com/migrate/anthos/docs/migration-prerequisites) to Google Kubernetes Engine or [Anthos](https://cloud.google.com/anthos).

[https://cloud.google.com/migrate/anthos/docs/getting-started](https://cloud.google.com/migrate/anthos/docs/getting-started)


#### Migrating enterprise workloads using Migrate for Anthos

[https://www.youtube.com/watch?v=8Q1kqWVbKQY](https://www.youtube.com/watch?v=8Q1kqWVbKQY)


### Transfer Appliance

Transfer Appliance is a hardware appliance you can use to securely migrate large volumes of data (from hundreds of terabytes up to 1 petabyte) to Google Cloud Platform without disrupting business operations.

[https://cloud.google.com/transfer-appliance/docs/2.0](https://cloud.google.com/transfer-appliance/docs/2.0)


### Cloud Data Transfer

There are many different ways to transfer data in GCP: Online Transfer, Transfer Service, Transfer Appliance, BigQuery Data Transfer Service and Offline Transfer Methods.

[https://cloud.google.com/products/data-transfer](https://cloud.google.com/products/data-transfer)


### Storage Transfer Service

Whether you're coming from an online or on-premises source, our online storage transfer solutions enable you to manage large-scale data transfers easily, securely, and efficiently. Storage Transfer Service and Transfer Service for on-premises data offer two highly performant pathways to Cloud Storage—both with the scalability and speed you need to simplify the data transfer process.

[https://cloud.google.com/storage-transfer-service](https://cloud.google.com/storage-transfer-service)


### Database Migration Service

[https://cloud.google.com/database-migration](https://cloud.google.com/database-migration)

[https://cloud.google.com/blog/products/databases/database-migration-service-now-available-for-cloud-sql-and-more](https://cloud.google.com/blog/products/databases/database-migration-service-now-available-for-cloud-sql-and-more)


### All Google Cloud Migration Guides

[https://cloud.google.com/blog/products/cloud-migration/guide-to-all-google-cloud-migration-guides](https://cloud.google.com/blog/products/cloud-migration/guide-to-all-google-cloud-migration-guides)


### Big Data Transfer over WAN

[https://asperasoft.com/fileadmin/media/Asperasoft.com/Product_Briefs/Google_AoD_AsperaPB.pdf](https://asperasoft.com/fileadmin/media/Asperasoft.com/Product_Briefs/Google_AoD_AsperaPB.pdf)


### Netapp

[https://cloud.google.com/netapp](https://cloud.google.com/netapp)


#### Trident

[https://github.com/NetApp/trident](https://github.com/NetApp/trident)


#### Cloud Volumes Service 

[https://cloud.netapp.com/cloud-volumes-service-for-gcp](https://cloud.netapp.com/cloud-volumes-service-for-gcp)


### AWS to GCP Data migration

[https://cloud.google.com/migrate/compute-engine/docs/4.2/how-to/migrate-aws-to-gcp/overview](https://cloud.google.com/migrate/compute-engine/docs/4.2/how-to/migrate-aws-to-gcp/overview)
