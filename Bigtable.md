


## Introduction

Cloud Bigtable is Google's NoSQL Big Data database service. It's the same database that powers many core Google services, including Search, Analytics, Maps, and Gmail.

https://www.youtube.com/watch?v=KaRbKdMInuc

[https://cloud.google.com/bigtable/docs](https://cloud.google.com/bigtable/docs)

https://www.youtube.com/watch?v=Lq9uDOM4whI

Handle massive amounts of data workload with Cloud Bigtable.

[https://www.youtube.com/watch?v=MzT0c0l3RPc](https://www.youtube.com/watch?v=MzT0c0l3RPc)

Discuss the differences between Cassandra and Cloud Bigtable, why and how Spotify migrated some of their workloads, and how they built an auto-scaler for Cloud Bigtable.

[https://www.youtube.com/watch?v=Hfd3VZOYXNU](https://www.youtube.com/watch?v=Hfd3VZOYXNU)

## Global Data Services with Bigtable

[https://www.youtube.com/watch?v=dHr707_6woY](https://www.youtube.com/watch?v=dHr707_6woY)

## Bigtable and Spanner

[https://www.youtube.com/watch?v=_Qm0eopwjG0](https://www.youtube.com/watch?v=_Qm0eopwjG0)


## HBase

This page lists differences between Bigtable and HBase. 

[https://cloud.google.com/bigtable/docs/hbase-differences](https://cloud.google.com/bigtable/docs/hbase-differences)


## SSTable, LSM Tree, LevelDB

[https://www.igvita.com/2012/02/06/sstable-and-log-structured-storage-leveldb/](https://www.igvita.com/2012/02/06/sstable-and-log-structured-storage-leveldb/)

## Moving from Cassandra to Bigtable

https://www.youtube.com/watch?v=Hfd3VZOYXNU

## Qwiklabs


### Hbase

One way to communicate with Cloud Bigtable is through the Cloud Bigtable HBase client for Java, which is a customized version of the [Apache HBase](https://hbase.apache.org/) client. The Cloud Bigtable HBase client for Java enables you to write Java applications that communicate with Cloud Bigtable through the open-source [HBase API](https://hbase.apache.org/apidocs/). The client is compatible with versions 1.0.x, 1.1.x, 1.2.x, and 1.3.x of the HBase API.

[Bigtable: Qwik Start - Hbase Shell](https://www.qwiklabs.com/focuses/580?catalog_rank=%7B%22rank%22%3A1%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&parent=catalog&search_id=7500925)


##### Bigtable

Cloud Bigtable is a sparsely populated table that can scale to billions of rows and thousands of columns, enabling you to store terabytes or even petabytes of data. A single value in each row is indexed; this value is known as the row key. Cloud Bigtable is ideal for storing very large amounts of single-keyed data with very low latency. It supports high read and write throughput at low latency, and it is an ideal data source for MapReduce operations.

Cloud Bigtable is exposed to applications through multiple client libraries, including a supported extension to the [Apache HBase library for Java](https://hbase.apache.org/). As a result, it integrates with the existing Apache ecosystem of open-source Big Data software.

[Intro to Bigtable](https://cloud.google.com/bigtable/docs) 


### Cloud Bigtable Command line

In this lab you'll learn how to use the cbt command line to connect to a Cloud Bigtable instance, perform basic administrative tasks, and read and write data in a table.

[Bigtable: Qwik Start - Command Line](https://www.qwiklabs.com/focuses/579?catalog_rank=%7B%22rank%22%3A1%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&parent=catalog&search_id=7467646)


### OpenTSDB

In this lab you will learn how to collect, record, and monitor [time-series data](https://en.wikipedia.org/wiki/Time_series) on Google Cloud using [OpenTSDB](http://opentsdb.net/) running on [Google Kubernetes Engine](https://cloud.google.com/kubernetes-engine/) and [Cloud Bigtable](https://cloud.google.com/bigtable/).

[Using OpenTSDB to Monitor Time-Series Data on Cloud Platform](https://www.qwiklabs.com/focuses/629?catalog_rank=%7B%22rank%22%3A3%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&parent=catalog&search_id=7467646)


### Cryptocurrency Trading 

Currently, using an [econometric](https://www.investopedia.com/terms/e/econometrics.asp) approach—applying models to financial data to forecast future trends—doesn’t work for real-time financial predictions. And data that’s old, inaccurate or from a single source doesn’t translate into dependable data for financial institutions to use. But building pipelines with Google Cloud Platform (GCP) can solve some of these key challenges. In this lab, we’ll describe how to build a pipeline to predict financial trends in microseconds. We’ll walk through how to set up and configure a pipeline for ingesting real-time, time-series data from various financial exchanges and how to design a suitable data model, which facilitates querying and graphing at scale.

[Tracking Cryptocurrency Exchange Trades with Google Cloud Platform in Real-Time](https://www.qwiklabs.com/focuses/5570?catalog_rank=%7B%22rank%22%3A8%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&parent=catalog&search_id=7467646)
