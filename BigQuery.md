
<img src="https://storage.googleapis.com/gweb-cloudblog-publish/images/BQ_Explained_2.max-900x900.jpg" width="600">


[BigQuery](https://cloud.google.com/bigquery/docs)  is Google Cloud's [fully managed](https://www.youtube.com/watch?v=kKBnFsNWwYM), petabyte-scale, and cost-effective analytics [data warehouse](https://cloud.google.com/solutions/bigquery-data-warehouse)  that lets you run [analytics over vast amounts](https://cloud.google.com/blog/topics/developers-practitioners/bigquery-explained-blog-series)  of data in near real time. 

With BigQuery, there's no infrastructure to set up or manage, letting you [focus on finding meaningful insights](https://cloudblog.withgoogle.com/products/data-analytics/new-blog-series-bigquery-explained-overview/) using standard SQL and taking advantage of flexible pricing models across on-demand and flat-rate options.

[BigQuery](https://www.youtube.com/watch?v=sUcInkIqClI&list=PL6oqHwbsfYMwAC5cedqFSCQwaO_gBoYf8&index=1)  is designed to [ingest and store](https://www.youtube.com/watch?v=d3MDxC_iuaw) large amounts of data, and make that data accessible for fast, [large-scale analytics](https://www.youtube.com/watch?v=JLXLCv5nUCE&list=PLIivdWyY5sqIZLeLzyg1B-Pd1MIOo6d-g) - to help analysts and developers alike. BigQuery stores data in columns which are in separate files that are compressed and work well with distributed systems like Colossus.

<img src="https://s3.amazonaws.com/files.dezyre.com/images/blog/Impala+vs+Hive/Columnar+Storage+Technology+in+Impala.png" width="500">

Learn [how to load](https://www.youtube.com/watch?v=Abzj-Vyhi74) CSV data in batch, and analyze your own data in BigQuery.

Most experienced data analysts and programmers already have the skills to get started. [BigQuery](https://www.youtube.com/watch?v=ZVgt1-LfWW4) is [fully managed](https://www.youtube.com/watch?v=7bW7P-8SJ_4&list=PLIivdWyY5sqIF17nHLuY3_XkFjrqb54Hw&index=1) and lets you search through terabytes of data in seconds. It’s also cost effective: you can store gigabytes, terabytes, or even [petabytes of data](https://www.youtube.com/watch?v=qqbYrQGSibQ).

## Loading Data into BigQuery

You can [upload data](https://cloud.google.com/bigquery/docs/batch-loading-data?skip_cache=true) files from local sources, Google Drive, or Cloud Storage buckets, take advantage of [BigQuery Data Transfer Service](https://cloud.google.com/bigquery-transfer/docs/introduction?skip_cache=true) (DTS), [Data Fusion](https://cloud.google.com/data-fusion/plugins?skip_cache=true) plug-ins, or leverage Google's industry-leading [data integration partnerships](https://cloud.google.com/bigquery?skip_cache=true#section-12). You have ultimate flexibility in how you bring data into your data warehouse. 



<img src="https://cloudx-bricks-prod-bucket.storage.googleapis.com/7347fa6a31d8e2242e6483befbdb6d3fdc617824352b5bf9f7b52de12a23d3ec.svg" width="600">


## Anatomy of a BigQuery query

Google [BigQuery](https://cloud.google.com/blog/products/gcp/bigquery-under-the-hood) is a lightning-fast analytics database. Customers find BigQuery performance liberating, allowing them to experiment with enormous datasets without compromise. But how fast is BigQuery really? And what does it take to achieve BigQuery speeds? Let’s check out the publically-available bigquery-samples:wikipedia_benchmark, specifically the Wiki100B table. This table contains 100 billion rows and is about 7 Terabytes in size.

You can see that this query runs in under 30 seconds, but let’s round up to 30. It’s quite impressive, since to churn through this much data, BigQuery has had to:

- Read about 1TB of data, then uncompress it to 4TB (assuming ~4:1 compression)
- Execute 100 billion regular expressions with 3 wildcards each
- Distribute 1.25TB of data across the network (1TB compressed for initial read, and 0.25TB for the aggregation)
- Let’s assume for a second that all distributed analytics engines take the same amount of resources to process a query and that queries are perfectly parallelizable.

That’s a lot of resources! So it’s quite impressive that BigQuery lets you use all this stuff for just the few seconds required for your job to complete.
But what’s even more impressive is that we do not know this is happening — we simply press “Run Query” and BigQuery takes care of the rest automagically. BigQuery entirely hides the complexity of large-scale analytics technologies.

[https://cloud.google.com/blog/products/gcp/anatomy-of-a-bigquery-query](https://cloud.google.com/blog/products/gcp/anatomy-of-a-bigquery-query)

## In memory query execution

BigQuery is a fast petabyte-scale analytics database. To achieve that level of performance, BigQuery executes queries completely in memory. Most databases and data processing systems achieve scalability using hybrid executors that operate on both disk and memory. Meanwhile, BigQuery’s execution engine builds simple and purely in-memory operators and achieves petabyte-scale analytics through scalable data repartitioning, or "shuffle." This post takes a closer look at BigQuery shuffle, and how it enables high performance, in-memory query execution by leveraging Google’s petabit-scale networking technologies, such as Jupiter.

Shuffle is a key ingredient in any distributed data processing system, from Hadoop and Spark to Google Cloud Dataflow. The shuffle step is required for execution of large and complex joins, aggregations and analytic operations. For example, MapReduce uses the shuffle step as a mechanism to redistribute data between the "map" and "reduce" steps based on mapped keys. To support large-scale computation, shuffled data is transiently stored on remote servers. This enables separation of "map" and "reduce" phases and is a key principle in supporting large-scale data processing. The shuffle step is notoriously slow — Hadoop engineers joke that MapReduce should really be called small Map, huge Shuffle, and small Reduce.

[[https://storage.googleapis.com/gweb-cloudblog-publish/images/in-memory-query-2ntao.max-700x700.PNG]]

The variety of BigQuery query characteristics and requirements called for rethinking of the shuffle step. In 2014, BigQuery shuffle migrated to a newly developed infrastructure that's memory-based (with support for disk spooling) and specifically designed for Google data center networking technology. Moreover, it's designed as a flexible data delivery system with use cases beyond specific distributed operations, for example hash joins. This project culminated a multi-year research and development effort on data transfer technologies.

[In-memory BigQuery shuffle](https://cloud.google.com/blog/products/gcp/in-memory-query-execution-in-google-bigquery) stores intermediate data produced from various stages of query processing in a set of nodes that are dedicated to hosting remote memory. Persisting the intermediate results of a data processing job is common in many systems, such as Spark (in the form of RDDs) or Piccolo (in the form of distributed hash sets). However, BigQuery takes a different direction with respect to in-memory intermediate results in a form that's tightly integrated with shuffle operations.






## Query plan and timeline


When BigQuery executes a query job, it converts the declarative SQL statement into a graph of execution, broken up into a series of query stages, which themselves are composed of more granular sets of execution steps. BigQuery leverages a heavily distributed parallel architecture to run these queries. Stages model the units of work that many potential workers may execute in parallel. Stages communicate with one another by using a fast distributed shuffle architecture, which you can read about at In-memory query execution in BigQuery.

Within the [query plan](https://cloud.google.com/bigquery/query-plan-explanation), the terms work units and workers are used to convey information specifically about parallelism. Elsewhere within BigQuery, you may encounter the term slot", which is an abstracted representation of multiple facets of query execution, including compute, memory, and I/O resources. Top level job statistics provide the estimate of individual query cost using the totalSlotMs estimate of the query using this abstracted accounting.



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




## Dremel

[Dremel](https://research.google/pubs/pub36632/) is a scalable, interactive ad-hoc query system for analysis of read-only nested data. BigQuery is based on Dremel.



<img src="https://panoply.io/uploads/bigquery-architecture-1.png" width="500">




## Building the world’s largest data warehouse

[https://www.youtube.com/watch?v=1gYUGv_omJA](https://www.youtube.com/watch?v=1gYUGv_omJA)



## BigQuery nested and repeated fields

[https://www.youtube.com/watch?v=STo98QUKDS8](https://www.youtube.com/watch?v=STo98QUKDS8)


## BigQuery tutorials

[https://cloud.google.com/bigquery/docs/tutorials](https://cloud.google.com/bigquery/docs/tutorials)


## Learn writing java code to connect Dataproc map/reduce to BigQuery

[https://cloud.google.com/dataproc/docs/tutorials/bigquery-connector-mapreduce-example](https://cloud.google.com/dataproc/docs/tutorials/bigquery-connector-mapreduce-example)



## BigQuery connector to Spark

[https://cloud.google.com/dataproc/docs/tutorials/bigquery-connector-spark-example](https://cloud.google.com/dataproc/docs/tutorials/bigquery-connector-spark-example)


## Data Warehouse Topics


### BigQuery, [Snowflake](https://0x0fff.com/snowflake-the-good-the-bad-and-the-ugly/), [Redshift](https://aws.amazon.com/redshift/?whats-new-cards.sort-by=item.additionalFields.postDateTime&whats-new-cards.sort-order=desc)


[https://medium.com/2359media/redshift-vs-bigquery-vs-snowflake-a-comparison-of-the-most-popular-data-warehouse-for-data-driven-cb1c10ac8555](https://medium.com/2359media/redshift-vs-bigquery-vs-snowflake-a-comparison-of-the-most-popular-data-warehouse-for-data-driven-cb1c10ac8555)


https://www.youtube.com/watch?v=XpaN-PqSczM

### Snowflake, Star, Galaxy

Star Schema in a data warehouse, in which the center of the star can have one fact table and a number of associated dimension tables. It is known as star schema as its structure resembles a star. The Star Schema data model is the simplest type of Data Warehouse schema. It is also known as Star Join Schema and is optimized for querying large data sets.

Snowflake Schema in a data warehouse is a logical arrangement of tables in a multidimensional database such that the [ER diagram](https://www.guru99.com/er-diagram-tutorial-dbms.html) resembles a snowflake shape. A Snowflake Schema is an extension of a Star Schema, and it adds additional dimensions. The dimension tables are normalized which splits data into additional tables.

A Galaxy Schema contains two fact table that share dimension tables between them. It is also called Fact Constellation Schema. The schema is viewed as a collection of stars hence the name Galaxy Schema.

[https://www.guru99.com/star-snowflake-data-warehousing.html](https://www.guru99.com/star-snowflake-data-warehousing.html)


### Denormalization

[Denormalization](https://en.wikipedia.org/wiki/Denormalization) is a strategy used on a previously-normalized database to increase performance. In computing, denormalization is the process of trying to improve the read performance of a database, at the expense of losing some write performance, by adding redundant copies of data or by grouping data.




## Public Datasets

[https://cloud.google.com/bigquery/public-data](https://cloud.google.com/bigquery/public-data)


## BigQuery Standard SQL

[https://cloud.google.com/bigquery/docs/reference/standard-sql/migrating-from-legacy-sql](https://cloud.google.com/bigquery/docs/reference/standard-sql/migrating-from-legacy-sql)


## Qwiklabs


### Data Analysts

BigQuery uses SQL and can take advantage of the pay-as-you-go model. BigQuery allows you to focus on analyzing data to find meaningful insights.

[BigQuery Basics for Data Analysts](https://www.qwiklabs.com/quests/69?catalog_rank=%7B%22rank%22%3A8%2C%22num_filters%22%3A1%2C%22has_search%22%3Atrue%7D&search_id=7467580)

GSP340

A favorite BigQuery challenge on Covid-19 public data sources

[https://www.qwiklabs.com/focuses/14341?parent=catalog](https://www.qwiklabs.com/focuses/14341?parent=catalog)


### Data Warehousing

Looking to build or optimize your data warehouse? Learn best practices to Extract, Transform, and Load your data into Google Cloud with BigQuery. 

[Build and Optimize Data Warehouses with BigQuery](https://www.qwiklabs.com/quests/147?catalog_rank=%7B%22rank%22%3A1%2C%22num_filters%22%3A1%2C%22has_search%22%3Atrue%7D&search_id=7467580)


### Marketing Analysts

Want to turn your marketing data into insights and build dashboards? Bring all of your data into one place for large-scale analysis and model building.

[BigQuery for Marketing Analysts](https://www.qwiklabs.com/quests/70?catalog_rank=%7B%22rank%22%3A2%2C%22num_filters%22%3A1%2C%22has_search%22%3Atrue%7D&search_id=7467580)


### Machine Learning

Want to learn and practice machine learning and build models in minutes instead of hours using just SQL? BigQuery Machine Learning is a new feature in BigQuery where data analysts can create, train, evaluate, and predict machine learning models with minimal coding. In this series of labs you will experiment with different model types and learn what makes a good model.

[BigQuery for Machine Learning](https://www.qwiklabs.com/quests/71?catalog_rank=%7B%22rank%22%3A3%2C%22num_filters%22%3A1%2C%22has_search%22%3Atrue%7D&search_id=7467580)


### Data Warehousing Optimization

In this series of interactive labs you will create and optimize your own data warehouse using a variety of large-scale BigQuery public datasets. 

[BigQuery for Data Warehousing](https://www.qwiklabs.com/quests/68?catalog_rank=%7B%22rank%22%3A4%2C%22num_filters%22%3A1%2C%22has_search%22%3Atrue%7D&search_id=7467580)


### Insights from Data

Learn the best practices for querying and getting insights from your data warehouse with this interactive series of BigQuery labs. 

A favorite lab.

[Insights from Data with BigQuery](https://www.qwiklabs.com/quests/123?catalog_rank=%7B%22rank%22%3A5%2C%22num_filters%22%3A1%2C%22has_search%22%3Atrue%7D&search_id=7467580)


### Create ML Models

Want to build ML models in minutes instead of hours using just SQL? BigQuery ML democratizes machine learning by letting data analysts create, train, evaluate, and predict with machine learning models using existing SQL tools and skills. 

[Create ML Models with BigQuery ML](https://www.qwiklabs.com/quests/146?catalog_rank=%7B%22rank%22%3A7%2C%22num_filters%22%3A1%2C%22has_search%22%3Atrue%7D&search_id=7467580)


### March Madness

In this series of labs you will learn how to use BigQuery to analyze NCAA basketball data with SQL. Build a Machine Learning Model to predict the outcomes of NCAA March Madness basketball tournament games.

 
[NCAA® March Madness®: Bracketology with Google Cloud](https://www.qwiklabs.com/quests/58?catalog_rank=%7B%22rank%22%3A9%2C%22num_filters%22%3A1%2C%22has_search%22%3Atrue%7D&search_id=7467580)


### Scientific Data Processing

Big data, machine learning, and scientific data? It sounds like the perfect match. In this advanced-level quest, you will get hands-on practice with GCP services like Big Query, Dataproc, and TensorFlow by applying them to use cases that employ real-life, scientific data sets. By getting experience with tasks like earthquake data analysis and satellite image aggregation, Scientific Data Processing will expand your skill set in big data and machine learning so you can start tackling your own problems across a spectrum of scientific disciplines.

[Scientific Data Processing](https://www.qwiklabs.com/quests/28?catalog_rank=%7B%22rank%22%3A1%2C%22num_filters%22%3A1%2C%22has_search%22%3Atrue%7D&search_id=7467566)


### Analyzing Natality Data Using AI Platform and BigQuery

A favorite lab.

This lab illustrates how you can carry out data exploration of large datasets, but continue to use familiar tools like Pandas and Jupyter. The trick is to do the first part of your aggregation in BigQuery, get back a Pandas DataFrame, then work with the smaller Pandas DataFrame locally. AI Platform provides a managed Jupyter experience, so you don't need to run notebook servers yourself.

[https://google.qwiklabs.com/focuses/604?parent=catalog](https://google.qwiklabs.com/focuses/604?parent=catalog)


### Weather data in BigQuery

A favorite lab.

This lab uses two public datasets in BigQuery: weather data from NOAA and citizen complaints data from New York City.  Interestingly, you will find what types of municipal complaints are correlated with weather. For example, you will find (not surprisingly) that complaints about residential furnaces are most common when it is cold outside.

[https://google.qwiklabs.com/focuses/609?parent=catalog](https://google.qwiklabs.com/focuses/609?parent=catalog)
