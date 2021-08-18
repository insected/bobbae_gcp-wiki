[Cloud SQL](https://cloud.google.com/sql ) is a fully managed service that makes it easy to set up, manage, and administer relational databases: [PostgreSQL](  https://www.postgresql.org/ ), [MySQL](  https://www.mysql.com/  ), and [SQL Server](   https://en.m.wikipedia.org/wiki/Microsoft_SQL_Server ).


## CloudSQL for MySQL

https://cloud.google.com/sql/docs/mysql

## CloudSQL for PostgreSQL

https://cloud.google.com/sql/docs/postgres

## Database Migration Service

Database Migration Service (DMS) makes it easy to migrate your production databases to Cloud SQL with minimal downtime. This serverless offering eliminates the manual hassle of provisioning, managing, and monitoring migration-specific resources. DMS leverages the native replication capabilities of MySQL and PostgreSQL to maximize the fidelity and reliability of your migration. And it’s available at no additional charge for native like-to-like migrations to Cloud SQL.

https://cloud.google.com/database-migration


## High Availability

The purpose of an HA configuration is to reduce downtime when a zone or instance becomes unavailable. This might happen during a zonal outage, or when an instance becomes corrupted. With HA, your data continues to be available to client applications.


https://cloud.google.com/sql/docs/mysql/high-availability

## Importing and exporting data


https://cloud.google.com/sql/docs/mysql/import-export

## Users & IAM

https://cloud.google.com/sql/docs/mysql/add-manage-iam-users

## Security and Access Control

https://cloud.google.com/sql/docs/mysql/authentication

## Best Practices

https://cloud.google.com/sql/docs/mysql/best-practices

## Replication

Replication is the ability to create copies of a Cloud SQL instance or an on-premises database, and offload work to the copies.

The primary reason for using replication is to scale the use of data in a database without degrading performance.


- Migrating data between regions
- Migrating data between platforms
- Migrating data from an on-premises database to Cloud SQL

Additionally, a replica could be promoted if the original instance becomes corrupted.

When referring to a Cloud SQL instance, the instance that is replicated is called the primary instance and the copies are called read replicas. The primary instance and read replicas all reside in Cloud SQL.

When referring to an on-premises database, the replication scenario is called replicating from an external server. In this scenario, the database that is replicated is the source database server. The copies that reside in Cloud SQL are called Cloud SQL replicas. There is also an instance that represents the source database server in Cloud SQL called the source representation instance.


https://cloud.google.com/sql/docs/mysql/replication

### Read Replicas

You use a read replica to offload work from a Cloud SQL instance. The read replica is an exact copy of the primary instance. Data and other changes on the primary instance are updated in almost real time on the read replica.

Read replicas are read-only; you cannot write to them. The read replica processes queries, read requests, and analytics traffic, thus reducing the load on the primary instance. You can have up to 10 read replicas per primary instance.

### Cross-region read replicas


Cross-region replication lets you create a read replica in a different region from the primary instance. You create a cross-region read replica the same way as you create an in-region replica.

https://cloud.google.com/sql/docs/mysql/replication#cross-region-read-replicas

### External read replicas

External read replicas are external MySQL instances that replicate from a Cloud SQL primary instance. For example, a MySQL instance running on Compute Engine is considered an external instance.

https://cloud.google.com/sql/docs/mysql/replication#external-read-replicas
https://cloud.google.com/sql/docs/mysql/replication#cross-region-read-replicas



https://cloud.google.com/sql/docs/mysql/replication#read-replicas


## Backups


https://cloud.google.com/sql/docs/mysql/backup-recovery/backups

## Disaster Recovery

https://cloud.google.com/architecture/intro-to-cloud-sql-disaster-recovery

