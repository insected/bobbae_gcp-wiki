[Cloud SQL](https://cloud.google.com/sql ) is a fully managed service that makes it easy to set up, manage, and administer relational [SQL](SQL) databases: [PostgreSQL](  https://www.postgresql.org/ ), [MySQL](  https://www.mysql.com/  ), and [SQL Server](   https://wikipedia.org/wiki/Microsoft_SQL_Server ).


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

[Replication]( https://cloud.google.com/sql/docs/sqlserver/replication?hl=en   ) is the ability to create copies of a Cloud SQL instance or an on-premises database, and offload work to the copies.



https://cloud.google.com/sql/docs/mysql/replication

### Read Replicas

You use a [read replica](  https://cloud.google.com/sql/docs/mysql/replication/create-replica ) to offload work from a Cloud SQL instance. The read replica is an exact copy of the primary instance. Data and other changes on the primary instance are updated in almost real time on the read replica.

Read replicas are read-only; you cannot write to them. The read replica processes queries, read requests, and analytics traffic, thus reducing the load on the primary instance. You can have up to 10 read replicas per primary instance.

### Cross-region read replicas


[Cross-region replication](   https://cloud.google.com/sql/docs/mysql/replication#cross-region-read-replicas ) lets you create a read replica in a different region from the primary instance. You create a cross-region read replica the same way as you create an in-region replica.



### External read replicas

External [read replicas](https://cloud.google.com/sql/docs/mysql/replication#read-replicas) are external MySQL instances that replicate from a Cloud SQL primary instance. For example, a MySQL instance running on Compute Engine is considered an external instance.

https://cloud.google.com/sql/docs/mysql/replication#external-read-replicas
https://cloud.google.com/sql/docs/mysql/replication#cross-region-read-replicas





## Maintenance

https://cloud.google.com/blog/products/databases/how-cloud-sql-maintenance-works-to-keep-instances-updated

## Backups


https://cloud.google.com/sql/docs/mysql/backup-recovery/backups

## Disaster Recovery

https://cloud.google.com/architecture/intro-to-cloud-sql-disaster-recovery

## CloudSQL Insights

https://cloud.google.com/blog/products/databases/get-ahead-of-database-performance-issues-with-cloud-sql-insights

## Tutorials

https://cloud.google.com/sql/docs/media

### Migrating Postgres 

https://cloud.google.com/blog/topics/developers-practitioners/upgrade-postgres-pglogical-and-database-migration-service

### Creating alerts based on Cloud SQL logs

https://cloud.google.com/blog/products/databases/learn-how-to-create-alerts-based-on-your-database-logs-in-cloud-sql