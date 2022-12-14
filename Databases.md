https://en.wikipedia.org/wiki/Database

## GCP Databases


There are many GCP databases: [BigQuery](BigQuery), [Bigtable](Bigtable), [Cloud SQL](  CloudSQL 
 ), [Datastore](Datastore), [Firebase](Firebase), [Firestore](Firestore), [Spanner](Spanner), and [Memorystore](Memorystore).


https://cloud.google.com/products/databases

https://cloud.google.com/blog/products/databases/google-clouds-key-investment-areas-to-accelerate-your-database-transformation

https://cloud.google.com/blog/products/databases/industry-leading-reliability-global-scale-open-standards-google-cloud-databases

## Cloud Databases

* [GCP Database Products](https://cloud.google.com/products/databases)
* [AWS Database products](https://aws.amazon.com/products/databases/) 
* [Azure databases](https://azure.microsoft.com/en-us/product-categories/databases/)
* [Oracle databases](https://www.oracle.com/database/)
* [IBM  DB2 database](https://www.ibm.com/cloud/db2-on-cloud)
* [SAP HANA Cloud](   https://www.sap.com/products/hana/cloud.html )


## Database paradigms

https://www.youtube.com/watch?v=W2Z7fbCLSTw


## SQL, NoSQL, NewSQL

[Structured Query Language](SQL) (SQL) is the standard language for data manipulation in a DBMS.

A [NoSQL](https://en.wikipedia.org/wiki/NoSQL) (originally referring to "non-SQL" or "non-relational") database provides a mechanism for storage and retrieval of data that is not modeled  in relational databases. 

[NewSQL](https://en.wikipedia.org/wiki/NewSQL) is a class of relational database management systems that seek to provide the scalability of NoSQL systems for online transaction processing (OLTP) workloads while maintaining the ACID guarantees of a traditional database system.


[HTAP](https://en.wikipedia.org/wiki/Hybrid_transactional/analytical_processing)  is an emerging application architecture merge transaction processing and analytics.  It may combine support for both [OLTP](https://en.wikipedia.org/wiki/Online_transaction_processing) and [OLAP](https://en.wikipedia.org/wiki/Online_analytical_processing).

A [Distributed SQL](https://en.wikipedia.org/wiki/Distributed_SQL) database is a single relational database which [replicates data across multiple servers](https://www.infoworld.com/article/3564543/beyond-nosql-the-case-for-distributed-sql.html). Distributed SQL databases are strongly consistent and most [support consistency](https://www.nextplatform.com/2021/01/25/after-three-decades-you-can-finally-have-a-distributed-sql-database/) across racks, data centers, and wide area networks including cloud availability zones and cloud geographic zones.


### NewSQL databases

https://medium.com/capital-one-tech/newsql-the-next-evolution-in-databases-19109973ee53

### SQL vs NOSQL

[https://www.virtual-dba.com/differences-between-sql-nosql-and-newsql/](https://www.virtual-dba.com/differences-between-sql-nosql-and-newsql/)


## Databases vs file systems

https://www.guru99.com/difference-between-file-system-and-dbms.html

## OLTP vs. OLAP

https://www.holistics.io/blog/the-rise-and-fall-of-the-olap-cube/

## ELT vs ETL

https://www.informatica.com/blogs/etl-vs-elt-whats-the-difference.html

### Reverse ETL

https://www.hightouch.io/

## Data lakes vs Data warehouses

https://aws.amazon.com/big-data/datalakes-and-analytics/what-is-a-data-lake/

## ACID, BASE, CAP

A [database transaction](  http://dist-prog-book.com/chapter/6/acidic-to-basic-how-the-database-ph-has-changed.html ) can be either a single operation or a sequence of operations, but is treated as a single logical operation on the data by the database. 

The [CAP theorem](  https://medium.com/@pranabj.aec/acid-cap-and-base-cc73dee43f8c ) dictates that the three desirable properties, [consistency, availability and partition tolerance](https://en.m.wikipedia.org/wiki/CAP_theorem) cannot be offered simultaneously. 



## Serializability, Linearizability, and locality


[Linearizability](https://accelazh.github.io/storage/Linearizability-Vs-Serializability-And-Distributed-Transactions-Copy) (also known as atomic consistency, strong consistency, immediate consistency) describes reads and writes on a single object (stores a single value).  [Serializability](https://aphyr.com/posts/333-serializability-linearizability-and-locality) deals with multiple objects.

## MVCC

[Multiversion concurrency control](https://wikipedia.org/wiki/Multiversion_concurrency_control)  (MCC or MVCC), is a concurrency control method commonly used by database management systems to provide concurrent access to the database and in programming languages to implement transactional memory.



## Distributed Consensus Protocols

[Distributed consensus problem](Distributed-Consensus) requires agreement among a number of processes (or agents) for a single data value. 

## Database of Databases

[https://dbdb.io/browse](https://dbdb.io/browse)

## Comparisons

https://kokizzu.blogspot.com/2021/11/databases-with-automatic-rebalance.html?m=1

https://www.cockroachlabs.com/docs/stable/cockroachdb-in-comparison.html


https://docs.yugabyte.com/latest/comparisons/

## PostgreSQL varieties


### Aurora

https://docs.aws.amazon.com/AmazonRDS/latest/AuroraUserGuide/CHAP_AuroraOverview.html

### Redshift

https://docs.aws.amazon.com/redshift/latest/dg/c_redshift-and-postgres-sql.html

### AlloyDB

https://cloud.google.com/blog/products/databases/alloydb-for-postgresql-intelligent-scalable-storage

#### AlloyDB Columnal Engine
https://cloud.google.com/blog/products/databases/alloydb-for-postgresql-columnar-engine

### TimescaleDB

https://www.timescale.com/

### PostgresML

https://postgresml.org/

### Other PostgreSQL derived databases

https://wiki.postgresql.org/wiki/PostgreSQL_derived_databases

## Other databases available on Google Cloud

### Databricks

https://medium.com/google-cloud/from-zero-to-hero-with-databricks-on-google-cloud-7cb41b1bfb30

### MongoDB Atlas

https://cloud.google.com/blog/topics/retail/unlocking-the-power-of-modern-devops

### Snowflake

https://www.snowflake.com/technology-partners/google-cloud-platform/

### Elasticsearch

https://www.elastic.co/cloud/elasticsearch-service/signup

### Oracle

https://medium.com/google-cloud-platform-by-cloud-ace/oracle-database-on-google-cloud-platform-what-do-you-need-to-know-1e331c874c24

### Vitess

https://cloudplatform.googleblog.com/2015/03/scaling-MySQL-in-the-cloud-with-Vitess-and-Kubernetes.html

### Hasura

https://hasura.io/docs/latest/graphql/core/deployment/deployment-guides/google-kubernetes-engine-cloud-sql.html

### GraphQL APIs with Apigee

https://cloud.google.com/blog/products/api-management/how-to-manage-your-graphql-apis-with-apigee

### MariaDB SkySQL on GCP

https://mariadb.com/products/skysql/google-cloud-platform/

### DataStax

https://www.datastax.com/platform/google-cloud-platform

#### Astra DB on GCP

https://docs.datastax.com/en/astra/docs/setting-up-an-astra-database-on-gcp.html