[Cloud SQL](https://cloud.google.com/sql ) is a fully managed service that makes it easy to set up, manage, and administer relational [SQL](SQL) databases: [PostgreSQL](  https://www.postgresql.org/ ), [MySQL](  https://www.mysql.com/  ), and [SQL Server](   https://wikipedia.org/wiki/Microsoft_SQL_Server ).


### CloudSQL for MySQL

https://cloud.google.com/sql/docs/mysql

### CloudSQL for PostgreSQL

https://cloud.google.com/sql/docs/postgres

### SQL server performance analysis and query tuning
https://cloud.google.com/blog/products/databases/sql-server-performance-analysis-and-query-tuning


### SQL Server

https://medium.com/google-cloud/going-cloud-with-sql-server-google-cloud-options-6cd44bb52bef

#### SQL Server database auditing
https://cloud.google.com/sql/docs/sqlserver/db-audit
### AlloyDB

https://cloud.google.com/blog/products/databases/alloydb-for-postgresql-intelligent-scalable-storage

https://medium.com/@bvjebin/connecting-to-alloydb-from-your-local-39ca8f326ea9

### Database Migration Service

[Database Migration Service](https://cloud.google.com/database-migration
) (DMS) makes it easy to migrate your production databases to Cloud SQL with minimal downtime. This serverless offering eliminates the manual hassle of provisioning, managing, and monitoring migration-specific resources. DMS leverages the native replication capabilities of MySQL and PostgreSQL to maximize the fidelity and reliability of your migration. And it’s available at no additional charge for native like-to-like migrations to Cloud SQL.

https://cloud.google.com/blog/products/databases/migrate-oracle-to-postgresql

https://cloud.google.com/blog/products/databases/migrate-your-databases-to-google-cloud-with-the-new-database-migration-program

### In-pace updates 

https://cloud.google.com/blog/products/databases/cloud-sql-launches-support-for-in-place-upgrades

### High Availability

[HA](https://cloud.google.com/sql/docs/mysql/high-availability
) features reduce downtime when a zone or instance becomes unavailable which might happen during a zonal outage, or when an instance becomes corrupted.


### Importing and exporting data


https://cloud.google.com/sql/docs/mysql/import-export

### Users & IAM

https://cloud.google.com/sql/docs/mysql/add-manage-iam-users

### Security and Access Control

https://cloud.google.com/sql/docs/mysql/authentication

### Cloud SQL Auth proxy

https://cloud.google.com/sql/docs/mysql/sql-proxy

### Best Practices

https://cloud.google.com/sql/docs/mysql/best-practices

### Replication

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





### Maintenance

https://cloud.google.com/blog/products/databases/how-cloud-sql-maintenance-works-to-keep-instances-updated

### Backups


https://cloud.google.com/sql/docs/mysql/backup-recovery/backups

### Disaster Recovery

https://cloud.google.com/architecture/intro-to-cloud-sql-disaster-recovery

### Cloud SQL is not great

https://dev.to/mark_saward/cloud-sql-is-not-great-38ae

## PostgreSQL HA

https://cloud.google.com/sql/docs/postgres/high-availability

https://cloud.google.com/blog/products/gcp/cloud-sql-for-postgresql-adds-high-availability-and-replication

https://cloud.google.com/architecture/architectures-high-availability-postgresql-clusters-compute-engine


### SQL Server failover cluster

https://cloud.google.com/compute/docs/instances/sql-server/configure-failover-cluster-instance

### CloudSQL Insights

https://cloud.google.com/blog/products/databases/mysql-database-performance-monitoring

https://cloud.google.com/blog/products/databases/get-ahead-of-database-performance-issues-with-cloud-sql-insights

## Configuration

https://dev.to/hunghvu/random-configuration-tips-for-google-cloud-sql-2lg4

## Self-service maintenance

https://cloud.google.com/sql/docs/mysql/self-service-maintenance

## Tutorials



https://cloud.google.com/sql/docs/media

### backing up cloud sql to cloud storage using terraform and workflow 

https://medium.com/@titasmon/easily-backup-mysql-gcp-instances-to-gcp-storage-using-terraform-c798a11210ec

### Setting up PostgreSQL on GCE

https://cloud.google.com/community/tutorials/setting-up-postgres

### Setting up PostgreSQL data disk

https://cloud.google.com/community/tutorials/setting-up-postgres-data-disk

### PostgreSQL for high availability and replication with Hot Standby

https://cloud.google.com/community/tutorials/setting-up-postgres-hot-standby


### Migrating Postgres 

https://cloud.google.com/blog/topics/developers-practitioners/upgrade-postgres-pglogical-and-database-migration-service

### Creating alerts based on Cloud SQL logs

https://cloud.google.com/blog/products/databases/learn-how-to-create-alerts-based-on-your-database-logs-in-cloud-sql


### TXID freezing in PostgreSQL

https://cloud.google.com/blog/products/databases/how-to-accelerate-transaction-id-freezing-in-cloud-sql-for-postgresql

### Monitor Transaction ID

https://cloud.google.com/blog/products/databases/monitor-transaction-id-utilization-in-cloud-sql-postgresql

### Regain Cloud SQL disk space with Database Migration Service

https://medium.com/google-cloud/regain-cloud-sql-disk-space-with-database-migration-service-edabc708b1b0

## Examples

### extend datalake by querying cloud sql from bigquery over VPC peering 

https://medium.com/@attachew974/extend-your-datalake-with-cloudsql-and-bigquery-connections-b1acb8c4d9be

### Cherre use case with Postgres and GraphQL

https://cloud.google.com/blog/products/databases/how-cherre-creates-real-estate-data-products-with-cloud-sql

### Backup and restore using CURL

https://medium.com/@jason19930803/gcp-restore-cloud-sql-to-instance-in-another-project-631cb82d82c5

### Bi-directional replication for Cloud SQL for PostgreSQL using logical replication
https://cloud.google.com/blog/products/databases/setting-bi-directional-replication-for-cloud-sql-for-postgresql

