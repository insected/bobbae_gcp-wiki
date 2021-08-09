Cloud [Bigtable](https://cloud.google.com/bigtable/docs)  is Google's [NoSQL Big Data database](https://research.google.com/archive/bigtable-osdi06.pdf
)  service. It's the same [database that powers many core Google services](https://www.youtube.com/watch?v=KaRbKdMInuc
), including Search, Analytics, Maps, and Gmail.


## Overview

https://cloud.google.com/bigtable/docs/overview


## Quickstart

https://cloud.google.com/bigtable/docs/quickstart-cbt

## Scalable Key-value store

Bigtable is a compressed, high performance, proprietary data storage system built on Google File System, Chubby Lock Service, [SSTable](https://etcnotes.com/posts/sstable-and-lsm/) (log-structured storage like LevelDB) and a few other Google technologies. On May 6, 2015, a public version of Bigtable was made available as a service. Bigtable also underlies Google Cloud Datastore, which is available as a part of the Google Cloud Platform.

[https://cloud.google.com/bigtable/docs](https://cloud.google.com/bigtable/docs)

## History and Usage

Bigtable development began in 2004 and is now used by a number of Google applications, such as web indexing, MapReduce, which is often used for generating and modifying data stored in Bigtable, Google Maps, Google Book Search, "My Search History", Google Earth, Blogger.com, Google Code hosting, YouTube, and Gmail. Google's reasons for developing its own database include scalability and better control of performance characteristics.

https://www.youtube.com/watch?v=Lq9uDOM4whI

## Architecture

<img src="https://cloud.google.com/bigtable/img/bigtable-architecture.svg" width="600">

Bigtable is one of the prototypical examples of a wide column store. It maps two arbitrary string values (row key and column key) and timestamp (hence three-dimensional mapping) into an associated arbitrary byte array. It is not a relational database and can be better defined as a sparse, distributed multi-dimensional sorted map.

Bigtable is designed to scale into the petabyte range across "hundreds or thousands of machines, and to make it easy to add more machines  the system and automatically start taking advantage of those resources without any reconfiguration".

For example, Google's copy of the web can be stored in a bigtable where the row key is a domain-reversed URL, and columns describe various properties of a web page, with one particular column holding the page itself. The page column can have several timestamped versions describing different copies of the web page timestamped by when they were fetched. Each cell of a bigtable can have zero or more timestamped versions of the data. Another function of the timestamp is to allow for both versioning and garbage collection of expired data.





Cloud Bigtable is a sparsely populated table that can scale to billions of rows and thousands of columns, enabling you to store terabytes or even petabytes of data. A single value in each row is indexed; this value is known as the row key. Bigtable is ideal for storing very large amounts of single-keyed data with very low latency. It supports high read and write throughput at low latency, and it is an ideal data source for MapReduce operations.

Bigtable is exposed to applications through multiple client libraries, including a supported extension to the [Apache HBase](https://hbase.apache.org/) library for Java. As a result, it integrates with the existing Apache ecosystem of open-source Big Data software.

Bigtable's powerful back-end servers offer several key advantages over a self-managed HBase installation.

## Incredible scalability

Bigtable scales in direct proportion to the number of machines in your cluster. A self-managed HBase installation has a design bottleneck that limits the performance after a certain threshold is reached. Bigtable does not have this bottleneck, so you can scale your cluster up to handle more reads and writes.

## Simple administration

Bigtable handles upgrades and restarts transparently, and it automatically maintains high data durability. To replicate your data, simply add a second cluster to your instance, and replication starts automatically. No more managing replicas or regions; just design your table schemas, and Bigtable will handle the rest for you.


## Cluster resizing without downtime

You can increase the size of a Bigtable cluster for a few hours to handle a large load, then reduce the cluster's size again—all without any downtime. After you change a cluster's size, it typically takes just a few minutes under load for Bigtable to balance performance across all of the nodes in your cluster.


## What it's good for

Bigtable is ideal for applications that need very high throughput and scalability for key/value data, where each value is typically no larger than 10 MB. Bigtable also excels as a storage engine for batch MapReduce operations, stream processing/analytics, and machine-learning applications.

You can use Bigtable to store and query all of the following types of data:

* Time-series data, such as CPU and memory usage over time for multiple servers.
* Marketing data, such as purchase histories and customer preferences.
* Financial data, such as transaction histories, stock prices, and currency exchange rates.
* Internet of Things data, such as usage reports from energy meters and home appliances.
* Graph data, such as information about how users are connected to one another.

## Bigtable storage model

Bigtable stores data in massively scalable tables, each of which is a sorted key/value map. The table is composed of rows, each of which typically describes a single entity, and columns, which contain individual values for each row. Each row is indexed by a single row key, and columns that are related to one another are typically grouped together into a column family. Each column is identified by a combination of the column family and a column qualifier, which is a unique name within the column family.


Tables are split into multiple tablets – segments of the table are split at certain row keys so that each tablet is a few hundred megabytes or a few gigabytes in size. 

When Table size threaten to grow beyond a specified limit, the tablets may be compressed using the algorithm BMDiff and the Zippy compression algorithm publicly known and open-sourced as Snappy, which is a less space-optimal variation of LZ77 but more efficient in terms of computing time. 

The locations in the GFS of tablets are recorded as database entries in multiple special tablets, which are called "META1" tablets. META1 tablets are found by querying the single "META0" tablet, which typically resides on a server of its own since it is often queried by clients as to the location of the "META1" tablet which itself has the answer to the question of where the actual data is located. Like GFS's master server, the META0 server is not generally a bottleneck since the processor time and bandwidth necessary to discover and transmit META1 locations is minimal and clients aggressively cache locations to minimize queries.



## Schema design

[Designing a Bigtable schema]( https://cloud.google.com/bigtable/docs/schema-design  ) is different than designing a schema for a relational database. In Bigtable, a schema is a blueprint or model of a table, including the structure of the following table components:

- Row keys
- Column families, including their garbage-collection policies
- Columns


## Schema for time series data

A time series is a collection of data that consists of measurements and the times when the measurements are recorded.

There are [different schema design patterns]( https://cloud.google.com/bigtable/docs/keyvis-overview  ) for storing time series data in Cloud Bigtable.




## Key Visualizer


[Key Visualizer]( https://cloud.google.com/bigtable/docs/keyvis-overview ) is a tool that helps you analyze your Bigtable usage patterns. It generates visual reports for your tables that break down your usage based on the row keys that you access.


## Cassandra and Cloud Bigtable

Why and how Spotify migrated some of their workloads, and how they built an auto-scaler for Cloud Bigtable.

[https://www.youtube.com/watch?v=Hfd3VZOYXNU](https://www.youtube.com/watch?v=Hfd3VZOYXNU)

## Global Data Services with Bigtable

[https://www.youtube.com/watch?v=dHr707_6woY](https://www.youtube.com/watch?v=dHr707_6woY)

## Bigtable and Spanner

[https://www.youtube.com/watch?v=_Qm0eopwjG0](https://www.youtube.com/watch?v=_Qm0eopwjG0)

## Bigtable emulator

https://cloud.google.com/bigtable/docs/emulator

## Music Recommendation

https://www.youtube.com/watch?v=807uHC0Ia10

## HBase

This page lists differences between Bigtable and HBase. 

[https://cloud.google.com/bigtable/docs/hbase-differences](https://cloud.google.com/bigtable/docs/hbase-differences)



https://codelabs.developers.google.com/codelabs/cloud-bigtable-intro-java/index.html#0



## SSTable, LSM Tree, LevelDB

[https://www.igvita.com/2012/02/06/sstable-and-log-structured-storage-leveldb/](https://www.igvita.com/2012/02/06/sstable-and-log-structured-storage-leveldb/)

https://etcnotes.com/posts/sstable-and-lsm/

## Querying from BigQuery

https://cloud.google.com/bigquery/external-data-bigtable


## HBase tutorial

https://www.guru99.com/hbase-tutorials.html

## Qwiklabs




[Bigtable: Qwik Start - Hbase Shell](https://www.qwiklabs.com/focuses/580?catalog_rank=%7B%22rank%22%3A1%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&parent=catalog&search_id=7500925)






[Bigtable: Qwik Start - Command Line](https://www.qwiklabs.com/focuses/579?catalog_rank=%7B%22rank%22%3A1%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&parent=catalog&search_id=7467646)


[Using OpenTSDB to Monitor Time-Series Data on Cloud Platform](https://www.qwiklabs.com/focuses/629?catalog_rank=%7B%22rank%22%3A3%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&parent=catalog&search_id=7467646)



[Tracking Cryptocurrency Exchange Trades with Google Cloud Platform in Real-Time](https://www.qwiklabs.com/focuses/5570?catalog_rank=%7B%22rank%22%3A8%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&parent=catalog&search_id=7467646)
