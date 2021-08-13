



<img src="https://cloudx-bricks-prod-bucket.storage.googleapis.com/138633884648c8406920f543d8dfce83fc0b78fff0a3130c68ec528ae5df84aa.svg" width="800">

### Introduction



Migrate for Compute Engine enables you to migrate (Lift and Shift) your virtual machines (VMs), with minor automatic modifications, from your source environment to Google Compute Engine. Migrate for Compute Engine uses data replication technology which continuously replicates disk data from the source VMs to Google Cloud without causing any downtime on the source. You then create VM clones from replicated data for testing and perform predictable VM cut-over to your final workloads running on Google Cloud.

Data replication allows Migrate for Compute Engine to perform an initial replication of the data from the source VM so that you can quickly clone and test a migrated VM. However, because the source VM continues to run during the migration process, including during testing, Migrate for Compute Engine continues to replicate data until you perform the final cut over to your migrated VM.

https://cloud.google.com/migrate/compute-engine/docs/5.0/concepts/lifecycle

A video on Cloud Migration.

[https://www.youtube.com/watch?v=Bt_cWJrdfS8](https://www.youtube.com/watch?v=Bt_cWJrdfS8)

[https://cloud.google.com/solutions/migration-to-gcp-getting-started](https://cloud.google.com/solutions/migration-to-gcp-getting-started)




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
### Migration from AWS to GCP



https://cloud.google.com/migrate/compute-engine/docs/4.2/how-to/migrate-aws-to-gcp/overview

### Migration from VMWare to GCP

https://cloud.google.com/migrate/compute-engine/docs/4.2/how-to/configure-manager/configuring-vms-vm



### BigQuery Data Transfer Service

The BigQuery Data Transfer Service automates data movement into BigQuery on a scheduled, managed basis. Your analytics team can lay the foundation for a BigQuery data warehouse without writing a single line of code.

[https://cloud.google.com/bigquery-transfer/docs/transfer-service-overview](https://cloud.google.com/bigquery-transfer/docs/transfer-service-overview)


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

Database Migration Service makes it easier for you to migrate your data to Google Cloud. This service helps you lift and shift your MySQL and PostgreSQL workloads into Cloud SQL.

Database Migration Service streamlines networking workflows, manages the initial snapshot and ongoing replication, and provides a status of the migration operations.

[https://cloud.google.com/database-migration](https://cloud.google.com/database-migration)

[https://cloud.google.com/blog/products/databases/database-migration-service-now-available-for-cloud-sql-and-more](https://cloud.google.com/blog/products/databases/database-migration-service-now-available-for-cloud-sql-and-more)


### All Google Cloud Migration Guides

[https://cloud.google.com/blog/products/cloud-migration/guide-to-all-google-cloud-migration-guides](https://cloud.google.com/blog/products/cloud-migration/guide-to-all-google-cloud-migration-guides)


### Big Data Transfer over WAN

[https://asperasoft.com/fileadmin/media/Asperasoft.com/Product_Briefs/Google_AoD_AsperaPB.pdf](https://asperasoft.com/fileadmin/media/Asperasoft.com/Product_Briefs/Google_AoD_AsperaPB.pdf)


### Netapp

[https://cloud.google.com/netapp](https://cloud.google.com/netapp)


#### Trident

Trident is a fully supported open source project maintained by NetApp. It has been designed from the ground up to help you meet your containerized applications' persistence demands using industry-standard interfaces, such as the Container Storage Interface (CSI).

[https://github.com/NetApp/trident](https://github.com/NetApp/trident)


#### Cloud Volumes Service 

Cloud Volumes Service removes obstacles so you can move more of your file-based apps to Google Cloud, with support for Network File System (NFSv3 and NFSv4.1) and Server Message Block (SMB) volumes. You don't have to re-architect your apps, and you get persistent storage for your apps without complexity.

[https://cloud.netapp.com/cloud-volumes-service-for-gcp](https://cloud.netapp.com/cloud-volumes-service-for-gcp)


### AWS to GCP Data migration

This overview outlines the general steps required for migrating VMs from AWS EC2 to Google Cloud using Velostrata.

https://cloud.google.com/migrate/compute-engine/docs/4.2/how-to/migrate-aws-to-gcp/overview

