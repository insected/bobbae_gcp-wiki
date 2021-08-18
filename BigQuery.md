


[BigQuery](https://cloud.google.com/bigquery/docs)  is Google Cloud's [fully managed](https://www.youtube.com/watch?v=kKBnFsNWwYM), petabyte-scale, and  analytics [data warehouse](https://cloud.google.com/solutions/bigquery-data-warehouse)  that lets you run [analytics over vast amounts](https://cloud.google.com/blog/topics/developers-practitioners/bigquery-explained-blog-series)  of data in near real time. 

## Quickstart

https://cloud.google.com/bigquery/docs/quickstarts/quickstart-command-line


## BigQuery tutorials

[https://cloud.google.com/bigquery/docs/tutorials](https://cloud.google.com/bigquery/docs/tutorials)


### Basics

https://blog.coupler.io/bigquery-tutorial/

## Architecture




BigQuery has a [distributed architecture](https://cloud.google.com/blog/products/data-analytics/new-blog-series-bigquery-explained-overview) running on thousands of nodes across Google's data centers. Your datasets are not stored in a unique server but are chunked and replicated across different regions.

The [storage and compute layers are fully decoupled](https://cloud.google.com/blog/products/bigquery/separation-of-storage-and-compute-in-bigquery) in BigQuery. This means that the query engine runs on different servers from the servers where the data is stored. This feature enables BigQuery to provide great scalability both in terms of data volume and query execution. This decoupled paradigm is only possible thanks to [Google's Petabit network](https://cloud.google.com/blog/products/networking/google-cloud-networking-in-depth-how-andromeda-2-2-enables-high-throughput-vms), which moves data very quickly from one server to another, leveraging Google's proprietary fiber cables across the globe.

Unlike traditional data warehouses, BigQuery stores data in [columnar format](https://towardsdatascience.com/want-to-use-bigquery-read-this-fab36822830) rather than in row format. This approach enables you to do the following:

- Achieve a better compression ratio for each column, because the data in a column is typically homogeneous and simpler to compress.
- Reduce the amount of data to read and get the best possible performance for data warehouse use cases that are usually based on a small selection of columns in a table and aggregating operations such as sums, average, and maximum.

All the data is stored in Google's proprietary distributed filesystem named [Google File System](https://cloud.google.com/blog/products/storage-data-transfer/a-peek-behind-colossus-googles-file-system) (codename Colossus). The distribution of the data allows it to guarantee faster I/O performance and better availability of data in the case of failures.



[Google File System](https://pierrezemb.fr/posts/colossus-google/) is based on two different server types:

- Master servers: Nodes that don't store data but are responsible for managing the metadata of each file, such as the location and available number of replicas of each chunk that compose a file.
- Chunk servers: Nodes that actually store the chunks of files that are replicated across different servers.


Fully [decoupled from storage](https://medium.com/@raigonjolly/separation-of-storage-and-compute-in-bigquery-7a0084c7cbe0), the [compute layer](https://research.google/pubs/pub43438/) is responsible for receiving query statements from BigQuery users and executing them in the fastest way. The query engine is based on Dremel, a technology developed by Google and then published in a paper in 2010. This engine leverages a multi-level tree architecture:

- The root node of the tree receives the query to execute.
- The root node splits and distributes the query to other intermediate nodes named mixers.
- Mixer nodes have the task of rewriting queries before passing them to the leaf nodes or to other intermediate mixer nodes.
- Leaf nodes are responsible for parallelizing the reading of the chunks of data from Google File System.
- When the right chunks of data are extracted from the filesystem, leaf nodes perform computations on the data and eventually shuffle them across other leaf nodes.
- At the end of the computation, each leaf node produces a result that is returned to the parent node.
When all the results are returned to the root node, the outcome of the query is sent to the user or application that requested the execution.


Each node provides a number of processing units called [BigQuery slots](https://cloud.google.com/bigquery/docs/slots) to execute the business logic of the query. A BigQuery slot can be considered a virtual CPU on a Dremel node. The calculation of the slots needed to perform a specific query is automatically managed depending on the complexity of the query and impacted data volumes.

https://panoply.io/data-warehouse-guide/bigquery-architecture/

## No Index

Each time BigQuery executes a query, it executes [a full-column scan](https://towardsdatascience.com/want-to-use-bigquery-read-this-fab36822830). BigQuery doesn't use or support indexes. Because BigQuery performance and query costs are based on the amount of data scanned during a query, design your queries so that they reference only the columns that are relevant to the query. When using date-partitioned tables, ensure only the relevant partitions are scanned. You can achieve this by using partition filters based on PARTITIONTIME or PARTITIONDATE.

https://cloud.google.com/files/BigQueryTechnicalWP.pdf

https://cloud.google.com/bigquery/docs/querying-partitioned-tables

https://github.com/jorwalk/data-engineering-gcp/blob/master/know/bigquery/best-practices-performance-input.md

https://cloud.google.com/architecture/bigquery-data-warehouse#query_optimization

## Data Types

https://cloud.google.com/bigquery/docs/reference/standard-sql/data-types

## Query Syntax

https://cloud.google.com/bigquery/docs/reference/standard-sql/query-syntax

## Query Plan

To understand the performance characteristics after a query executes, take a look at the detailed query plan explanation. The explanation breaks down the stages that the query went through, the number of input/output rows handled at each stage, and the timing profile within each stage. Using the results from the explanation can help you understand and optimize your queries.


https://cloud.google.com/blog/topics/developers-practitioners/bigquery-admin-reference-guide-query-processing

## Managed

With BigQuery, there's no infrastructure to set up or manage, letting you [focus on finding insights](https://cloudblog.withgoogle.com/products/data-analytics/new-blog-series-bigquery-explained-overview/) using standard SQL and taking advantage of flexible pricing models across on-demand and flat-rate options.

## Wide Column Storage

[BigQuery](https://www.youtube.com/watch?v=sUcInkIqClI&list=PL6oqHwbsfYMwAC5cedqFSCQwaO_gBoYf8&index=1)  is designed to [ingest and store](https://www.youtube.com/watch?v=d3MDxC_iuaw) large amounts of data, and make that data accessible for fast, [large-scale analytics](https://www.youtube.com/watch?v=JLXLCv5nUCE&list=PLIivdWyY5sqIZLeLzyg1B-Pd1MIOo6d-g) - to help analysts and developers alike. BigQuery [stores data in wide columns](https://www.youtube.com/watch?v=1gYUGv_omJA) which are in separate files that are compressed and work well with distributed systems like [Colossus](https://cloud.google.com/blog/products/storage-data-transfer/a-peek-behind-colossus-googles-file-system). 


https://cloud.google.com/blog/topics/developers-practitioners/bigquery-admin-reference-guide-storage

## In-Memory Shuffling

BigQuery is a data warehouse that uses [dynamic query planning](https://cloud.google.com/bigquery/query-plan-explanation) and different shards using in-memory shuffling for optimal distributed performance.

[This document](https://cloud.google.com/bigquery/docs/clustered-tables) provides an overview of table clustering capabilities in BigQuery which allow for [better partitioning and performance](https://www.youtube.com/watch?v=1gYUGv_omJA).


## Loading Data

Learn [how to load](https://www.youtube.com/watch?v=Abzj-Vyhi74) CSV data in batch, and analyze your own data in BigQuery.

## Peta Bytes

[BigQuery](https://www.youtube.com/watch?v=ZVgt1-LfWW4) is [fully managed](https://www.youtube.com/watch?v=7bW7P-8SJ_4&list=PLIivdWyY5sqIF17nHLuY3_XkFjrqb54Hw&index=1) and lets you search through terabytes of data in seconds. It’s also cost effective: you can store gigabytes, terabytes, or even [petabytes of data](https://www.youtube.com/watch?v=qqbYrQGSibQ).

## BigQuery Data Transfer Service

You can [upload data](https://cloud.google.com/bigquery/docs/batch-loading-data?skip_cache=true) files from local sources, Google Drive, or Cloud Storage buckets, take advantage of [BigQuery Data Transfer Service](https://cloud.google.com/bigquery-transfer/docs/introduction?skip_cache=true) (DTS), [Cloud Data Fusion](Data-Fusion) plug-ins, or leverage Google's industry-leading [data integration partnerships](https://cloud.google.com/bigquery?skip_cache=true#section-12). You have ultimate flexibility in how you bring data into your data warehouse. 




## Anatomy of a BigQuery query

Google [BigQuery](https://cloud.google.com/blog/products/gcp/bigquery-under-the-hood) is a lightning-fast analytics database. Customers find BigQuery performance liberating, allowing them to experiment with enormous datasets without compromise. But how fast is BigQuery really? And what does it take to achieve BigQuery speeds? Let’s check out the [publically-available bigquery-samples:wikipedia_benchmark](https://console.cloud.google.com/bigquery?project=publicdata&page=table&t=wikipedia&d=samples&p=publicdata), specifically the Wiki100B table. This table contains 100 billion rows and is about 7 Terabytes in size.

You can see that this query runs in under 30 seconds, but let’s round up to 30. It’s quite impressive, since to churn through this much data, BigQuery has had to:

- Read about 1TB of data, then uncompress it to 4TB (assuming ~4:1 compression)
- Execute 100 billion regular expressions with 3 wildcards each
- Distribute 1.25TB of data across the network (1TB compressed for initial read, and 0.25TB for the aggregation)
- Let’s assume for a second that all distributed analytics engines take the same amount of resources to process a query and that queries are perfectly parallelizable.

That’s a lot of resources! So it’s quite impressive that BigQuery lets you use all this stuff for just the few seconds required for your job to complete. But what’s even more impressive is that we do not know this is happening — we simply press “Run Query” and BigQuery takes care of the rest automagically. BigQuery entirely hides the complexity of large-scale analytics technologies.

[https://cloud.google.com/blog/products/gcp/anatomy-of-a-bigquery-query](https://cloud.google.com/blog/products/gcp/anatomy-of-a-bigquery-query)

## In memory query execution

BigQuery is a fast petabyte-scale analytics database. To achieve that level of performance, BigQuery executes queries completely in memory. Most databases and data processing systems achieve scalability using hybrid executors that operate on both disk and memory. Meanwhile, BigQuery’s execution engine builds simple and purely in-memory operators and achieves petabyte-scale analytics through scalable data repartitioning, or "shuffle." This post takes a closer look at BigQuery shuffle, and how it enables high performance, in-memory query execution by leveraging Google’s petabit-scale networking technologies, such as Jupiter.

[Shuffle](https://cloud.google.com/blog/products/bigquery/in-memory-query-execution-in-google-bigquery) is a key ingredient in any distributed data processing system, from Hadoop and Spark to Google Cloud Dataflow. The shuffle step is required for execution of large and complex joins, aggregations and analytic operations. For example, MapReduce uses the shuffle step as a mechanism to redistribute data between the "map" and "reduce" steps based on mapped keys. To support large-scale computation, shuffled data is transiently stored on remote servers. This enables separation of "map" and "reduce" phases and is a key principle in supporting large-scale data processing. The shuffle step is notoriously slow — Hadoop engineers joke that MapReduce should really be called small Map, huge Shuffle, and small Reduce.

[[https://storage.googleapis.com/gweb-cloudblog-publish/images/in-memory-query-2ntao.max-700x700.PNG]]

The variety of BigQuery query characteristics and requirements called for rethinking of the shuffle step. In 2014, BigQuery shuffle migrated to a newly developed infrastructure that's memory-based (with support for disk spooling) and specifically designed for Google data center networking technology. Moreover, it's designed as a flexible data delivery system with use cases beyond specific distributed operations, for example hash joins. This project culminated a multi-year research and development effort on data transfer technologies.

[In-memory BigQuery shuffle](https://cloud.google.com/blog/products/gcp/in-memory-query-execution-in-google-bigquery) stores intermediate data produced from various stages of query processing in a set of nodes that are dedicated to hosting remote memory. Persisting the intermediate results of a data processing job is common in many systems, such as Spark (in the form of RDDs) or Piccolo (in the form of distributed hash sets). However, BigQuery takes a different direction with respect to in-memory intermediate results in a form that's tightly integrated with shuffle operations.






## Query plan and timeline


When BigQuery executes a query job, it converts the declarative SQL statement into a graph of execution, broken up into a [series of query stages](https://cloud.google.com/bigquery/query-plan-explanation), which themselves are composed of more granular sets of execution steps. BigQuery leverages a heavily distributed parallel architecture to run these queries. Stages model the units of work that many potential workers may execute in parallel. Stages communicate with one another by using a fast distributed shuffle architecture, which you can read about at In-memory query execution in BigQuery.

Within the [query plan](https://cloud.google.com/bigquery/query-plan-explanation), the terms work units and workers are used to convey information specifically about parallelism. Elsewhere within BigQuery, you may encounter the term slot", which is an abstracted representation of multiple facets of query execution, including compute, memory, and I/O resources. Top level job statistics provide the estimate of individual query cost using the totalSlotMs estimate of the query using this abstracted accounting.

## Point in time recovery

https://cloud.google.com/spanner/docs/pitr


## Managing input data and data sources

When [evaluating](https://cloud.google.com/bigquery/docs/best-practices-performance-input) your input data, consider the required I/O. How many bytes does your query read? Are you properly limiting the amount of input data? Is your data in native BigQuery storage or an external data source? The amount of data read by a query and the source of the data impact query performance and cost.




## Optimizing communication between slots

When evaluating your [communication](https://cloud.google.com/bigquery/docs/best-practices-performance-communication) throughput, consider the amount of shuffling that is required by your query. How many bytes are passed between stages? How many bytes are passed to each slot? For example, a GROUP BY clause passes like values to the same slot for processing. The amount of data that is shuffled directly impacts communication throughput and as a result, query performance.




## Optimizing query computation

When evaluating the computation that is required by a query, consider the [amount of work](https://cloud.google.com/bigquery/docs/best-practices-performance-compute) that is required. How much CPU time is required? Are you using functions like JavaScript user-defined functions that require additional CPU resources?




## Managing materialization and outputs

When evaluating your output data, consider the number of bytes written by your query. How many bytes are written for your result set? Are you properly limiting the amount of data written? Are you repeatedly writing the same data? The amount of data written by a query impacts query performance (I/O). If you are writing results to a permanent (destination) table, the amount of data written also has a cost.




## Anti patterns

Avoid [query anti-patterns](https://cloud.google.com/bigquery/docs/best-practices-performance-patterns) that impact performance in BigQuery.

## Managing partitioned tables

A partitioned table is a special table that is divided into segments, called partitions, that make it easier to manage and query your data. By dividing a large table into smaller partitions, you can improve query performance, and you can control costs by reducing the number of bytes read by a query.


You can partition BigQuery tables by:

- Time-unit column: Tables are partitioned based on a TIMESTAMP, DATE, or DATETIME column in the table.
- Ingestion time: Tables are partitioned based on the timestamp when BigQuery ingests the data.
- Integer range: Tables are partitioned based on an integer column.

If a query filters on the value of the partitioning column, BigQuery can scan the partitions that match the filter and skip the remaining partitions. This process is called pruning.


https://cloud.google.com/bigquery/docs/managing-partitioned-tables


### Using datasets

A dataset is contained within a specific project. Datasets are top-level containers that are used to organize and control access to your tables and views. A table or view must belong to a dataset, so you need to create at least one dataset before loading data into BigQuery.

https://cloud.google.com/bigquery/docs/reference/standard-sql/query-syntax

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

### Using partitioned tables

A partitioned table is a special table that is divided into segments, called partitions, that make it easier to manage and query your data. By dividing a large table into smaller partitions, you can improve query performance, and you can control costs by reducing the number of bytes read by a query.

You can partition BigQuery tables by:

- Time-unit column: Tables are partitioned based on a TIMESTAMP, DATE, or DATETIME column in the table.
- Ingestion time: Tables are partitioned based on the timestamp when BigQuery ingests the data.
- Integer range: Tables are partitioned based on an integer column.



### Clustered tables

When you create a clustered table in BigQuery, the table data is automatically organized based on the contents of one or more columns in the table’s schema. The columns you specify are used to colocate related data. When you cluster a table using multiple columns, the order of columns you specify is important. The order of the specified columns determines the sort order of the data.

Clustering can improve the performance of certain types of queries such as queries that use filter clauses and queries that aggregate data. When data is written to a clustered table by a query job or a load job, BigQuery sorts the data using the values in the clustering columns. These values are used to organize the data into multiple blocks in BigQuery storage. When you submit a query that contains a clause that filters data based on the clustering columns, BigQuery uses the sorted blocks to eliminate scans of unnecessary data. You might not see a significant difference in query performance between a clustered and unclustered table if the table or partition is under 1 GB.


https://cloud.google.com/bigquery/docs/clustered-tables


### Paritioning vs. clustering

Both partitioning and clustering can improve performance and reduce query cost.  Use clustering when you don't need strict cost guarantees before running the query.  Use partitioning when you want to know query costs before a query runs.  You may prefer cluster over partitioning when partitioning results in a small amount of data per partition approximately less than  1GB.

https://cloud.google.com/bigquery/docs/partitioned-tables#partitioning_versus_clustering

### Views

A view is a virtual table defined by a SQL query. When you create a view, you query it in the same way you query a table. When a user queries the view, the query results contain data only from the tables and fields specified in the query that defines the view.

https://cloud.google.com/bigquery/docs/views-intro

### Materialized Views

In BigQuery, materialized views are precomputed views that periodically cache the results of a query for increased performance and efficiency. BigQuery leverages precomputed results from materialized views and whenever possible reads only delta changes from the base table to compute up-to-date results. Materialized views can be queried directly or can be used by the BigQuery optimizer to process queries to the base tables.

Queries that use materialized views are generally faster and consume fewer resources than queries that retrieve the same data only from the base table. Materialized views can significantly improve the performance of workloads that have the characteristic of common and repeated queries.


https://cloud.google.com/bigquery/docs/materialized-views-intro

### Reservations


BigQuery Reservations enables you to switch between on-demand pricing and flat-rate pricing. With flat-rate pricing, you purchase dedicated query processing capacity. You can allocate this capacity across your organization, by reserving pools of capacity for different projects or different parts of your organization. You can also combine the two billing models, taking advantage of both on-demand and flat-rate pricing.

https://cloud.google.com/bigquery/docs/reservations-intro


https://cloud.google.com/blog/topics/developers-practitioners/bigquery-admin-reference-guide-jobs-reservation-model

### Controlling costs

https://cloud.google.com/bigquery/docs/controlling-costs

#### Optimizing BigQuery Cost with Looker

https://cloud.google.com/blog/topics/developers-practitioners/optimizing-your-google-cloud-spend-bigquery-and-looker





### Organizing BigQuery resources

Resource Hierarchy.

https://cloud.google.com/bigquery/docs/resource-hierarchy


## Dremel

[Dremel](https://research.google/pubs/pub36632/) is a scalable, interactive ad-hoc query system for analysis of read-only nested data. BigQuery is based on Dremel.

https://www.wired.com/2012/08/googles-dremel-makes-big-data-look-small/

https://titanwolf.org/Network/Articles/Article?AID=ae877f35-2dd6-49f7-9679-47d465de1f7f#gsc.tab=0

http://www.goldsborough.me/distributed-systems/2019/05/18/21-09-00-a_look_at_dremel/

## INFORMATIN_SCHEMA

https://cloud.google.com/bigquery/docs/information-schema-intro


## Denormalize whenever possible

https://cloud.google.com/bigquery/docs/best-practices-performance-input#denormalize_data_whenever_possible


## Building the world’s largest data warehouse

[https://www.youtube.com/watch?v=1gYUGv_omJA](https://www.youtube.com/watch?v=1gYUGv_omJA)



## BigQuery nested and repeated fields

[https://www.youtube.com/watch?v=STo98QUKDS8](https://www.youtube.com/watch?v=STo98QUKDS8)


## Learn writing java code to connect Dataproc map/reduce to BigQuery

[https://cloud.google.com/dataproc/docs/tutorials/bigquery-connector-mapreduce-example](https://cloud.google.com/dataproc/docs/tutorials/bigquery-connector-mapreduce-example)



## BigQuery connector to Spark

[https://cloud.google.com/dataproc/docs/tutorials/bigquery-connector-spark-example](https://cloud.google.com/dataproc/docs/tutorials/bigquery-connector-spark-example)


## Data Warehouse Topics


### BigQuery, Snowflake and Redshift

[Compare](https://medium.com/2359media/redshift-vs-bigquery-vs-snowflake-a-comparison-of-the-most-popular-data-warehouse-for-data-driven-cb1c10ac8555) and [review](https://www.youtube.com/watch?v=XpaN-PqSczM
) various Data Warehousing solutions: BigQuery, [Snowflake](https://0x0fff.com/snowflake-the-good-the-bad-and-the-ugly/) and [RedShift](https://aws.amazon.com/redshift/).



### Snowflake, Star, Galaxy

Star Schema in a data warehouse, in which the center of the star can have one fact table and a number of associated dimension tables. It is known as star schema as its structure resembles a star. The Star Schema data model is the simplest type of Data Warehouse schema. It is also known as Star Join Schema and is optimized for querying large data sets.

Snowflake Schema in a data warehouse is a logical arrangement of tables in a multidimensional database such that the [ER diagram](https://www.guru99.com/er-diagram-tutorial-dbms.html) resembles a snowflake shape. A Snowflake Schema is an extension of a Star Schema, and it adds additional dimensions. The dimension tables are normalized which splits data into additional tables.

A Galaxy Schema contains two fact table that share dimension tables between them. It is also called Fact Constellation Schema. The schema is viewed as a collection of stars hence the name Galaxy Schema.

[https://www.guru99.com/star-snowflake-data-warehousing.html](https://www.guru99.com/star-snowflake-data-warehousing.html)


### Denormalization

[Denormalization](https://en.wikipedia.org/wiki/Denormalization) is a strategy used on a previously-normalized database to increase performance. In computing, denormalization is the process of trying to improve the read performance of a database, at the expense of losing some write performance, by adding redundant copies of data or by grouping data.

### Transactions

https://cloud.google.com/bigquery/docs/reference/standard-sql/transactions


## Public Datasets

[https://cloud.google.com/bigquery/public-data](https://cloud.google.com/bigquery/public-data)


## BigQuery Standard SQL

BigQuery supports two different SQL dialects: standard SQL and legacy SQL. Legacy SQL may be useful if you want to test queries coming from legacy applications.

https://cloud.google.com/blog/topics/developers-practitioners/bigquery-explained-querying-your-data

BigQuery was developed as an internal product within Google and was initially realized to process log records. The query engine Dremel was able to support a limited set of SQL operations that are now defined as Legacy SQL.

[https://cloud.google.com/bigquery/docs/reference/standard-sql/migrating-from-legacy-sql](https://cloud.google.com/bigquery/docs/reference/standard-sql/migrating-from-legacy-sql)


### Newer features in BigQuery SQL

https://cloud.google.com/blog/topics/developers-practitioners/spring-forward-bigquery-user-friendly-sql

https://cloud.google.com/blog/topics/developers-practitioners/shine-user-friendly-sql-bigquery



## BigQuery BI Engine 

[BigQuery BI Engine](https://cloud.google.com/bi-engine/docs) is a fast, in-memory analysis service that allows you to analyze data stored in BigQuery. 




## Data Security and Governance

Data governance is a principled approach to manage data during its lifecycle — from acquisition, to use, to disposal. Your data governance program clearly outlines policies, procedures, responsibilities, and controls surrounding data activities. This program helps to ensure that information is collected, maintained, used, and disseminated in such a way that both meets your organization's data integrity and [security](security) needs, and also helps empower your employees to discover and use the data to its fullest potential.


https://cloud.google.com/bigquery/docs/data-governance

### BigQuery Column-level security

[https://cloud.google.com/blog/products/data-analytics/data-governance-new-ways-to-securely-access-and-discover-data](https://cloud.google.com/blog/products/data-analytics/data-governance-new-ways-to-securely-access-and-discover-data)

## Using Connected Sheets with BigQuery

With Connected Sheets, you can access, analyze, visualize, and share billions of rows of BigQuery data from your Sheets spreadsheet.

You can also do the following:

- Collaborate with partners, analysts, or other stakeholders in a familiar spreadsheet interface.
- Ensure a single source of truth for data analysis without additional spreadsheet exports.
- Streamline your reporting and dashboard workflows.



https://cloud.google.com/bigquery/docs/connected-sheets

## Pricing

BigQuery is a [serverless](Serverless) data analytics platform. You don't need to provision individual instances or virtual machines to use BigQuery. Instead, BigQuery automatically allocates computing resources as you need them. You can also reserve compute capacity ahead of time in the form of slots, which represent virtual CPUs. The pricing structure of BigQuery reflects this design.

BigQuery pricing has two main components:

- Analysis pricing is the cost to process queries, including SQL queries, user-defined functions, scripts, and certain data manipulation language (DML) and data definition language (DDL) statements that scan tables.

- Storage pricing is the cost to store data that you load into BigQuery.


https://cloud.google.com/bigquery/pricing

### BigQuery Flex Slots

https://cloud.google.com/blog/products/data-analytics/introducing-bigquery-flex-slots

### Flat rate

https://cloud.google.com/bigquery/pricing#flat_rate_pricing

## Sandbox

https://cloud.google.com/bigquery/docs/sandbox

## Tutorials

https://cloud.google.com/bigquery/docs/tutorials

### Authorize and Share access views

https://cloud.google.com/bigquery/docs/share-access-views

### Using BigQuery GIS to plot a hurricane's path

https://cloud.google.com/bigquery/docs/gis-tutorial-hurricane

### Visualize BigQuery data in Jupyter notebook

https://cloud.google.com/bigquery/docs/visualize-jupyter



## Looker and BigQuery

[Looker](Looker) is an enterprise platform for business intelligence, data applications, and embedded analytics. Looker helps you explore, share, and visualize your company's data so that you can make better business decisions.


https://cloud.google.com/bigquery/docs/looker

## Sync data from MySQL to BigQuery

https://blog.fourninecloud.com/how-to-sync-data-from-mysql-to-bigquery-9ef980ef602c

## Three ways to query in Python

https://towardsdatascience.com/3-ways-to-query-bigquery-in-python-66838f45cb43

## Genomics Analytics with BigQuery

https://cloud.google.com/blog/products/data-analytics/genomics-data-analytics-with-cloud-pt2

## BigQuery GIS 

[BigQuery GIS](https://cloud.google.com/bigquery/docs/gis-intro) uniquely combines the serverless architecture of BigQuery with native support for geospatial analysis, so you can augment your analytics workflows with location intelligence. 


### BigQuery GIS tutorial

https://cloud.google.com/bigquery/docs/gis-tutorial-hurricane


## BigQuery Omni

[BigQuery Omni](https://cloud.google.com/blog/products/data-analytics/introducing-bigquery-omni) is a flexible, fully managed, multicloud analytics solution that allows you to analyze data across clouds such as AWS and Azure. 



## BigQuery ML 

[BigQuery ML](BigQuery-ML) enables users to create and execute machine learning models in BigQuery by using SQL queries.



## Qwiklabs


[BigQuery Basics for Data Analysts](https://www.qwiklabs.com/quests/69?catalog_rank=%7B%22rank%22%3A8%2C%22num_filters%22%3A1%2C%22has_search%22%3Atrue%7D&search_id=7467580)

[BigQuery challenge on Covid-19 public data sources](https://www.qwiklabs.com/focuses/14341?parent=catalog)


[Build and Optimize Data Warehouses with BigQuery](https://www.qwiklabs.com/quests/147?catalog_rank=%7B%22rank%22%3A1%2C%22num_filters%22%3A1%2C%22has_search%22%3Atrue%7D&search_id=7467580)


[BigQuery for Marketing Analysts](https://www.qwiklabs.com/quests/70?catalog_rank=%7B%22rank%22%3A2%2C%22num_filters%22%3A1%2C%22has_search%22%3Atrue%7D&search_id=7467580)


[BigQuery for Machine Learning](https://www.qwiklabs.com/quests/71?catalog_rank=%7B%22rank%22%3A3%2C%22num_filters%22%3A1%2C%22has_search%22%3Atrue%7D&search_id=7467580)


[BigQuery for Data Warehousing](https://www.qwiklabs.com/quests/68?catalog_rank=%7B%22rank%22%3A4%2C%22num_filters%22%3A1%2C%22has_search%22%3Atrue%7D&search_id=7467580)


[Insights from Data with BigQuery](https://www.qwiklabs.com/quests/123?catalog_rank=%7B%22rank%22%3A5%2C%22num_filters%22%3A1%2C%22has_search%22%3Atrue%7D&search_id=7467580)


[Create ML Models with BigQuery ML](https://www.qwiklabs.com/quests/146?catalog_rank=%7B%22rank%22%3A7%2C%22num_filters%22%3A1%2C%22has_search%22%3Atrue%7D&search_id=7467580)


 
[NCAA® March Madness®: Bracketology with Google Cloud](https://www.qwiklabs.com/quests/58?catalog_rank=%7B%22rank%22%3A9%2C%22num_filters%22%3A1%2C%22has_search%22%3Atrue%7D&search_id=7467580)


[Scientific Data Processing](https://www.qwiklabs.com/quests/28?catalog_rank=%7B%22rank%22%3A1%2C%22num_filters%22%3A1%2C%22has_search%22%3Atrue%7D&search_id=7467566)


[Analyzing Natality Data Using AI Platform and BigQuery](https://google.qwiklabs.com/focuses/604?parent=catalog)



[Weather data in BigQuery](https://google.qwiklabs.com/focuses/609?parent=catalog)
