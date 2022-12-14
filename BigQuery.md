
[BigQuery](https://cloud.google.com/bigquery/docs)  is Google Cloud's [fully managed](https://www.youtube.com/watch?v=kKBnFsNWwYM), [serverless](serverless), petabyte-scale, SQL [data warehouse](https://cloud.google.com/solutions/bigquery-data-warehouse)  that lets you run [analytics over vast amounts](https://cloud.google.com/blog/topics/developers-practitioners/bigquery-explained-blog-series)  of data.

## Quickstart

https://cloud.google.com/bigquery/docs/quickstarts/quickstart-command-line


## Overview

https://medium.com/@knoldus/google-bigquery-an-introduction-to-big-data-analytics-platform-43a8935b69f3

### Using bq CLI

https://codelabs.developers.google.com/codelabs/bigquery-cli


### python

https://github.com/googleapis/python-bigquery

## Architecture




BigQuery has a [distributed architecture](https://cloud.google.com/blog/products/data-analytics/new-blog-series-bigquery-explained-overview) running on thousands of nodes across Google's data centers. Your datasets are not stored in a unique server but are chunked and replicated across different regions.

The [storage and compute layers are fully decoupled](https://cloud.google.com/blog/products/bigquery/separation-of-storage-and-compute-in-bigquery) in BigQuery. This means that the query engine runs on different servers from the servers where the data is stored. This feature enables BigQuery to provide great scalability both in terms of data volume and query execution. This decoupled paradigm is only possible thanks to [Google's Petabit network](https://cloud.google.com/blog/products/networking/google-cloud-networking-in-depth-how-andromeda-2-2-enables-high-throughput-vms), which moves data very quickly from one server to another, leveraging Google's proprietary fiber cables across the globe. 

Unlike traditional data warehouses, BigQuery stores data in [columnar format](https://towardsdatascience.com/want-to-use-bigquery-read-this-fab36822830) in [Google File System](https://cloud.google.com/blog/products/storage-data-transfer/a-peek-behind-colossus-googles-file-system) codename [Colossus](https://pierrezemb.fr/posts/colossus-google/). 


Fully [decoupled from storage](https://medium.com/@raigonjolly/separation-of-storage-and-compute-in-bigquery-7a0084c7cbe0), the [compute layer](https://research.google/pubs/pub43438/) is responsible for receiving query statements from BigQuery users and executing them in the fastest way. The query engine is based on [Dremel](https://research.google/pubs/pub36632/). 

BigQuery is an append-only database, meaning as new rows are updated, rows are added to the database, rather than being updated in place. 

BigQuery supports [Standard SQL](https://cloud.google.com/bigquery/docs/reference/standard-sql/introduction).

Each node provides a number of processing units called [BigQuery slots](https://cloud.google.com/bigquery/docs/slots) to execute the business logic of the query. A BigQuery slot can be considered a virtual CPU on a Dremel node. The calculation of the slots needed to perform a specific query is automatically managed depending on the complexity of the query and impacted data volumes.

### Beginner's Guide
https://medium.com/google-cloud/a-seniors-guide-to-kickstart-your-bigquery-journey-75566e131983

### No Index

Each time BigQuery executes a query, it executes [a full-column scan](https://towardsdatascience.com/want-to-use-bigquery-read-this-fab36822830). BigQuery doesn't use or support indexes. Because BigQuery performance and query s are based on the amount of data scanned during a query, design your queries so that they reference only the columns that are relevant to the query. 

https://cloud.google.com/files/BigQueryTechnicalWP.pdf

https://cloud.google.com/bigquery/docs/querying-partitioned-tables

https://github.com/jorwalk/data-engineering-gcp/blob/master/know/bigquery/best-practices-performance-input.md

https://cloud.google.com/architecture/bigquery-data-warehouse#query_optimization

### Data Types

https://cloud.google.com/bigquery/docs/reference/standard-sql/data-types

### Query Syntax

https://cloud.google.com/bigquery/docs/reference/standard-sql/query-syntax

### Query Plan

The Query Plan explanation breaks down the stages that the query went through, the number of input/output rows handled at each stage, and the timing profile within each stage. Using the results from the explanation can help you understand and optimize your queries.


https://cloud.google.com/blog/topics/developers-practitioners/bigquery-admin-reference-guide-query-processing


### Serverless

There's no infrastructure to manage in BigQuery. Developers [focus on finding insights](https://cloudblog.withgoogle.com/products/data-analytics/new-blog-series-bigquery-explained-overview/) using standard SQL using on-demand or flat-rate options.

### Wide Column Storage

[BigQuery](https://www.youtube.com/watch?v=sUcInkIqClI&list=PL6oqHwbsfYMwAC5cedqFSCQwaO_gBoYf8&index=1)  is designed to [ingest and store](https://www.youtube.com/watch?v=d3MDxC_iuaw) large amounts of data, and make that data accessible for [large-scale analytics](https://www.youtube.com/watch?v=JLXLCv5nUCE&list=PLIivdWyY5sqIZLeLzyg1B-Pd1MIOo6d-g). BigQuery [stores data in wide columns](https://www.youtube.com/watch?v=1gYUGv_omJA) which are in separate files that are compressed and work well with distributed systems like [Colossus](https://cloud.google.com/blog/products/storage-data-transfer/a-peek-behind-colossus-googles-file-system). 


https://cloud.google.com/blog/topics/developers-practitioners/bigquery-admin-reference-guide-storage


### In-Memory Shuffling

BigQuery  uses [dynamic query planning](https://cloud.google.com/bigquery/query-plan-explanation) and different shards using in-memory shuffling for optimal distributed performance.

[Clustered tables](https://cloud.google.com/bigquery/docs/clustered-tables)  allow for [better partitioning and performance](https://www.youtube.com/watch?v=1gYUGv_omJA).


### Loading Data

Learn [how to load](https://www.youtube.com/watch?v=Abzj-Vyhi74) CSV data in batch and analyze in BigQuery.

### Peta Bytes

[BigQuery](https://www.youtube.com/watch?v=ZVgt1-LfWW4) is [fully managed](https://www.youtube.com/watch?v=7bW7P-8SJ_4&list=PLIivdWyY5sqIF17nHLuY3_XkFjrqb54Hw&index=1) and lets you search through [terabytes of data in seconds](https://www.youtube.com/watch?v=qqbYrQGSibQ). 

### BigQuery Data Transfer Service

You can [upload data](https://cloud.google.com/bigquery/docs/batch-loading-data?skip_cache=true) files from local sources, Google Drive, or Cloud Storage buckets, take advantage of [BigQuery Data Transfer Service](https://cloud.google.com/bigquery-transfer/docs/introduction) (DTS), [Cloud Data Fusion](Data-Fusion) plug-ins, or leverage Google's industry-leading [data integration partnerships](https://cloud.google.com/bigquery?skip_cache=true#section-12). 

### BigQuery Migration Service

https://cloud.google.com/blog/topics/data-warehousing/announcing-bigquery-migration-service

### Anatomy of a BigQuery query

Google [BigQuery](https://cloud.google.com/blog/products/gcp/bigquery-under-the-hood) has the [benchmark data](https://console.cloud.google.com/bigquery?project=publicdata&page=table&t=wikipedia&d=samples&p=publicdata) for the Wiki100B table. This table contains 100 billion rows and is about 7 Terabytes in size.


[https://cloud.google.com/blog/products/gcp/anatomy-of-a-bigquery-query](https://cloud.google.com/blog/products/gcp/anatomy-of-a-bigquery-query)

### In memory query execution

BigQuery is a fast petabyte-scale analytics database. To achieve that level of performance, BigQuery executes queries completely in memory by leveraging Google???s peta bit scale networking technologies, such as [Andromeda and Jupiter](https://cloud.google.com/blog/products/networking/google-cloud-networking-in-depth-how-andromeda-2-2-enables-high-throughput-vms).

[Shuffle](https://cloud.google.com/blog/products/bigquery/in-memory-query-execution-in-google-bigquery) is required for execution of large and complex joins, aggregations and analytic operations. 

<!--
[[https://storage.googleapis.com/gweb-cloudblog-publish/images/in-memory-query-2ntao.max-700x700.PNG]]
-->

[In-memory BigQuery shuffle](https://cloud.google.com/blog/products/gcp/in-memory-query-execution-in-google-bigquery) stores intermediate data produced from various stages of query processing in a set of nodes that are dedicated to hosting remote memory. 





### Query plan and timeline


When BigQuery executes a query job, it converts the declarative SQL statement into a graph of execution, broken up into a [series of query stages](https://cloud.google.com/bigquery/query-plan-explanation), which themselves are composed of [more granular sets of execution steps](https://cloud.google.com/bigquery/query-plan-explanation). 


### Managing input data and data sources

When [evaluating](https://cloud.google.com/bigquery/docs/best-practices-performance-input) your input data, consider the required I/O. How many bytes does your query read? Are you properly limiting the amount of input data? Is your data in native BigQuery storage or an external data source? The amount of data read by a query and the source of the data impact query performance and .



### BigQuery Spanner federation 

BigQuery [Spanner](Spanner) federation  enables BigQuery to query data residing in [Spanner](Spanner) in real-time, without copying or moving data.

https://cloud.google.com/bigquery/docs/cloud-spanner-federated-queries

### Replicating from Cloud Spanner to BigQuery at scale

https://cloud.google.com/blog/topics/developers-practitioners/replicating-cloud-spanner-bigquery-scale

### Optimizing communication between slots

When evaluating your [communication between slots](https://cloud.google.com/bigquery/docs/best-practices-performance-communication) consider the amount of shuffling that is required by your query. How many bytes are passed between stages? How many bytes are passed to each slot? The amount of data that is shuffled directly impacts communication throughput and  query performance.

### Optimizing against multiple reads

https://boonepeter.github.io/posts/unnecessary_bigquery_optimization

### Time Travel

BigQuery lets you use [time travel](https://cloud.google.com/bigquery/docs/time-travel
) to access data stored in BigQuery that has been changed or deleted. You can access the data from any point within the last seven days. You can use time travel to query data that was updated or deleted, restore a table that was deleted, or restore a table that expired.

https://cloud.google.com/bigquery/docs/time-travel

https://medium.com/codex/more-options-to-restore-your-data-in-google-bigquery-181a32f7fa76

### Optimizing query computation

When evaluating the computation that is required by a query, consider the [amount of work](https://cloud.google.com/bigquery/docs/best-practices-performance-compute) that is required. How much CPU time is required? Are you using functions like JavaScript user-defined functions that require additional CPU resources?




### Managing materialization and outputs

When [evaluating your output data](https://cloud.google.com/bigquery/docs/best-practices-performance-output), consider the number of bytes written by your query. How many bytes are written for your result set? Are you properly limiting the amount of data written? Are you repeatedly writing the same data? The amount of data written by a query impacts query performance (I/O). If you are writing results to a permanent (destination) table, the amount of data written also has a .


## BigQuery BI Engine
BI Engine is an in-memory analysis service that helps customers get low latency performance for their queries across all [BI](Business-Intelligence) tools that connect to [BigQuery](BigQuery).

https://cloud.google.com/bigquery/docs/bi-engine-intro


## Comparisons

https://dzone.com/articles/cloud-data-warehouse-comparison-redshift-vs-bigque


### Migration from Redshift to BigQuery

https://medium.com/99dotco/a-migration-misstep-from-redshift-to-bigquery-13e9000c3f50

## Using BigQuery

### Anti patterns

Avoid [query anti-patterns](https://cloud.google.com/bigquery/docs/best-practices-performance-patterns) that impact performance in BigQuery.

### Partitions and Clusters

https://towardsdatascience.com/how-to-use-partitions-and-clusters-in-bigquery-using-sql-ccf84c89dd65

### Managing partitioned tables

A [partitioned table](https://cloud.google.com/bigquery/docs/partitioned-tables) is a special table that is divided into segments, called partitions, that make it easier to manage and query your data. By dividing a large table into smaller partitions, you can improve query performance, and you can control s by reducing the number of bytes read by a query.


You can partition BigQuery tables by:

- [Time-unit column](https://cloud.google.com/bigquery/docs/partitioned-tables#date_timestamp_partitioned_tables): Tables are partitioned based on a TIMESTAMP, DATE, or DATETIME column in the table.
- [Ingestion time](https://cloud.google.com/bigquery/docs/partitioned-tables#ingestion_time): Tables are partitioned based on the timestamp when BigQuery ingests the data.
- [Integer range](https://cloud.google.com/bigquery/docs/partitioned-tables#integer_range): Tables are partitioned based on an integer column.

If a query filters on the value of the partitioning column, BigQuery can scan the partitions that match the filter and skip the remaining partitions. This process is called pruning.


https://cloud.google.com/bigquery/docs/managing-partitioned-tables


### Using datasets

A [dataset](https://cloud.google.com/bigquery/docs/datasets-intro
) is contained within a specific project. Datasets are top-level containers that are used to organize and control access to your tables and views. A table or view must belong to a dataset, so you need to create at least one dataset before loading data into BigQuery.


BigQuery datasets are subject to the following limitations:

- You can set the geographic location at creation time only. After a dataset has been created, the location becomes immutable and can't be changed by using the Cloud Console, using the bq command-line tool, or calling the patch or update API methods.
All tables that are referenced in a query must be stored in datasets in the same location.
- When you copy a table, the datasets that contain the source table and destination table must reside in the same location.
- Dataset names must be unique for each project.

https://cloud.google.com/bigquery/docs/datasets-intro

### Using dataset properties

After you create a dataset, you can update the following dataset properties:

- Description
- Default expiration time for new tables
- Default partition expiration for new partitioned tables
- Access controls
- Labels


https://cloud.google.com/bigquery/docs/updating-datasets

### BigQuery data update optimization by partitioning 
https://medium.com/cstech/google-bigquery-data-update-optimization-9d788bfe811b

### Updating default table expiration times

https://cloud.google.com/bigquery/docs/updating-datasets#table-expiration

### Using tables

A BigQuery table contains individual records organized in rows. Each record is composed of columns (also called fields).

Every table is defined by a schema that describes the column names, data types, and other information. You can specify the schema of a table when it is created, or you can create a table without a schema and declare the schema in the query job or load job that first populates it with data.

BigQuery supports the following table types:

- Native tables: tables backed by native BigQuery storage.
- External tables: tables backed by storage external to BigQuery. For more information, see Querying External Data Sources.
- Views: Virtual tables defined by a SQL query. For more information, see Creating views.

https://cloud.google.com/bigquery/docs/tables-intro

### Table schemas

https://cloud.google.com/bigquery/docs/schemas




### Clustered tables

When you create a clustered table in BigQuery, the table data is automatically organized based on the contents of one or more columns in the table???s schema. The columns you specify are used to colocate related data. When you cluster a table using multiple columns, the order of columns you specify is important. The order of the specified columns determines the sort order of the data.

Clustering can improve the performance of certain types of queries such as queries that use filter clauses and queries that aggregate data. When data is written to a clustered table by a query job or a load job, BigQuery sorts the data using the values in the clustering columns. These values are used to organize the data into multiple blocks in BigQuery storage. When you submit a query that contains a clause that filters data based on the clustering columns, BigQuery uses the sorted blocks to eliminate scans of unnecessary data. You might not see a significant difference in query performance between a clustered and unclustered table if the table or partition is under 1 GB.


https://cloud.google.com/bigquery/docs/clustered-tables


### Paritioning vs. clustering

Both partitioning and clustering can improve performance and reduce query .  Use clustering when you don't need strict  guarantees before running the query.  Use partitioning when you want to know query s before a query runs.  You may prefer cluster over partitioning when partitioning results in a small amount of data per partition approximately less than  1GB.

https://cloud.google.com/bigquery/docs/partitioned-tables#partitioning_versus_clustering

### Views

A view is a virtual table defined by a SQL query. When you create a view, you query it in the same way you query a table. When a user queries the view, the query results contain data only from the tables and fields specified in the query that defines the view.

https://cloud.google.com/bigquery/docs/views-intro

### Materialized Views

In BigQuery, [materialized views](https://cloud.google.com/bigquery/docs/materialized-views-intro
) are precomputed views that periodically cache the results of a query for increased performance and efficiency. BigQuery leverages precomputed results from materialized views and whenever possible reads only delta changes from the base table to compute up-to-date results. Materialized views can be queried directly or can be used by the BigQuery optimizer to process queries to the base tables.

Queries that use materialized views are generally faster and consume fewer resources than queries that retrieve the same data only from the base table. Materialized views can significantly improve the performance of workloads that have the characteristic of common and repeated queries.


https://cloud.google.com/bigquery/docs/materialized-views-intro

### Remote Functions

https://cloud.google.com/blog/products/data-analytics/extending-bigquery-functions


https://towardsdatascience.com/remote-functions-in-bigquery-af9921498438

### Reservations


BigQuery [Reservations](https://cloud.google.com/bigquery/docs/reservations-intro
) enables you to switch between on-demand pricing and flat-rate pricing. With flat-rate pricing, you purchase dedicated query processing capacity. You can allocate this capacity across your organization, by reserving pools of capacity for different projects or different parts of your organization. You can also combine the two billing models, taking advantage of both on-demand and flat-rate pricing.

https://cloud.google.com/bigquery/docs/reservations-intro


https://cloud.google.com/blog/topics/developers-practitioners/bigquery-admin-reference-guide-jobs-reservation-model


### Scheduling queries

https://cloud.google.com/bigquery/docs/scheduling-queries

### Scripting

https://jimbeepbeep.medium.com/getting-started-with-bigquery-scripting-45bdd968010c

https://cloud.google.com/bigquery/docs/reference/standard-sql/scripting


### Audit Logs


https://cloud.google.com/blog/products/data-analytics/bigquery-audit-logs-pipelines-analysis


### BigQuery BI Engine Preferred Tables
https://cloud.google.com/blog/products/data-analytics/now-in-preview-bigquery-bi-engine-preferred-tables

### Controlling s

https://cloud.google.com/bigquery/docs/controlling-s

#### Optimizing BigQuery  with Looker

https://cloud.google.com/blog/topics/developers-practitioners/optimizing-your-google-cloud-spend-bigquery-and-looker

#### Optimizing strategies

https://fares-daoud.medium.com/how-i-have-optimized-bigquery-s-for-my-company-948df95b9f0d

### Organizing BigQuery resources

Resource Hierarchy.

https://cloud.google.com/bigquery/docs/resource-hierarchy


### Dataform

https://cloud.google.com/blog/products/data-analytics/welcoming-dataform-to-bigquery

Dataform is a platform to manage data in BigQuery, Snowflake, Redshift, and other data warehouses. It helps data teams build data pipelines that turn raw data into new tables and views that can be used for analytics.

Dataform does the T in ELT (Extract, Load, Transform) processes. It doesn???t extract or loads data in your warehouse but it???s very powerful to transform data already loaded in your warehouse.

https://medium.com/@danilo.drobac/supercharge-your-bigquery-data-warehouse-with-dataform-d871d4df123a







#### Dataform SQLX

https://docs.dataform.co/introduction/dataform-in-5-minutes

### UDF

https://cloud.google.com/bigquery/docs/reference/standard-sql/user-defined-functions

https://towardsdatascience.com/bigquery-udfs-complete-guide-181cbdaea55b

#### Testing UDF with Dataform

https://cloud.google.com/blog/topics/data-warehousing/learn-how-to-use-the-dataform-cli-tool-to-unit-test-udf

### Collation
https://medium.com/codex/using-collation-in-google-bigquery-e63d34ee4799

### Testable SQL

https://tufin.medium.com/testable-bigquery-sql-61a911e35ab5


### transaction and session 


#### multi statement transactions 

https://cloud.google.com/bigquery/docs/reference/standard-sql/transactions

#### writing queries in sessions 

https://cloud.google.com/bigquery/docs/sessions-write-queries

#### transactions with multiple queries with sessions 

https://dev.to/stack-labs/bigquery-transactions-over-multiple-queries-with-sessions-2ll5


### MERGE

https://medium.com/plumbersofdatascience/incremental-data-ingestion-in-bigquery-using-merge-1387e49c7eb5


### Data Fusion

[Data Fusion](Data-Fusion) is built using open source project [CDAP](https://github.com/cdapio/cdap).  It is a GUI based data integration service for building and managing data pipelines.

https://cloud.google.com/data-fusion/

#### Import CSV data into BigQuery using Data Fusion

https://codelabs.developers.google.com/codelabs/batch-csv-cdf-bq

### Datastream  and Data Fusion

https://cloud.google.com/blog/products/vmware-engine/visual-data-with-bigquery-and-google-cloud-vmware-engine

### Dremel

[Dremel](https://research.google/pubs/pub36632/) is a scalable, interactive ad-hoc query system for analysis of read-only nested data. BigQuery is based on Dremel.

https://www.wired.com/2012/08/googles-dremel-makes-big-data-look-small/

Dremel has been in production at Google since 2006. A selection of use cases for Dremel at Google include analysis of:

- Crawled web documents
- Spam
- Build system results
- Crash reports

Further, there are two ways to use Dremel outside of Google. The first is Google???s BigQuery service, which Google provides as part of its cloud offering. The second is [Apache Drill](  https://drill.apache.org/  ), effectively an open source re-implementation of Dremel. [Cloudera Impala](  https://wikipedia.org/wiki/Apache_Impala  ) is also influenced by Dremel. As is [Presto](  https://prestodb.io/  ) and [Dremio](   https://www.dremio.com/architectural-analysis-why-dremio-is-faster-than-any-presto ).  All these are addressing SQL over Hadoop issues.

http://www.goldsborough.me/distributed-systems/2019/05/18/21-09-00-a_look_at_dremel/

### INFORMATION_SCHEMA

INFORMATION_SCHEMA is a series of views that provide access to metadata about datasets, routines, tables, views, jobs, reservations, and streaming data.

https://cloud.google.com/bigquery/docs/information-schema-intro

You can query the INFORMATION_SCHEMA.JOBS_TIMELINE_BY_* views to retrieve real-time BigQuery metadata by timeslice. This view contains currently running and completed jobs. Data is retained for 180 days.

https://cloud.google.com/bigquery/docs/information-schema-jobs-timeline

#### Monitor and analyze BigQuery performance using information schema
https://cloud.google.com/blog/topics/developers-practitioners/monitor-analyze-bigquery-performance-using-information-schema

### Denormalize whenever possible

https://cloud.google.com/bigquery/docs/best-practices-performance-input#denormalize_data_whenever_possible


### Building the world???s largest data warehouse

[https://www.youtube.com/watch?v=1gYUGv_omJA](https://www.youtube.com/watch?v=1gYUGv_omJA)



### BigQuery nested and repeated fields

[https://www.youtube.com/watch?v=STo98QUKDS8](https://www.youtube.com/watch?v=STo98QUKDS8)

### SEARCH INDEX

https://levelup.gitconnected.com/enhancing-bigquery-search-features-with-search-index-771c1eec186e


### BigQuery, Snowflake and Redshift

[Compare](https://medium.com/2359media/redshift-vs-bigquery-vs-snowflake-a-comparison-of-the-most-popular-data-warehouse-for-data-driven-cb1c10ac8555) and [review](https://www.youtube.com/watch?v=XpaN-PqSczM
) various Data Warehousing solutions: BigQuery, [Snowflake](https://0x0fff.com/snowflake-the-good-the-bad-and-the-ugly/) and [RedShift](https://aws.amazon.com/redshift/).



### Snowflake, Star, Galaxy

[Star Schema]( https://wikipedia.org/wiki/Star_schema)   in a data warehouse, in which the center of the star can have one fact table and a number of associated dimension tables. It is known as star schema as its structure resembles a star. The Star Schema data model is the simplest type of Data Warehouse schema. It is also known as Star Join Schema and is optimized for querying large data sets.

[Snowflake Schema](  https://wikipedia.org/wiki/Snowflake_schema  ) in a data warehouse is a logical arrangement of tables in a multidimensional database such that the [ER diagram](https://www.guru99.com/er-diagram-tutorial-dbms.html) resembles a snowflake shape. A Snowflake Schema is an extension of a Star Schema, and it adds additional dimensions. The dimension tables are normalized which splits data into additional tables.

A [Galaxy Schema](  https://www.educba.com/galaxy-schema/  ) contains two fact table that share dimension tables between them. It is also called Fact Constellation Schema. The schema is viewed as a collection of stars hence the name Galaxy Schema.

[https://www.guru99.com/star-snowflake-data-warehousing.html](https://www.guru99.com/star-snowflake-data-warehousing.html)


### Denormalization

[Denormalization](https://en.wikipedia.org/wiki/Denormalization) is a strategy used on a previously-normalized database to increase performance. In computing, denormalization is the process of trying to improve the read performance of a database, at the expense of losing some write performance, by adding redundant copies of data or by grouping data.

### Transactions

https://cloud.google.com/bigquery/docs/reference/standard-sql/transactions

### Write API

https://cloud.google.com/blog/topics/developers-practitioners/bigquery-write-api-explained-overview-write-api


### Streaming JSON data via Storage Write API

https://cloud.google.com/blog/topics/developers-practitioners/learn-how-stream-json-data-bigquery-using-new-bigquery-storage-write-api

### Storage Write API with Kafka to stream deliver data exactly once

https://medium.com/@wojcikpawel/exactly-once-delivery-in-bigquerys-storage-write-api-67885c5c5e16

### Public Datasets

[https://cloud.google.com/bigquery/public-data](https://cloud.google.com/bigquery/public-data)

### Query queues for concurrency
https://medium.com/codex/bigquery-now-supporting-query-queues-378a65fdc9c1

### BigQuery Standard SQL

BigQuery supports two different SQL dialects: standard SQL and legacy SQL. Legacy SQL may be useful if you want to test queries coming from legacy applications.

https://cloud.google.com/blog/topics/developers-practitioners/bigquery-explained-querying-your-data

BigQuery was developed as an internal product within Google and was initially realized to process log records. The query engine Dremel was able to support a limited set of SQL operations that are now defined as Legacy SQL.

[https://cloud.google.com/bigquery/docs/reference/standard-sql/migrating-from-legacy-sql](https://cloud.google.com/bigquery/docs/reference/standard-sql/migrating-from-legacy-sql)

### Table Snapshots

https://cloud.google.com/blog/products/data-analytics/google-bigquery-table-snapshots-for-data-backups

### Newer features in BigQuery SQL

https://cloud.google.com/blog/topics/developers-practitioners/spring-forward-bigquery-user-friendly-sql

https://cloud.google.com/blog/topics/developers-practitioners/shine-user-friendly-sql-bigquery

### Analytics
https://cloud.google.com/bigquery/docs/query-overview

### Analytics Hub
https://cloud.google.com/bigquery/docs/analytics-hub-introduction

### BigQuery BI Engine 

[BigQuery BI Engine](https://cloud.google.com/bi-engine/docs) is a fast, in-memory analysis service that allows you to analyze data stored in BigQuery. 


https://cloud.google.com/bigquery/docs/bi-engine-intro

https://cloud.google.com/blog/products/data-analytics/bigquery-bi-engine-generally-available

#### BigQuery BI Engine Preferred tables
https://cloud.google.com/blog/products/data-analytics/now-in-preview-bigquery-bi-engine-preferred-tables

#### Data  Studio

https://cloud.google.com/bigquery/docs/bi-engine-data-studio

#### Looker


https://cloud.google.com/bigquery/docs/analyze-data-looker


#### Tableau

https://cloud.google.com/bigquery/docs/analyze-data-tableau

#### Connected Sheets

https://cloud.google.com/bigquery/docs/connected-sheets

#### Excel connector
https://cloud.google.com/bigquery/docs/bigquery-connector-for-excel


#### Datalab
https://cloud.google.com/architecture/analyzing-financial-time-series-using-bigquery-and-cloud-datalab

### Data Security 

#### Data Governance

[Data governance](https://cloud.google.com/bigquery/docs/data-governance
) is a principled approach to manage data during its lifecycle ??? from acquisition, to use, to disposal. Your data governance program clearly outlines policies, procedures, responsibilities, and controls surrounding data activities. This program helps to ensure that information is collected, maintained, used, and disseminated in such a way that both meets your organization's data integrity and [security](security) needs, and also helps empower your employees to discover and use the data to its fullest potential.


https://cloud.google.com/bigquery/docs/data-governance


[https://cloud.google.com/blog/products/data-analytics/data-governance-new-ways-to-securely-access-and-discover-data](https://cloud.google.com/blog/products/data-analytics/data-governance-new-ways-to-securely-access-and-discover-data)

#### BigQuery Access Control

https://medium.com/@VishalBulbule/access-control-in-bigquery-d5d800654f47

#### BigQuery Access Control Examples

https://cloud.google.com/bigquery/docs/access-control-examples

#### BigQuery Data Encryption

https://cloud.google.com/bigquery/docs/encryption-at-rest

#### BigQuery column-level security

https://cloud.google.com/bigquery/docs/column-level-security

#### BigQuery column-level encryption functions
https://cloud.google.com/blog/products/identity-security/announcing-new-bigquery-capabilities-to-help-secure-sensitive-data


#### Restricting access to columns
https://medium.com/plumbersofdatascience/restrict-access-to-columns-on-bigquery-1550895b3356
#### BigQuery row-level security

https://cloud.google.com/blog/products/data-analytics/bigquery-provides-tighter-controls-over-data-access

#### Column based data masking
https://medium.com/codex/google-improves-data-security-in-bigquery-195a90cc5b85

#### Dynamic data masking

https://cloud.google.com/blog/products/identity-security/announcing-new-bigquery-capabilities-to-help-secure-sensitive-data


https://medium.com/plumbersofdatascience/dynamic-data-masking-on-bigquery-ae3d004b496c


### Using Connected Sheets with BigQuery

With [Connected Sheets](https://cloud.google.com/bigquery/docs/connected-sheets
), you can access, analyze, visualize, and share billions of rows of BigQuery data from your Sheets spreadsheet.

You can also do the following:

- Collaborate with partners, analysts, or other stakeholders in a familiar spreadsheet interface.
- Ensure a single source of truth for data analysis without additional spreadsheet exports.
- Streamline your reporting and dashboard workflows.



https://cloud.google.com/bigquery/docs/connected-sheets


###  BigQuery Migration Service (BQMS)

https://cloud.google.com/blog/products/data-analytics/automated-sql-translation-to-accelerate-bigquery-migrations

### Pricing

BigQuery is a [serverless](Serverless) data analytics platform. You don't need to provision individual instances or virtual machines to use BigQuery. Instead, BigQuery automatically allocates computing resources as you need them. You can also reserve compute capacity ahead of time in the form of slots, which represent virtual CPUs. The pricing structure of BigQuery reflects this design.

[BigQuery pricing](https://cloud.google.com/bigquery/pricing
) has two main components:

- Analysis pricing is the  to process queries, including SQL queries, user-defined functions, scripts, and certain data manipulation language (DML) and data definition language (DDL) statements that scan tables.

- Storage pricing is the  to store data that you load into BigQuery.


https://cloud.google.com/bigquery/pricing

### BigQuery Flex Slots

https://cloud.google.com/blog/products/data-analytics/introducing-bigquery-flex-slots

### Flat rate

https://cloud.google.com/bigquery/pricing#flat_rate_pricing

### Controlling cost

https://cloud.google.com/blog/topics/developers-practitioners/controlling-your-bigquery-costs

### Resource Charts and Slot Estimator

https://cloud.google.com/blog/products/data-analytics/bigquery-administrator-hub-helps-manage-bigquery-at-scale

### Regional performances


https://medium.com/google-cloud/bigquery-tell-me-your-region-i-will-tell-you-your-speed-41dcf42b8cc


### Sandbox

https://cloud.google.com/bigquery/docs/sandbox

### Importing existing BigQuery Resources to Terraform

https://medium.com/trendyol-tech/importing-existing-bigquery-resources-to-terraform-automatically-f52a36b6e819

### Looker and BigQuery

[Looker](Looker) is an enterprise platform for business intelligence, data applications, and embedded analytics. Looker helps you explore, share, and visualize your company's data so that you can make better business decisions.


https://cloud.google.com/bigquery/docs/looker



### BigQuery Performance Optimization

https://towardsdatascience.com/14-ways-to-optimize-bigquery-sql-for-ferrari-speed-at-honda--632ec705979

### BigQuery GIS 

[BigQuery GIS](https://cloud.google.com/bigquery/docs/gis-intro) uniquely combines the serverless architecture of BigQuery with native support for geospatial analysis, so you can augment your analytics workflows with location intelligence. 

https://mentin.medium.com/bigquery-geospatial-query-tricks-8ebb4453ab5e

### BigQuery Omni

[BigQuery Omni](https://cloud.google.com/blog/products/data-analytics/introducing-bigquery-omni) is a flexible, fully managed, multi-cloud analytics solution that allows you to analyze data across clouds such as AWS and Azure. 

https://medium.com/google-cloud/bigquery-omni-is-everywhere-afa2b5f64688

https://ravi-manjunatha.medium.com/multi-cloud-analytics-with-bigquery-omni-no-time-to-load-ed187a9dcf20

https://cloud.google.com/blog/products/data-analytics/bq-omnis-cross-cloud-transfer-combines-data-across-clouds

### BigQuery ML 

[BigQuery ML](BigQuery-ML) enables users to create and execute machine learning models in BigQuery by using SQL queries.


### Comparing BigQuery Processing and Spark Dataproc

https://medium.com/paypal-tech/comparing-bigquery-processing-and-spark-dataproc-4c90c10e31ac

### BigQuery Metadata

https://betterprogramming.pub/4-ways-big-query-metadata-can-help-you-2cdf3b899fbc

### Metadata of all tables

https://medium.com/@erkan.ekser/how-to-keep-metadata-of-all-tables-in-bigquery-125516742bad

### BigQuery Scripting

https://cloud.google.com/bigquery/docs/reference/standard-sql/scripting

https://jimbeepbeep.medium.com/getting-started-with-bigquery-scripting-45bdd968010c?p=4bb74216b8c8


### BigQuery Clustered Tables from Beam

https://medium.com/@whatwouldaustindo/bigquery-clustered-tables-from-beam-now-available-without-partitioning-d2d24453eef6

### Pandas-gbq

https://cloud.google.com/bigquery/docs/pandas-gbq-migration

### BigQuery Storage API

https://cloud.google.com/bigquery/docs/bigquery-storage-python-pandas

#### Storage Read API Quotas

https://medium.com/codex/improved-storage-read-api-quotas-in-google-bigquery-f415a4c27bf1

### BigQuery data in a Jupyter notebook

https://cloud.google.com/bigquery/docs/visualize-jupyter


### BigQuery perspectives

https://medium.com/codeshake/bigquery-101-how-to-tame-the-beast-part-3-212356720b18

## BigQuery tutorials

[https://cloud.google.com/bigquery/docs/tutorials](https://cloud.google.com/bigquery/docs/tutorials)


### From GCS to BigQuery

https://jimbeepbeep.medium.com/google-cloud-storage-gcs-to-bigquery-the-simple-way-4bb74216b8c8

### Basics

https://blog.coupler.io/bigquery-tutorial/

### Importing data

https://digitalmarketinglikeapro.medium.com/5-ways-to-importing-marketing-data-into-bigquery-5355aafa36e8

### Learn writing java code to connect Dataproc map/reduce to BigQuery

[https://cloud.google.com/dataproc/docs/tutorials/bigquery-connector-mapreduce-example](https://cloud.google.com/dataproc/docs/tutorials/bigquery-connector-mapreduce-example)


### BigQuery connector to Spark

[https://cloud.google.com/dataproc/docs/tutorials/bigquery-connector-spark-example](https://cloud.google.com/dataproc/docs/tutorials/bigquery-connector-spark-example)



https://cloud.google.com/bigquery/docs/tutorials

### Authorize and Share access views

https://cloud.google.com/bigquery/docs/share-access-views

### Using BigQuery GIS to plot a hurricane's path

https://cloud.google.com/bigquery/docs/gis-tutorial-hurricane

### Visualize BigQuery data in Jupyter notebook

https://cloud.google.com/bigquery/docs/visualize-jupyter

### External data sources into BigQuery

https://medium.com/google-cloud/how-to-integrate-external-data-sources-with-bigquery-9e126d5751ea

### BigQuery GIS tutorial

https://cloud.google.com/bigquery/docs/gis-tutorial-hurricane

### Sync data from MySQL to BigQuery

https://blog.fourninecloud.com/how-to-sync-data-from-mysql-to-bigquery-9ef980ef602c

### Three ways to query in Python

https://towardsdatascience.com/3-ways-to-query-bigquery-in-python-66838f45cb43


### Genomics Analytics with BigQuery

https://cloud.google.com/blog/products/data-analytics/genomics-data-analytics-with-cloud-pt2

### Dynamic SQL using Jinja Template

https://soumendra-mishra.medium.com/bigquery-dynamic-sql-using-jinja-template-5c1332317960

### Bike Share membership 

https://medium.com/@urruchua.xabier/bike-share-chicago-case-study-72444a268dd1

### Game user data analytics

https://towardsdatascience.com/know-more-about-your-app-users-through-bigquery-4c0b6d67abfa

### Informatica Data Loader for BigQuery

https://cloud.google.com/blog/products/data-analytics/data-loader-speeds-up-time-to-value-for-bigquery-users


### Ploomer

https://github.com/ploomber/ploomber

https://towardsdatascience.com/analyze-and-plot-5-5m-records-in-20s-with-bigquery-and-ploomber-8bf7646c031

### Data Quality Analysis using BigQuery


https://medium.com/google-cloud/simplifying-data-quality-analysis-808e9fb8667f

### Streaming data into BigQuery using Cloud Run

https://medium.com/google-cloud/streaming-data-into-bigquery-using-google-cloud-run-469365a731b9

### Migrating from AWS Glue to BigQuery

https://towardsdatascience.com/migrating-from-aws-glue-to-bigquery-for-etl-ac12980f2036

### Firehose Kafka data ingestion
https://cloud.google.com/blog/products/data-analytics/introducing-firehose-an-open-source-tool-from-gojek

### Dynamic SQL Stored Procedure

https://medium.com/@michalwesleymnach/an-introduction-to-dynamic-sql-in-bigquery-4c8bb8d6dde7

### Bqfetch


https://towardsdatascience.com/the-fastest-way-to-fetch-bigquery-tables-352e2e26c9e1

### BigQuery fetching and Multi-processing

https://towardsdatascience.com/bigquery-fetching-multiprocessing-dcb79de50108

### Monitoring BigQuery

https://medium.com/teads-engineering/managing-a-bigquery-data-warehouse-at-scale-e6ec9a8406b2

### Mathematical functions and numbers

https://medium.com/geekculture/mathematical-functions-you-should-know-in-bigquery-ee674109be6d


### BigQuery to Slack

https://towardsdatascience.com/slack-alerts-from-a-sql-query-on-bigquery-f626b767304c

### Querying BigQuery with Google Analytics data

https://digitalmarketinglikeapro.medium.com/hands-on-experience-with-bigquery-how-to-query-with-google-analytics-data-b83e7cbdd3c9

### JFrog

https://cloud.google.com/blog/products/bigquery/how-google-cloud-bigquery-enables-big-devops-at-jfrog


### Policygenius

https://medium.com/policygenius-stories/building-a-data-warehouse-on-google-cloud-platform-that-scales-with-the-business-2b07f7c7292e

### Protobuf to BigQuery converter

https://medium.com/sardineai/open-sourcing-protobuf-to-bigquery-converter-c9168046b36b

### Retrieve BigQuery history

https://towardsdev.com/retrieve-your-bigquery-query-history-with-nodejs-sdk-6671dc5be503

### Data versioning

https://medium.com/codex/collaborate-better-with-data-versioning-566c2299c435


### BigQuery validator

https://conalldalydev.medium.com/why-i-built-the-python-bigquery-validator-package-3f2b32e9bc5b

### UNNEST

https://medium.com/@Marshall.Sansano.Roma/unnest-the-first-bigquery-function-for-ga4-the-e-commerce-tracking-82e687409b50

### BigQuery Cool SQL features

https://blog.devgenius.io/cool-bigquery-features-using-standard-sql-syntax-e7a47ef9b72e

### GeoJSON

https://cloud.google.com/blog/topics/developers-practitioners/using-geojson-bigquery-geospatial-analytics

### Covid 19 data Insights 

https://chriskyfung.github.io/blog/qwiklabs/Insights-from-Data-with-BigQuery-Challenge-Lab

### Steampipe

https://briansuk.medium.com/connecting-steampipe-with-google-bigquery-ae37f258090f

### ArcGIS and BigQuery


https://cloud.google.com/blog/products/data-analytics/use-bigquery-with-esri-arcgis-to-power-your-geospatial-analysis

### Plotting bar chars in BigQuery using SQL UDF

https://towardsdatascience.com/plotting-bar-charts-in-bigquery-using-a-sql-user-defined-function-udf-ca6056aac680


### Evaluate arithmetic expressions without values using BigQuery

https://blog.devgenius.io/evaluate-arithmetic-expressions-without-values-using-bigquery-a4abd99f0932

### Predicting Conversion Events from Google Analytics Dataset for Google Merchandise Store in BigQuery

https://towardsdatascience.com/predicting-conversion-events-from-google-analytics-dataset-for-google-merchandise-store-in-bigquery-a9cfb3b6087e


### Open source insights public data

https://cloud.google.com/blog/products/identity-security/announcing-open-source-insights-data-in-bigquery


### transferring Google analytics data to bigquery 

https://medium.com/google-cloud/google-analytics-data-transfer-to-bigquery-fad388ae646a


### Replicate Oracle data to BigQuery

https://cloud.google.com/blog/products/data-analytics/how-twitter-modernized-its-data-processing-with-google-cloud

### Connect Oracle to BigQuery using DB Link
https://medium.com/google-cloud/connect-oracle-to-bigquery-using-db-link-6f2040336a47

### Zoominfo

https://cloud.google.com/blog/products/data-analytics/gain-access-to-comprehensive-b2b-data-in-bigquery-with-zoominfo

### Raw GA4 data in BigQuery

https://datadice.medium.com/raw-google-analytics-4-ga4-data-in-bigquery-bq-9cb776ce1f3d

### Measuring string similarity using UDF implementation of Levenshtein distance
https://towardsdatascience.com/measuring-string-similarity-in-bigquery-using-sql-33c490638c89

### Median, Mode and Average in SQL

https://towardsdatascience.com/median-mode-and-average-order-value-in-bigquery-using-sql-8952bfbc288a

### Streaming JSON messages using dataflow into BigQuery JSON-type column
https://medium.com/google-cloud/streaming-json-messages-into-bigquery-json-type-column-7b9702a49a36

### Processing data from Hive to BigQuery using PySpark and Dataproc Serverless
https://medium.com/google-cloud/processing-data-from-hive-to-bigquery-using-pyspark-and-dataproc-serverless-217c7cb9e4f8

## Qwiklabs


https://www.qwiklabs.com/quests/69



[Build and Optimize Data Warehouses with BigQuery](https://www.qwiklabs.com/quests/147)



[BigQuery for Machine Learning](https://www.qwiklabs.com/quests/71)


[BigQuery for Data Warehousing](https://www.qwiklabs.com/quests/68)


[Insights from Data with BigQuery](https://www.qwiklabs.com/quests/123)


[Create ML Models with BigQuery ML](https://www.qwiklabs.com/quests/146)


 
[NCAA?? March Madness??: Bracketology with Google Cloud](https://www.qwiklabs.com/quests/58)


[Scientific Data Processing](https://www.qwiklabs.com/quests/28)


[Analyzing Natality Data Using AI Platform and BigQuery](https://google.qwiklabs.com/focuses/604?parent=catalog)



[Weather data in BigQuery](https://google.qwiklabs.com/focuses/609?parent=catalog)
