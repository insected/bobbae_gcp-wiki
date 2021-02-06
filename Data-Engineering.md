- [Data Engineering](#data-engineering)
  * [Overview](#overview)
  * [Database options](#database-options)
  * [Cloud SQL](#cloud-sql)
  * [SQL](#sql)
    + [Tutorials](#tutorials)
  * [Cloud Bigtable](#cloud-bigtable)
    + [Introduction](#introduction)
    + [HBase](#hbase)
    + [SSTable, LSM Tree, LevelDB](#sstable--lsm-tree--leveldb)
    + [Qwiklabs](#qwiklabs)
      - [Hbase](#hbase)
      - [Bigtable](#bigtable)
      - [Cloud Bigtable Command line](#cloud-bigtable-command-line)
      - [OpenTSDB](#opentsdb)
      - [Cryptocurrency Trading](#cryptocurrency-trading)
  * [Cloud Dataproc](#cloud-dataproc)
    + [Introduction](#introduction-1)
    + [Big Data analytics with Dataproc](#big-data-analytics-with-dataproc)
    + [Migrating Hadoop to GCP](#migrating-hadoop-to-gcp)
    + [Basic introduction to Apache Hadoop](#basic-introduction-to-apache-hadoop)
    + [Apache Spark Tutorial](#apache-spark-tutorial)
      - [A Scala tutorial for Java programmers](#a-scala-tutorial-for-java-programmers)
    + [Some online courses to learn Hadoop and Spark.](#some-online-courses-to-learn-hadoop-and-spark)
    + [Using Apache Hive on Cloud Dataproc](#using-apache-hive-on-cloud-dataproc)
    + [Spark by Example](#spark-by-example)
      - [Main Spark github source tree](#main-spark-github-source-tree)
      - [Spark examples source code](#spark-examples-source-code)
    + [Hadoop Data Storage](#hadoop-data-storage)
    + [Hive](#hive)
    + [Pig vs SQL](#pig-vs-sql)
      - [Hadoop Pig](#hadoop-pig)
    + [Pig Latin SQL Challenge](#pig-latin-sql-challenge)
      - [Sawzall](#sawzall)
    + [Qwiklabs](#qwiklabs-1)
      - [Spark Scala Jobs on Dataproc](#spark-scala-jobs-on-dataproc)
      - [Moving from Hadoop to GCP](#moving-from-hadoop-to-gcp)
  * [Cloud Pub/Sub](#cloud-pub-sub)
    + [What is Cloud Pub/Sub](#what-is-cloud-pub-sub)
    + [Example](#example)
    + [A list of task queues](#a-list-of-task-queues)
    + [Kafka](#kafka)
    + [Qwiklabs](#qwiklabs-2)
      - [Cloud Pub/Sub](#cloud-pub-sub-1)
      - [Kafka](#kafka-1)
  * [BigQuery](#bigquery)
    + [Introduction](#introduction-2)
    + [BigQuery 101](#bigquery-101)
      - [Data warehousing with BigQuery](#data-warehousing-with-bigquery)
      - [BigQuery Explained](#bigquery-explained)
    + [BigQuery under the hood](#bigquery-under-the-hood)
      - [Loading Data into BigQuery](#loading-data-into-bigquery)
      - [Anatomy of a BigQuery query](#anatomy-of-a-bigquery-query)
      - [In memory query execution](#in-memory-query-execution)
      - [Query plan and timeline](#query-plan-and-timeline)
      - [Managing input data and data sources](#managing-input-data-and-data-sources)
      - [Optimizing communication between slots](#optimizing-communication-between-slots)
      - [Optimizing query computation](#optimizing-query-computation)
      - [Managing materialization and outputs](#managing-materialization-and-outputs)
      - [Anti patterns](#anti-patterns)
      - [Dremel](#dremel)
      - [Building the world’s largest data warehouse](#building-the-world-s-largest-data-warehouse)
      - [BigQuery nested and repeated fields](#bigquery-nested-and-repeated-fields)
    + [BigQuery tutorials](#bigquery-tutorials)
      - [Learn writing java code to connect Dataproc map/reduce to BigQuery](#learn-writing-java-code-to-connect-dataproc-map-reduce-to-bigquery)
      - [BigQuery connector to Spark](#bigquery-connector-to-spark)
    + [Data Warehouse Topics](#data-warehouse-topics)
      - [BigQuery, Snowflake, Redshift](#bigquery--snowflake--redshift)
      - [Snowflake, Star, Galaxy](#snowflake--star--galaxy)
      - [Denormalization](#denormalization)
    + [Public Datasets](#public-datasets)
    + [BigQuery Standard SQL](#bigquery-standard-sql)
    + [Qwiklabs](#qwiklabs-3)
      - [Data Analysts](#data-analysts)
      - [Data Warehousing](#data-warehousing)
      - [Marketing Analysts](#marketing-analysts)
      - [Machine Learning](#machine-learning)
      - [Data Warehousing Optimization](#data-warehousing-optimization)
      - [Insights from Data](#insights-from-data)
      - [Create ML Models](#create-ml-models)
      - [March Madness](#march-madness)
      - [Scientific Data Processing](#scientific-data-processing)
      - [Analyzing Natality Data Using AI Platform and BigQuery](#analyzing-natality-data-using-ai-platform-and-bigquery)
      - [Weather data in BigQuery](#weather-data-in-bigquery)
  * [Cloud Spanner](#cloud-spanner)
    + [Introduction](#introduction-3)
    + [External Consistency, Linearizability, Serializability](#external-consistency--linearizability--serializability)
    + [TrueTime](#truetime)
    + [Cloud Spanner 101](#cloud-spanner-101)
    + [Tutorials](#tutorials-1)
    + [Perspectives](#perspectives)
    + [Qwiklabs](#qwiklabs-4)
      - [Quick Start](#quick-start)
      - [Java Client](#java-client)
      - [Leaderboard](#leaderboard)
      - [Backend](#backend)
      - [Python](#python)
  * [Cloud Data Fusion](#cloud-data-fusion)
    + [Introduction](#introduction-4)
    + [CDAP](#cdap)
    + [Qwiklab](#qwiklab)
      - [Codeless Pipelines](#codeless-pipelines)
  * [Dataflow](#dataflow)
    + [Introduction](#introduction-5)
    + [Apache beam](#apache-beam)
    + [Example Notebook](#example-notebook)
    + [Word Count Example](#word-count-example)
    + [Dataflow Templates](#dataflow-templates)
    + [Creating a pipeline](#creating-a-pipeline)
    + [Using provided Dataflow templates](#using-provided-dataflow-templates)
    + [Creating Dataflow templates](#creating-dataflow-templates)
    + [Using Dataflow Flex templates](#using-dataflow-flex-templates)
    + [Migrating from App  Engine Map/reduce to Dataflow](#migrating-from-app--engine-map-reduce-to-dataflow)
    + [Dataflow Mobile Gaming Example](#dataflow-mobile-gaming-example)
  * [Cloud Dataprep](#cloud-dataprep)
    + [Introduction](#introduction-6)
    + [Qwiklabs](#qwiklabs-5)
      - [Data Transformation Pipeline](#data-transformation-pipeline)
  * [Cloud Composer](#cloud-composer)
    + [Introduction](#introduction-7)
      - [Data Pipelines with Cloud Composer](#data-pipelines-with-cloud-composer)
      - [Cloud Composer best practices](#cloud-composer-best-practices)
    + [Tutorials](#tutorials-2)
      - [Automating infrastructure using Airflow](#automating-infrastructure-using-airflow)
    + [Apache Airflow](#apache-airflow)
      - [Concepts](#concepts)
      - [Apache Airflow for Beginners.](#apache-airflow-for-beginners)
      - [Developing workflows with Apache Airflow](#developing-workflows-with-apache-airflow)
      - [Operators](#operators)
      - [XCom](#xcom)
      - [Task Orchestration tools: Comparison and Alternatives](#task-orchestration-tools--comparison-and-alternatives)
      - [Industrialization of a Machine Learning model using Apache Airflow and Apache BEAM.](#industrialization-of-a-machine-learning-model-using-apache-airflow-and-apache-beam)
      - [Airflow vs. Luigi vs. Argo vs. MLFlow vs. KubeFlow](#airflow-vs-luigi-vs-argo-vs-mlflow-vs-kubeflow)
  * [Google Data Studio](#google-data-studio)
  * [Datalab](#datalab)
    + [Introduction](#introduction-8)
    + [Datalab Quickstart](#datalab-quickstart)
    + [Working with Notebooks](#working-with-notebooks)
  * [Looker](#looker)
    + [Introduction](#introduction-9)
    + [Getting Started with Looker](#getting-started-with-looker)
    + [Building Reports in Looker](#building-reports-in-looker)
    + [LookML](#lookml)
    + [Looker vs Tableau](#looker-vs-tableau)
    + [Looker, Building Explores:](#looker--building-explores-)
    + [Looker, Dashboards](#looker--dashboards)
    + [Looker API Examples:](#looker-api-examples-)
    + [Recorded Training](#recorded-training)
  * [Data Catalog](#data-catalog)
  * [Cloud Life Sciences](#cloud-life-sciences)
  * [Firestore](#firestore)
    + [Introduction](#introduction-10)
    + [Datastore](#datastore)
  * [Memorystore](#memorystore)
  * [Firebase](#firebase)
    + [Introduction](#introduction-11)
    + [Cloud Storage for Firebase](#cloud-storage-for-firebase)
    + [Firebase Realtime Database](#firebase-realtime-database)
    + [Cloud Firestore or Realtime Database](#cloud-firestore-or-realtime-database)
    + [Firebase Authentication](#firebase-authentication)
    + [Cloud Functions for Firebase](#cloud-functions-for-firebase)
    + [Cloud Storage for Firebase](#cloud-storage-for-firebase-1)
    + [Firebase Test Lab](#firebase-test-lab)
    + [Qwiklabs](#qwiklabs-6)
      - [Build Apps](#build-apps)
      - [Hugo](#hugo)
  * [Choosing Which Database to Use](#choosing-which-database-to-use)

<small><i><a href='http://ecotrust-canada.github.io/markdown-toc/'>Table of contents generated with markdown-toc</a></i></small>


## Data Engineering


### Overview

[https://www.youtube.com/watch?v=tc2940Zwvyk](https://www.youtube.com/watch?v=tc2940Zwvyk)


### Database options

One of Google Cloud Platform's competitive advantages is the strong ecosystem of managed databases.  However, the wealth of options can be confusing to navigate as you look for the right technologies to grow your product.  This is a video about picking the right databases for your tech stack and how to make it all work in a unified way.

[https://www.youtube.com/watch?v=3aHBkfBRFEU](https://www.youtube.com/watch?v=3aHBkfBRFEU)

Choosing the right database for your workloads.

[https://www.youtube.com/watch?v=3YnLuEdGzU8](https://www.youtube.com/watch?v=3YnLuEdGzU8)

Compare different GCP Database services.

[https://cloud.google.com/products/databases](https://cloud.google.com/products/databases)


### Cloud SQL

Cloud SQL is a fully-managed database service that helps you set up, maintain, manage, and administer your relational databases on Google Cloud Platform.

You can use Cloud SQL with [MySQL](https://cloud.google.com/sql/docs/mysql), [PostgreSQL](https://cloud.google.com/sql/docs/postgres), or [SQL Server](https://cloud.google.com/sql/docs/sqlserver). 

[https://cloud.google.com/sql/docs](https://cloud.google.com/sql/docs)

[https://www.youtube.com/watch?v=OvR2KX8GVtU](https://www.youtube.com/watch?v=OvR2KX8GVtU)


### SQL


#### Tutorials

[https://www.youtube.com/watch?v=HXV3zeQKqGY](https://www.youtube.com/watch?v=HXV3zeQKqGY)

[https://www.freecodecamp.org/news/best-sql-database-tutorial/](https://www.freecodecamp.org/news/best-sql-database-tutorial/)


### Cloud Bigtable


#### Introduction

Cloud Bigtable is Google's NoSQL Big Data database service. It's the same database that powers many core Google services, including Search, Analytics, Maps, and Gmail.

[https://cloud.google.com/bigtable/docs](https://cloud.google.com/bigtable/docs)

Handle massive amounts of data workload with Cloud Bigtable.

[https://www.youtube.com/watch?v=MzT0c0l3RPc](https://www.youtube.com/watch?v=MzT0c0l3RPc)

Discuss the differences between Cassandra and Cloud Bigtable, why and how Spotify migrated some of their workloads, and how they built an auto-scaler for Cloud Bigtable.

[https://www.youtube.com/watch?v=Hfd3VZOYXNU](https://www.youtube.com/watch?v=Hfd3VZOYXNU)

Global Data Services with Bigtable.

[https://www.youtube.com/watch?v=dHr707_6woY](https://www.youtube.com/watch?v=dHr707_6woY)

Bigtable and Spanner.

[https://www.youtube.com/watch?v=_Qm0eopwjG0](https://www.youtube.com/watch?v=_Qm0eopwjG0)


#### HBase

This page lists differences between Bigtable and HBase. 

[https://cloud.google.com/bigtable/docs/hbase-differences](https://cloud.google.com/bigtable/docs/hbase-differences)


#### SSTable, LSM Tree, LevelDB

[https://www.igvita.com/2012/02/06/sstable-and-log-structured-storage-leveldb/](https://www.igvita.com/2012/02/06/sstable-and-log-structured-storage-leveldb/)


#### Qwiklabs


##### Hbase

One way to communicate with Cloud Bigtable is through the Cloud Bigtable HBase client for Java, which is a customized version of the [Apache HBase](https://hbase.apache.org/) client. The Cloud Bigtable HBase client for Java enables you to write Java applications that communicate with Cloud Bigtable through the open-source [HBase API](https://hbase.apache.org/apidocs/). The client is compatible with versions 1.0.x, 1.1.x, 1.2.x, and 1.3.x of the HBase API.

[Bigtable: Qwik Start - Hbase Shell](https://www.qwiklabs.com/focuses/580?catalog_rank=%7B%22rank%22%3A1%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&parent=catalog&search_id=7500925)


##### Bigtable

Cloud Bigtable is a sparsely populated table that can scale to billions of rows and thousands of columns, enabling you to store terabytes or even petabytes of data. A single value in each row is indexed; this value is known as the row key. Cloud Bigtable is ideal for storing very large amounts of single-keyed data with very low latency. It supports high read and write throughput at low latency, and it is an ideal data source for MapReduce operations.

Cloud Bigtable is exposed to applications through multiple client libraries, including a supported extension to the [Apache HBase library for Java](https://hbase.apache.org/). As a result, it integrates with the existing Apache ecosystem of open-source Big Data software.

[Intro to Bigtable](https://cloud.google.com/bigtable/docs) 


##### Cloud Bigtable Command line

In this lab you'll learn how to use the cbt command line to connect to a Cloud Bigtable instance, perform basic administrative tasks, and read and write data in a table.

[Bigtable: Qwik Start - Command Line](https://www.qwiklabs.com/focuses/579?catalog_rank=%7B%22rank%22%3A1%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&parent=catalog&search_id=7467646)


##### OpenTSDB

In this lab you will learn how to collect, record, and monitor [time-series data](https://en.wikipedia.org/wiki/Time_series) on Google Cloud using [OpenTSDB](http://opentsdb.net/) running on [Google Kubernetes Engine](https://cloud.google.com/kubernetes-engine/) and [Cloud Bigtable](https://cloud.google.com/bigtable/).

[Using OpenTSDB to Monitor Time-Series Data on Cloud Platform](https://www.qwiklabs.com/focuses/629?catalog_rank=%7B%22rank%22%3A3%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&parent=catalog&search_id=7467646)


##### Cryptocurrency Trading 

Currently, using an [econometric](https://www.investopedia.com/terms/e/econometrics.asp) approach—applying models to financial data to forecast future trends—doesn’t work for real-time financial predictions. And data that’s old, inaccurate or from a single source doesn’t translate into dependable data for financial institutions to use. But building pipelines with Google Cloud Platform (GCP) can solve some of these key challenges. In this lab, we’ll describe how to build a pipeline to predict financial trends in microseconds. We’ll walk through how to set up and configure a pipeline for ingesting real-time, time-series data from various financial exchanges and how to design a suitable data model, which facilitates querying and graphing at scale.

[Tracking Cryptocurrency Exchange Trades with Google Cloud Platform in Real-Time](https://www.qwiklabs.com/focuses/5570?catalog_rank=%7B%22rank%22%3A8%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&parent=catalog&search_id=7467646)


### Cloud Dataproc


#### Introduction

Dataproc is a managed [Apache Spark](https://spark.apache.org/) and [Apache Hadoop](https://hadoop.apache.org/) service that lets you take advantage of open source data tools for batch processing, querying, streaming, and machine learning. Dataproc automation helps you create clusters quickly, manage them easily, and save money by turning clusters off when you don't need them. With less time and money spent on administration, you can focus on your jobs and your data.

[https://cloud.google.com/dataproc/docs](https://cloud.google.com/dataproc/docs)

Enterprises are migrating their existing on-premises Apache Hadoop and Spark clusters over to Dataproc to manage costs and unlock the power of elastic scale. With Dataproc, enterprises get a fully managed, purpose-built cluster that can autoscale to support any data or analytics processing job. 

[https://cloud.google.com/dataproc/docs/tutorials](https://cloud.google.com/dataproc/docs/tutorials)

See how to use Cloud Dataproc to manage Apache Spark and Hadoop in an easy, cost-effective way. Try the Dataproc: Qwik Start lab here:[ http://bit.ly/2KZaZJM](https://www.youtube.com/redirect?q=http%3A%2F%2Fbit.ly%2F2KZaZJM&v=h1LvACJWjKc&redir_token=QUFFLUhqbXk5SU9PTlVJMDY1SHdmOV8zbF92U29rUGFvQXxBQ3Jtc0tsQU1ZZENDa1U4cnVLX3NCeS1wXzFNOEdYVDFueGcybmI5NTBuWWMtUkp2bWd0YUtQTUlfQTdqWGRNZFBNdzhVeGZnb0diUDRSR1RoNk5RTFlWX3FnZ3JJQlA1cHJiWE1HUkhNTmFtM1pDR1ZaSmh6dw%3D%3D&event=video_description)

[https://www.youtube.com/watch?v=h1LvACJWjKc](https://www.youtube.com/watch?v=h1LvACJWjKc)

Run Spark and Hadoop faster with Dataproc.

[https://www.youtube.com/watch?v=h1LvACJWjKc](https://www.youtube.com/watch?v=h1LvACJWjKc)


#### Big Data analytics with Dataproc

[https://programmaticponderings.com/2018/12/11/big-data-analytics-with-java-and-python-using-cloud-dataproc-googles-fully-managed-spark-and-hadoop-service/](https://programmaticponderings.com/2018/12/11/big-data-analytics-with-java-and-python-using-cloud-dataproc-googles-fully-managed-spark-and-hadoop-service/)


#### Migrating Hadoop to GCP

[https://www.youtube.com/watch?v=YK_-yS9y_0k](https://www.youtube.com/watch?v=YK_-yS9y_0k)


#### Basic introduction to Apache Hadoop

[https://www.youtube.com/watch?v=OoEpfb6yga8](https://www.youtube.com/watch?v=OoEpfb6yga8)


#### Apache Spark Tutorial

[https://www.youtube.com/watch?v=IQfG0faDrzE4](https://www.youtube.com/watch?v=IQfG0faDrzE4)  


##### A Scala tutorial for Java programmers

[https://docs.scala-lang.org/tutorials/scala-for-java-programmers.html](https://docs.scala-lang.org/tutorials/scala-for-java-programmers.html)


#### Some online courses to learn Hadoop and Spark.

[https://medium.com/swlh/5-free-online-courses-to-learn-big-data-hadoop-and-spark-in-2019-a553e6ccfe30](https://medium.com/swlh/5-free-online-courses-to-learn-big-data-hadoop-and-spark-in-2019-a553e6ccfe30)


#### Using Apache Hive on Cloud Dataproc

[https://cloud.google.com/solutions/using-apache-hive-on-cloud-dataproc](https://cloud.google.com/solutions/using-apache-hive-on-cloud-dataproc)


#### Spark by Example

[https://sparkbyexamples.com/](https://sparkbyexamples.com/)


##### Main Spark github source tree

[https://github.com/apache/spark](https://github.com/apache/spark)


##### Spark examples source code

[https://github.com/apache/spark/tree/master/examples/src/main](https://github.com/apache/spark/tree/master/examples/src/main)


#### Hadoop Data Storage

Dataproc integrates with Apache Hadoop and the Hadoop Distributed File System (HDFS). 

[https://cloud.google.com/dataproc/docs/concepts/dataproc-hdfs](https://cloud.google.com/dataproc/docs/concepts/dataproc-hdfs)


#### Hive

[Apache Hive](https://hive.apache.org/) is a data warehouse software project built on top of Apache Hadoop for providing data query and analysis. 

[https://www.youtube.com/watch?v=cMziv1iYt28](https://www.youtube.com/watch?v=cMziv1iYt28)


#### Pig vs SQL


##### Hadoop Pig 

[Apache Pig](http://pig.apache.org/) is a platform for analyzing large data sets that consists of a high-level language for expressing data analysis programs, coupled with infrastructure for evaluating these programs.

[https://www.youtube.com/watch?v=Hve24pRW_Ps](https://www.youtube.com/watch?v=Hve24pRW_Ps) \


Hive vs. Pig vs. SQL.

[https://www.whizlabs.com/blog/hive-vs-pig-vs-sql/](https://www.whizlabs.com/blog/hive-vs-pig-vs-sql/)


#### Pig Latin SQL Challenge

Doing ETL in SQL or [Pig Latin](https://pig.apache.org/docs/latest/basic.html) to give more detailed feel for why one might prefer one or the other in solving actual common problems:

[http://www.olric.org/2019/09/pig-latin-sql-challenge-or-window.html?m=1](http://www.olric.org/2019/09/pig-latin-sql-challenge-or-window.html?m=1)


##### Sawzall

A perspective on Sawzall DSL (domain specific language) over Google map/reduce and Pig DSL over Hadoop map/reduce.

[http://glinden.blogspot.com/2007/04/yahoo-pig-and-google-sawzall.html?m=1](http://glinden.blogspot.com/2007/04/yahoo-pig-and-google-sawzall.html?m=1)

And finally a perspective on replacing Sawzell within Google.

[http://www.unofficialgoogledatascience.com/2015/12/replacing-sawzall-case-study-in-domain.html?m=1](http://www.unofficialgoogledatascience.com/2015/12/replacing-sawzall-case-study-in-domain.html?m=1)


#### Qwiklabs


##### Spark Scala Jobs on Dataproc

[Write Spark Scala Jobs (From Spark to DataProc)](https://cloud.google.com/dataproc/docs/tutorials/spark-scala)


##### Moving from Hadoop to GCP

[Hadoop to GCP](https://cloud.google.com/blog/products/data-analytics/goodbye-hadoop-building-a-streaming-data-processing-pipeline-on-google-cloud) 


### Cloud Pub/Sub


#### What is Cloud Pub/Sub

Cloud Pub/Sub is a fully-managed real-time messaging service that allows you to send and receive messages between independent applications.

[https://cloud.google.com/pubsub/docs](https://cloud.google.com/pubsub/docs)

This video walks you through how to create a Google Cloud Pub/Sub topic. Pub/Sub allows you to create global real-time messaging and subscribe to topics you want to follow to stay up to date.

[https://www.youtube.com/watch?v=pU1zA-DMlWk](https://www.youtube.com/watch?v=pU1zA-DMlWk)


#### Example

Cloud IoT Core to push airline data to PubSub, Dataflow, and BigQuery.

[https://www.youtube.com/watch?v=-y3s6XY70Os](https://www.youtube.com/watch?v=-y3s6XY70Os)


#### A list of task queues

[https://taskqueues.com/](https://taskqueues.com/)


#### Kafka

[Apache Kafka](https://kafka.apache.org/) is an open-source distributed event streaming platform used by thousands of companies for high-performance data pipelines, streaming analytics, data integration, and mission-critical applications.

[https://kafka.apache.org/](https://kafka.apache.org/)

Kafka is open source. You can see its implementation: 

[https://github.com/apache/kafka](https://github.com/apache/kafka)

Review some  examples:

[https://github.com/apache/kafka/tree/trunk/examples/src/main/java/kafka/examples](https://github.com/apache/kafka/tree/trunk/examples/src/main/java/kafka/examples)

Using Kafka and Confluent allows customers to integrate legacy systems and Google services like BigQuery and Dataflow in real time. 

[https://www.youtube.com/watch?v=LjF8IqKKbWc](https://www.youtube.com/watch?v=LjF8IqKKbWc)


#### Qwiklabs


##### Cloud Pub/Sub

[Google Cloud Pub/Sub: Qwik Start - Python](https://www.qwiklabs.com/focuses/2775?catalog_rank=%7B%22rank%22%3A4%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&parent=catalog&search_id=7524031)


##### Kafka

Organizations around the world rely on Apache Kafka to integrate existing systems in real time and build a new class of event streaming applications that unlock new business opportunities. Google and Confluent are in a partnership to deliver the best event streaming service based on Apache Kafka and to build event driven applications and big data pipelines on Google Cloud Platform. In this Quest, you will first learn how to deploy and create a streaming data pipeline with Apache Kafka. You will then perform hand-on labs on the different functionalities of the Confluent Platform such as deploying and running Apache Kafka on GKE, building a Cloud Run Streaming Application with Apache Kafka on Anthos or developing a Streaming Microservices Application.

[Getting Started with Apache Kafka and Confluent Platform on Google Cloud](https://www.qwiklabs.com/quests/145?catalog_rank=%7B%22rank%22%3A1%2C%22num_filters%22%3A1%2C%22has_search%22%3Atrue%7D&search_id=7467576)


### BigQuery


#### Introduction

BigQuery is Google Cloud's fully managed, petabyte-scale, and cost-effective analytics data warehouse that lets you run analytics over vast amounts of data in near real time. With BigQuery, there's no infrastructure to set up or manage, letting you focus on finding meaningful insights using standard SQL and taking advantage of flexible pricing models across on-demand and flat-rate options.

[https://www.google.com/amp/s/cloudblog.withgoogle.com/products/data-analytics/new-blog-series-bigquery-explained-overview/amp/](https://www.google.com/amp/s/cloudblog.withgoogle.com/products/data-analytics/new-blog-series-bigquery-explained-overview/amp/)

[https://cloud.google.com/bigquery/docs](https://cloud.google.com/bigquery/docs)

BigQuery is designed to ingest and store large amounts of data, and make that data accessible for fast, large-scale analytics - to help analysts and developers alike. 

[https://www.youtube.com/watch?v=d3MDxC_iuaw](https://www.youtube.com/watch?v=d3MDxC_iuaw)

How to load CSV data in batch, and analyze your own data in BigQuery.

[https://www.youtube.com/watch?v=Abzj-Vyhi74](https://www.youtube.com/watch?v=Abzj-Vyhi74)


#### BigQuery 101

[https://www.youtube.com/watch?v=kKBnFsNWwYM](https://www.youtube.com/watch?v=kKBnFsNWwYM)


##### Data warehousing with BigQuery

[https://cloud.google.com/solutions/bigquery-data-warehouse](https://cloud.google.com/solutions/bigquery-data-warehouse)


##### BigQuery Explained

[https://cloud.google.com/blog/topics/developers-practitioners/bigquery-explained-blog-series](https://cloud.google.com/blog/topics/developers-practitioners/bigquery-explained-blog-series)

[https://www.youtube.com/watch?v=ZVgt1-LfWW4](https://www.youtube.com/watch?v=ZVgt1-LfWW4)

Most experienced data analysts and programmers already have the skills to get started. BigQuery is fully managed and lets you search through terabytes of data in seconds. It’s also cost effective: you can store gigabytes, terabytes, or even petabytes of data.

[https://www.youtube.com/watch?v=qqbYrQGSibQ](https://www.youtube.com/watch?v=qqbYrQGSibQ)


#### BigQuery under the hood

[https://cloud.google.com/blog/products/gcp/bigquery-under-the-hood](https://cloud.google.com/blog/products/gcp/bigquery-under-the-hood)


##### Loading Data into BigQuery

[https://cloud.google.com/bigquery/docs/loading-data](https://cloud.google.com/bigquery/docs/loading-data)


##### Anatomy of a BigQuery query

[https://cloud.google.com/blog/products/gcp/anatomy-of-a-bigquery-query](https://cloud.google.com/blog/products/gcp/anatomy-of-a-bigquery-query)


##### In memory query execution

[https://cloud.google.com/blog/products/gcp/in-memory-query-execution-in-google-bigquery](https://cloud.google.com/blog/products/gcp/in-memory-query-execution-in-google-bigquery)


##### Query plan and timeline

[https://cloud.google.com/bigquery/query-plan-explanation](https://cloud.google.com/bigquery/query-plan-explanation)


##### Managing input data and data sources

[https://cloud.google.com/bigquery/docs/best-practices-performance-input](https://cloud.google.com/bigquery/docs/best-practices-performance-input)


##### Optimizing communication between slots

[https://cloud.google.com/bigquery/docs/best-practices-performance-communication](https://cloud.google.com/bigquery/docs/best-practices-performance-communication)


##### Optimizing query computation

[https://cloud.google.com/bigquery/docs/best-practices-performance-compute](https://cloud.google.com/bigquery/docs/best-practices-performance-compute)


##### Managing materialization and outputs

[https://cloud.google.com/bigquery/docs/best-practices-performance-output](https://cloud.google.com/bigquery/docs/best-practices-performance-output)


##### Anti patterns

[https://cloud.google.com/bigquery/docs/best-practices-performance-patterns](https://cloud.google.com/bigquery/docs/best-practices-performance-patterns)


##### Dremel

Dremel is a scalable, interactive ad-hoc query system for analysis of read-only nested data. BigQuery is based on Dremel.

[https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/36632.pdf](https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/36632.pdf)


##### Building the world’s largest data warehouse

[https://www.youtube.com/watch?v=1gYUGv_omJA](https://www.youtube.com/watch?v=1gYUGv_omJA)


##### BigQuery nested and repeated fields

[https://www.youtube.com/watch?v=STo98QUKDS8](https://www.youtube.com/watch?v=STo98QUKDS8)


#### BigQuery tutorials

[https://cloud.google.com/bigquery/docs/tutorials](https://cloud.google.com/bigquery/docs/tutorials)


##### Learn writing java code to connect Dataproc map/reduce to BigQuery

[https://cloud.google.com/dataproc/docs/tutorials/bigquery-connector-mapreduce-example](https://cloud.google.com/dataproc/docs/tutorials/bigquery-connector-mapreduce-example)


##### BigQuery connector to Spark

[https://cloud.google.com/dataproc/docs/tutorials/bigquery-connector-spark-example](https://cloud.google.com/dataproc/docs/tutorials/bigquery-connector-spark-example)


#### Data Warehouse Topics


##### BigQuery, Snowflake, Redshift

[https://medium.com/2359media/redshift-vs-bigquery-vs-snowflake-a-comparison-of-the-most-popular-data-warehouse-for-data-driven-cb1c10ac8555](https://medium.com/2359media/redshift-vs-bigquery-vs-snowflake-a-comparison-of-the-most-popular-data-warehouse-for-data-driven-cb1c10ac8555)


##### Snowflake, Star, Galaxy

Star Schema in a data warehouse, in which the center of the star can have one fact table and a number of associated dimension tables. It is known as star schema as its structure resembles a star. The Star Schema data model is the simplest type of Data Warehouse schema. It is also known as Star Join Schema and is optimized for querying large data sets.

Snowflake Schema in a data warehouse is a logical arrangement of tables in a multidimensional database such that the [ER diagram](https://www.guru99.com/er-diagram-tutorial-dbms.html) resembles a snowflake shape. A Snowflake Schema is an extension of a Star Schema, and it adds additional dimensions. The dimension tables are normalized which splits data into additional tables.

A Galaxy Schema contains two fact table that share dimension tables between them. It is also called Fact Constellation Schema. The schema is viewed as a collection of stars hence the name Galaxy Schema.

[https://www.guru99.com/star-snowflake-data-warehousing.html](https://www.guru99.com/star-snowflake-data-warehousing.html)


##### Denormalization

[https://en.wikipedia.org/wiki/Denormalization](https://en.wikipedia.org/wiki/Denormalization)


#### Public Datasets

[https://cloud.google.com/bigquery/public-data](https://cloud.google.com/bigquery/public-data)


#### BigQuery Standard SQL

[https://cloud.google.com/bigquery/docs/reference/standard-sql/migrating-from-legacy-sql](https://cloud.google.com/bigquery/docs/reference/standard-sql/migrating-from-legacy-sql)


#### Qwiklabs


##### Data Analysts

BigQuery uses SQL and can take advantage of the pay-as-you-go model. BigQuery allows you to focus on analyzing data to find meaningful insights.

[BigQuery Basics for Data Analysts](https://www.qwiklabs.com/quests/69?catalog_rank=%7B%22rank%22%3A8%2C%22num_filters%22%3A1%2C%22has_search%22%3Atrue%7D&search_id=7467580)

GSP340

A favorite BigQuery challenge on Covid-19 public data sources

[https://www.qwiklabs.com/focuses/14341?parent=catalog](https://www.qwiklabs.com/focuses/14341?parent=catalog)


##### Data Warehousing

Looking to build or optimize your data warehouse? Learn best practices to Extract, Transform, and Load your data into Google Cloud with BigQuery. 

[Build and Optimize Data Warehouses with BigQuery](https://www.qwiklabs.com/quests/147?catalog_rank=%7B%22rank%22%3A1%2C%22num_filters%22%3A1%2C%22has_search%22%3Atrue%7D&search_id=7467580)


##### Marketing Analysts

Want to turn your marketing data into insights and build dashboards? Bring all of your data into one place for large-scale analysis and model building.

[BigQuery for Marketing Analysts](https://www.qwiklabs.com/quests/70?catalog_rank=%7B%22rank%22%3A2%2C%22num_filters%22%3A1%2C%22has_search%22%3Atrue%7D&search_id=7467580)


##### Machine Learning

Want to learn and practice machine learning and build models in minutes instead of hours using just SQL? BigQuery Machine Learning is a new feature in BigQuery where data analysts can create, train, evaluate, and predict machine learning models with minimal coding. In this series of labs you will experiment with different model types and learn what makes a good model.

[BigQuery for Machine Learning](https://www.qwiklabs.com/quests/71?catalog_rank=%7B%22rank%22%3A3%2C%22num_filters%22%3A1%2C%22has_search%22%3Atrue%7D&search_id=7467580)


##### Data Warehousing Optimization

In this series of interactive labs you will create and optimize your own data warehouse using a variety of large-scale BigQuery public datasets. 

[BigQuery for Data Warehousing](https://www.qwiklabs.com/quests/68?catalog_rank=%7B%22rank%22%3A4%2C%22num_filters%22%3A1%2C%22has_search%22%3Atrue%7D&search_id=7467580)


##### Insights from Data

Learn the best practices for querying and getting insights from your data warehouse with this interactive series of BigQuery labs. 

A favorite lab.

[Insights from Data with BigQuery](https://www.qwiklabs.com/quests/123?catalog_rank=%7B%22rank%22%3A5%2C%22num_filters%22%3A1%2C%22has_search%22%3Atrue%7D&search_id=7467580)


##### Create ML Models

Want to build ML models in minutes instead of hours using just SQL? BigQuery ML democratizes machine learning by letting data analysts create, train, evaluate, and predict with machine learning models using existing SQL tools and skills. 

[Create ML Models with BigQuery ML](https://www.qwiklabs.com/quests/146?catalog_rank=%7B%22rank%22%3A7%2C%22num_filters%22%3A1%2C%22has_search%22%3Atrue%7D&search_id=7467580)


##### March Madness

In this series of labs you will learn how to use BigQuery to analyze NCAA basketball data with SQL. Build a Machine Learning Model to predict the outcomes of NCAA March Madness basketball tournament games.

 \
[NCAA® March Madness®: Bracketology with Google Cloud](https://www.qwiklabs.com/quests/58?catalog_rank=%7B%22rank%22%3A9%2C%22num_filters%22%3A1%2C%22has_search%22%3Atrue%7D&search_id=7467580)


##### Scientific Data Processing

Big data, machine learning, and scientific data? It sounds like the perfect match. In this advanced-level quest, you will get hands-on practice with GCP services like Big Query, Dataproc, and TensorFlow by applying them to use cases that employ real-life, scientific data sets. By getting experience with tasks like earthquake data analysis and satellite image aggregation, Scientific Data Processing will expand your skill set in big data and machine learning so you can start tackling your own problems across a spectrum of scientific disciplines.

[Scientific Data Processing](https://www.qwiklabs.com/quests/28?catalog_rank=%7B%22rank%22%3A1%2C%22num_filters%22%3A1%2C%22has_search%22%3Atrue%7D&search_id=7467566)


##### Analyzing Natality Data Using AI Platform and BigQuery

A favorite lab.

This lab illustrates how you can carry out data exploration of large datasets, but continue to use familiar tools like Pandas and Jupyter. The trick is to do the first part of your aggregation in BigQuery, get back a Pandas DataFrame, then work with the smaller Pandas DataFrame locally. AI Platform provides a managed Jupyter experience, so you don't need to run notebook servers yourself.

[https://google.qwiklabs.com/focuses/604?parent=catalog](https://google.qwiklabs.com/focuses/604?parent=catalog)


##### Weather data in BigQuery

A favorite lab.

This lab uses two public datasets in BigQuery: weather data from NOAA and citizen complaints data from New York City.  Interestingly, you will find what types of municipal complaints are correlated with weather. For example, you will find (not surprisingly) that complaints about residential furnaces are most common when it is cold outside.

[https://google.qwiklabs.com/focuses/609?parent=catalog](https://google.qwiklabs.com/focuses/609?parent=catalog)


### Cloud Spanner


#### Introduction 

Cloud Spanner is a fully managed, mission-critical, relational database service that offers transactional consistency at global scale, schemas, SQL (ANSI 2011 with extensions), and automatic, synchronous replication for high availability.

[https://cloud.google.com/spanner/docs](https://cloud.google.com/spanner/docs)

Original paper on Spanner. 

[https://static.googleusercontent.com/media/research.google.com/en//archive/spanner-osdi2012.pdf](https://static.googleusercontent.com/media/research.google.com/en//archive/spanner-osdi2012.pdf)


#### External Consistency, Linearizability, Serializability

Cloud Spanner provides clients with the strictest concurrency-control guarantees for transactions, which is called external consistency. Under external consistency, the system behaves as if all transactions were executed sequentially, even though Cloud Spanner actually runs them across multiple servers (and possibly in multiple datacenters) for higher performance and availability. In addition if one transaction completes before another transaction starts to commit, the system guarantees that clients can never see a state that includes the effect of the second transaction but not the first. Intuitively, Cloud Spanner is semantically indistinguishable from a single-machine database. Even though it provides such strong guarantees, Cloud Spanner enables applications to achieve performance comparable to databases that provide weaker guarantees. 

Cloud Spanner provides external consistency, which is a stronger property than linearizability, because linearizability does not say anything about the behavior of transactions.

Linearizability is a property of concurrent objects that support atomic read and write operations. In a database, an "object" would typically be a single row or even a single cell. External consistency is a property of transaction-processing systems, where clients dynamically synthesize transactions that contain multiple read and write operations on arbitrary objects. Linearizability can be viewed as a special case of external consistency, where a transaction can only contain a single read or write operation on a single object.

Cloud Spanner provides external consistency, which is a stricter property than serializability. A transaction-processing system is serializable if it executes transactions in a manner that is indistinguishable from a system in which the transactions are executed serially. Cloud Spanner also guarantees that the serial order is consistent with the order in which the transactions can be observed to commit.

 In a system that provides serializability but not external consistency, even though the customer executed T1 and then T2 sequentially, the system would be permitted to reorder them, which could cause the debit to incur a penalty due to insufficient funds.


#### TrueTime

TrueTime is a highly available, distributed clock that is provided to applications on all Google servers. TrueTime enables applications to generate monotonically increasing timestamps: an application can compute a timestamp T that is guaranteed to be greater than any timestamp T' if T' finished being generated before T started being generated. This guarantee holds across all servers and all timestamps.

[https://cloud.google.com/spanner/docs/true-time-external-consistency](https://cloud.google.com/spanner/docs/true-time-external-consistency)


#### Cloud Spanner 101

[https://www.youtube.com/watch?v=IfsTINNCooY](https://www.youtube.com/watch?v=IfsTINNCooY)

Cloud Spanner is a fully managed relational database with unlimited scale, strong consistency, and up to 99.999% availability. Cloud Spanner can help you create time-sensitive, mission critical applications at scale. 

[https://www.youtube.com/watch?v=5bjYk6Hhd10](https://www.youtube.com/watch?v=5bjYk6Hhd10)

Build  an inventory ledger solution that streamlines the order-to-shipping process using Cloud Spanner, a scalable, globally consistent database service. The single source of truth enables seamless customer experiences across channels and real-time decisioning at scale. 

[https://www.youtube.com/watch?v=8kj_uA5vJfo](https://www.youtube.com/watch?v=8kj_uA5vJfo)


#### Tutorials

[https://cloud.google.com/spanner/docs/tutorials](https://cloud.google.com/spanner/docs/tutorials)


#### Perspectives

A Shift to Distributed SQL.

[https://medium.com/@garyorenstein/the-shift-to-distributed-sql-232c04dec1f7](https://medium.com/@garyorenstein/the-shift-to-distributed-sql-232c04dec1f7)

Databases, ETL, ELT and tools.

[https://cube.dev/blog/category/data-stack/](https://cube.dev/blog/category/data-stack/)


#### Qwiklabs


##### Quick Start

[Cloud Spanner: Qwik Start](https://www.qwiklabs.com/focuses/1774?catalog_rank=%7B%22rank%22%3A1%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&parent=catalog&search_id=7467628)


##### Java Client

In this lab, you will set up a Cloud Spanner instance, create a database and schema, then run sample queries on a dataset. Helpful Cloud Spanner information is provided along the way to help you get the most out of this powerful database service.

[Querying Cloud Spanner With a Java Client](https://www.qwiklabs.com/focuses/2189?catalog_rank=%7B%22rank%22%3A3%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&parent=catalog&search_id=7467628)


##### Leaderboard

In this lab, you will learn how to set up a Cloud Spanner instance. You will go through the steps of creating a database and schema that can be used for a gaming leaderboard. You'll start by creating a Players table for storing player information and a Scores table to store player scores.

[Cloud Spanner: Create a Gaming Leaderboard with C#](https://www.qwiklabs.com/focuses/1815?catalog_rank=%7B%22rank%22%3A4%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&parent=catalog&search_id=7467628)


##### Backend

In this lab, you develop a backend service for an online Quiz application to process user feedback and save scores.

[App Dev: Developing a Backend Service - Java](https://www.qwiklabs.com/focuses/1128?catalog_rank=%7B%22rank%22%3A9%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&parent=catalog&search_id=7467628)


##### Python

This lab concentrates on the backend service, putting together Pub/Sub, Natural Language, and Spanner services and APIs to collect and analyze feedback and scores from an online Quiz application.

[App Dev: Developing a Backend Service - Python](https://www.qwiklabs.com/focuses/1107?catalog_rank=%7B%22rank%22%3A10%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&parent=catalog&search_id=7467628)


### Cloud Data Fusion


#### Introduction 

Cloud Data Fusion is a fully managed, cloud-native, enterprise data integration service for quickly building and managing data pipelines. Cloud Data Fusion provides a graphical interface to increase time efficiency and reduce complexity. Now business users, developers, and data scientists can easily and reliably build scalable data integration solutions to cleanse, prepare, blend, transfer, and transform data— without having to wrestle with infrastructure.


#### CDAP

Cloud Data Fusion is powered by the open source project [CDAP](https://cdap.io/).

[https://cloud.google.com/data-fusion/docs](https://cloud.google.com/data-fusion/docs)


#### Qwiklab


##### Codeless Pipelines

This fundamental-level Quest offers hands-on practice with Cloud Data Fusion, a cloud-native, code-free, data integration platform. ETL Developers, Data Engineers and Analysts can greatly benefit from the pre-built transformations and connectors to build and deploy their pipelines without worrying about writing code. This Quest starts with a quickstart lab that familiarises learners with the Cloud Data Fusion UI. Learners then get to try running batch and realtime pipelines as well as using the built-in Wrangler plugin to perform some interesting transformations on data.

[Building Codeless Pipelines on Cloud Data Fusion](https://www.qwiklabs.com/quests/130?catalog_rank=%7B%22rank%22%3A4%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&search_id=7467888)


### Dataflow


#### Introduction

Dataflow is a managed service for executing a wide variety of data processing patterns. The documentation on this site shows you how to deploy your batch and streaming data processing pipelines using Dataflow, including directions for using service features.

[https://cloud.google.com/dataflow/docs](https://cloud.google.com/dataflow/docs)

Google Cloud Dataflow makes it easy to process and analyze real-time streaming data so that you can derive insights and react to new information in real-time. Learn how it is used in conjunction with other technologies, like PubSub, Kafka, BigQuery, Bigtable, or Datastore, to build end-to-end streaming architectures. Learn how these architectures enable diverse use cases such as real-time ingestion and ETL, real-time reporting & analytics, real-time alerting, or fraud detection.

[https://www.youtube.com/watch?v=7lJyq1hw_KI](https://www.youtube.com/watch?v=7lJyq1hw_KI)

Google Cloud customers are increasingly looking to leverage streaming data (customer interactions, sales transactions, machine logs) for building new innovative features, increasing sales, and protecting against risks. AI/ML (artificial intelligence/machine learning) technologies make it possible to amp up the detection of insights in large volumes of data: insights that otherwise would be impossible to gain with manual inspection. Learn how Dataflow together with TensorFlow Extended (TFX) and Cloud AI are enabling the extraction of label and classification information from video clips and natural text, predicting probabilities and detecting anomalies, fraud, and patterns in streams of business data.

[https://www.youtube.com/watch?v=cqDBnOaS6O4](https://www.youtube.com/watch?v=cqDBnOaS6O4)


#### Apache beam

The Apache Beam SDK is an open source programming model that enables you to develop both batch and streaming pipelines. You create your pipelines with an Apache Beam program and then run them on the Dataflow service. The [Apache Beam documentation](https://beam.apache.org/documentation/) provides in-depth conceptual information and reference material for the Apache Beam programming model, SDKs, and other runners.

[https://github.com/apache/beam](https://github.com/apache/beam)

[https://beam.apache.org/documentation/programming-guide/](https://beam.apache.org/documentation/programming-guide/)


#### Example Notebook

In this notebook, we set up your development environment and work through a simple example using the [DirectRunner](https://beam.apache.org/documentation/runners/direct/). You can explore other runners with the [Beam Capability Matrix](https://beam.apache.org/documentation/runners/capability-matrix/).

[https://colab.research.google.com/github/apache/beam/blob/master/examples/notebooks/get-started/try-apache-beam-py.ipynb](https://colab.research.google.com/github/apache/beam/blob/master/examples/notebooks/get-started/try-apache-beam-py.ipynb)


#### Word Count Example

[https://beam.apache.org/get-started/wordcount-example/](https://beam.apache.org/get-started/wordcount-example/)


#### Dataflow Templates 

These Dataflow templates are an effort to solve simple, but large, in-Cloud data tasks, including data import/export/backup/restore and bulk API operations, without a development environment. The technology under the hood which makes these operations possible is the [Google Cloud Dataflow](https://cloud.google.com/dataflow/) service combined with a set of [Apache Beam](https://beam.apache.org/) SDK templated pipelines.

[https://github.com/GoogleCloudPlatform/DataflowTemplates](https://github.com/GoogleCloudPlatform/DataflowTemplates)


#### Creating a pipeline

Using the Apache Beam interactive runner with JupyterLab notebooks lets you iteratively develop pipelines, inspect your pipeline graph, and parse individual PCollections in a read-eval-print-loop (REPL) workflow. These Apache Beam notebooks are made available through [AI Platform Notebooks](https://cloud.google.com/ai-platform/notebooks/docs), a managed service that hosts notebook virtual machines pre-installed with the latest data science and machine learning frameworks.

[https://cloud.google.com/dataflow/docs/guides/interactive-pipeline-development](https://cloud.google.com/dataflow/docs/guides/interactive-pipeline-development)


#### Using provided Dataflow templates

Google provides a set of [open-source](https://github.com/GoogleCloudPlatform/DataflowTemplates) Dataflow templates. 

[https://cloud.google.com/dataflow/docs/guides/templates/provided-templates](https://cloud.google.com/dataflow/docs/guides/templates/provided-templates)


#### Creating Dataflow templates

Dataflow [templates](https://cloud.google.com/dataflow/docs/templates/overview) use runtime parameters to accept values that are only available during pipeline execution. To customize the execution of a templated pipeline, you can pass these parameters to functions that run within the pipeline (such as a DoFn).

To create a template from your Apache Beam pipeline, you must modify your pipeline code to support runtime parameters.

[https://cloud.google.com/dataflow/docs/guides/templates/creating-templates](https://cloud.google.com/dataflow/docs/guides/templates/creating-templates)

[https://cloud.google.com/dataflow/docs/guides/templates/running-templates](https://cloud.google.com/dataflow/docs/guides/templates/running-templates)


#### Using Dataflow Flex templates

Dataflow Flex templates use docker containers.

[https://cloud.google.com/dataflow/docs/guides/templates/using-flex-templates#python](https://cloud.google.com/dataflow/docs/guides/templates/using-flex-templates#python)


#### Migrating from App  Engine Map/reduce to Dataflow

[https://cloud.google.com/dataflow/docs/guides/gae-mapreduce-migration](https://cloud.google.com/dataflow/docs/guides/gae-mapreduce-migration)


#### Dataflow Mobile Gaming Example

[https://beam.apache.org/get-started/mobile-gaming-example/](https://beam.apache.org/get-started/mobile-gaming-example/)


### Cloud Dataprep


#### Introduction

Cloud Dataprep by Trifacta is an intelligent data service for visually exploring, cleaning, and preparing structured and unstructured data for analysis, reporting, and machine learning. Because Cloud Dataprep is serverless and works at any scale, there is no infrastructure to deploy or manage. 

[https://cloud.google.com/dataprep](https://cloud.google.com/dataprep)

Use Cloud Dataprep to explore and transform raw data from disparate and/or large datasets into clean and structured data for further analysis and processing.

Access Cloud Dataprep at [https://clouddataprep.com](http://clouddataprep.com/)

Learn how to easily clean up your data without the hassle of writing complex ETL pipelines. 

[https://www.youtube.com/watch?v=DEh3pZIgJ9k](https://www.youtube.com/watch?v=DEh3pZIgJ9k)


#### Qwiklabs


##### Data Transformation Pipeline

The dataset you'll use is an [ecommerce dataset](https://www.en.advertisercommunity.com/t5/Articles/Introducing-the-Google-Analytics-Sample-Dataset-for-BigQuery/ba-p/1676331#) that has millions of Google Analytics session records for the [Google Merchandise Store](https://shop.googlemerchandisestore.com/) loaded into BigQuery. You have a copy of that dataset for this lab and will explore the available fields and rows for insights.

[Creating a Data Transformation Pipeline with Cloud Dataprep](https://www.qwiklabs.com/focuses/4415?parent=catalog)


### Cloud Composer


#### Introduction

Cloud Composer is a managed [Apache Airflow](https://airflow.apache.org/) service that helps you create, schedule, monitor and manage workflows. Cloud Composer automation helps you create Airflow environments quickly and use Airflow-native tools, such as the powerful Airflow web interface and command line tools, so you can focus on your workflows and not your infrastructure.

[https://cloud.google.com/composer/docs](https://cloud.google.com/composer/docs)

Cloud Composer is a managed workflow orchestration service built on Apache Airflow. 

[https://www.youtube.com/watch?v=bwZOAXnCMf8](https://www.youtube.com/watch?v=bwZOAXnCMf8)

Environments are a core concept in Cloud Composer. You can create one or more Cloud Composer environments inside of a project. Environments are self-contained Airflow deployments based on Google Kubernetes Engine. These environments work with Google Cloud services through connectors that are built into Airflow. You create Cloud Composer environments in [supported regions](https://cloud.google.com/about/locations), and the environments run within a Compute Engine zone. For simple use cases, you can create one environment in one region. For complex use cases, you can create multiple environments within a single region or across multiple regions. Airflow communicates with other Google Cloud products through the products' public APIs.


##### Data Pipelines with Cloud Composer

[https://www.youtube.com/watch?v=GeNFEtt-D4k](https://www.youtube.com/watch?v=GeNFEtt-D4k)


##### Cloud Composer best practices

[https://www.youtube.com/watch?v=RrKXZcKOz4A](https://www.youtube.com/watch?v=RrKXZcKOz4A)


#### Tutorials

[https://cloud.google.com/composer/docs/tutorials](https://cloud.google.com/composer/docs/tutorials)


##### Automating infrastructure using Airflow

Stop VM, take snapshots, start VMs, using python API and airflow.   Each step is put into an operator.  Collection of operators are put into a Plugin.  DAGs are composed of each step operator put into a pipeline. DAGs and Plugins are copied into Cloud Storage and run as Cloud Composer jobs.

[https://cloud.google.com/solutions/automating-infrastructure-using-cloud-composer](https://cloud.google.com/solutions/automating-infrastructure-using-cloud-composer)


#### Apache Airflow 

[Airflow](https://airflow.apache.org/) is a platform to programmatically author, schedule and monitor workflows.

Use Airflow to author workflows as Directed Acyclic Graphs (DAGs) of tasks. The Airflow scheduler executes your tasks on an array of workers while following the specified dependencies. Rich command line utilities make performing complex surgeries on DAGs a snap. The rich user interface makes it easy to visualize pipelines running in production, monitor progress, and troubleshoot issues when needed. Airflow is a micro-service architected framework. To deploy Airflow in a distributed setup, Cloud Composer provisions several Google Cloud components, which are collectively known as a Cloud Composer environment.


##### Concepts

[https://airflow.apache.org/docs/stable/concepts.html](https://airflow.apache.org/docs/stable/concepts.html)


##### Apache Airflow for Beginners.

[https://www.youtube.com/watch?v=YWtfU0MQZ_4](https://www.youtube.com/watch?v=YWtfU0MQZ_4)


##### Developing workflows with Apache Airflow

[http://michal.karzynski.pl/blog/2017/03/19/developing-workflows-with-apache-airflow/](http://michal.karzynski.pl/blog/2017/03/19/developing-workflows-with-apache-airflow/)


##### Operators

 An Operator is an atomic block of workflow logic, which performs a single action. Operators are written as Python classes (subclasses of BaseOperator), where the __init__ function can be used to configure settings for the task and a method named execute is called when the task instance is executed.

[https://github.com/apache/airflow/tree/master/airflow/operators](https://github.com/apache/airflow/tree/master/airflow/operators)


##### XCom

[https://airflow.apache.org/docs/stable/concepts.html#xcoms](https://airflow.apache.org/docs/stable/concepts.html#xcoms)


##### Task Orchestration tools: Comparison and Alternatives

A survey of pipeline & workflow tools.

[https://github.com/pditommaso/awesome-pipeline](https://github.com/pditommaso/awesome-pipeline)


##### Industrialization of a Machine Learning model using Apache Airflow and Apache BEAM.

[https://medium.com/swlh/industrialization-of-a-ml-model-using-airflow-and-apache-beam-5a5338f20184](https://medium.com/swlh/industrialization-of-a-ml-model-using-airflow-and-apache-beam-5a5338f20184)


##### Airflow vs. Luigi vs. Argo vs. MLFlow vs. KubeFlow

[https://www.datarevenue.com/en-blog/airflow-vs-luigi-vs-argo-vs-mlflow-vs-kubeflow](https://www.datarevenue.com/en-blog/airflow-vs-luigi-vs-argo-vs-mlflow-vs-kubeflow)


### Google Data Studio

Data Studio is a free tool that turns your data into informative, easy to read, easy to share, and fully customizable dashboards and reports. 

[https://support.google.com/datastudio#topic=6267740](https://support.google.com/datastudio#topic=6267740)

We all have a story to tell. Beyond the compelling words you share, you have insightful data you want your audience to interact with. But building custom interactive data visualizations, and publishing and maintaining them online can be challenging – and expensive. Join us to learn how Google Data Studio keeps you focused on what you do best – telling great data stories.

[https://www.youtube.com/watch?v=NhGLOVkyKjg](https://www.youtube.com/watch?v=NhGLOVkyKjg)


### Datalab 


#### Introduction

[https://www.youtube.com/watch?v=pdQHyTy3s7M](https://www.youtube.com/watch?v=pdQHyTy3s7M)

Cloud Datalab runs inside of a Google Compute Engine VM with an attached persistent disk that is used to store notebooks. Cloud Datalab VMs are connected to a special network in a project called datalab-network. The default configuration of this network limits incoming connections to SSH connections.

[https://cloud.google.com/datalab/docs/how-to/lifecycle](https://cloud.google.com/datalab/docs/how-to/lifecycle)


#### Datalab Quickstart

[https://cloud.google.com/datalab/docs/quickstart](https://cloud.google.com/datalab/docs/quickstart)


#### Working with Notebooks

Jupyter notebooks.

[https://www.youtube.com/watch?v=eEsfPL6SvJc](https://www.youtube.com/watch?v=eEsfPL6SvJc)

Working with Datalab notebooks.

[https://cloud.google.com/datalab/docs/how-to/working-with-notebooks](https://cloud.google.com/datalab/docs/how-to/working-with-notebooks)


### Looker 


#### Introduction

Looker gives you the tools to power a multitude of data experiences, from modern business intelligence and embedded analytics to workflow integrations and custom data apps. Regardless of where your data resides, Looker offers a unified surface to access the truest, most up-to-date version of your company’s data. And with data integrated into users’ daily workflows, organizations can extract value from their data at web scales.

[https://cloud.google.com/looker](https://cloud.google.com/looker)

Looker overview.

[https://www.youtube.com/watch?v=krXaBEi3f1s](https://www.youtube.com/watch?v=krXaBEi3f1s)

Database to Dashboard, technical demo.

[https://www.youtube.com/watch?v=HBgJWCBOOZg](https://www.youtube.com/watch?v=HBgJWCBOOZg)

The Data Modeling Layer.

[https://www.holistics.io/blog/the-data-modeling-layer/](https://www.holistics.io/blog/the-data-modeling-layer/)

How do you decide what to model in dbt vs LookML.

[https://blog.getdbt.com/-how-do-you-decide-what-to-model-in-dbt-vs-lookml--/](https://blog.getdbt.com/-how-do-you-decide-what-to-model-in-dbt-vs-lookml--/)

Dbt vs. Matillion vs. LookML.

[https://www.stephenlevin.co/data-modeling-layer-startup-analytics-dbt-vs-matillion-vs-lookml/](https://www.stephenlevin.co/data-modeling-layer-startup-analytics-dbt-vs-matillion-vs-lookml/)


#### Getting Started with Looker

Looker for data consumers.

[https://training.looker.com/looker-for-data-consumers](https://training.looker.com/looker-for-data-consumers)


#### Building Reports in Looker

Looker for data explorers.

[https://training.looker.com/looker-for-data-explorers](https://training.looker.com/looker-for-data-explorers)


#### LookML

Defining the language of your business with LookML.

[https://www.youtube.com/watch?v=XG4ytmgqSpU](https://www.youtube.com/watch?v=XG4ytmgqSpU)

Looker development foundations.

[https://training.looker.com/looker-development-foundations](https://training.looker.com/looker-development-foundations)

Introduction to LookML.

[https://docs.looker.com/data-modeling/learning-lookml/lookml-intro](https://docs.looker.com/data-modeling/learning-lookml/lookml-intro)

Training business users.

[https://training.looker.com/training-business-users](https://training.looker.com/training-business-users)


#### Looker vs Tableau

[https://looker.com/compare/looker-vs-tableau](https://looker.com/compare/looker-vs-tableau)


#### Looker, Building Explores:

[https://training.looker.com/building-explores-users-will-love](https://training.looker.com/building-explores-users-will-love)


#### Looker, Dashboards

[https://training.looker.com/designing-great-dashboards](https://training.looker.com/designing-great-dashboards)


#### Looker API Examples:

[https://training.looker.com/series/recorded-webinars/the-looker-api](https://training.looker.com/series/recorded-webinars/the-looker-api)


#### Recorded Training

[https://training.looker.com/series/recorded-webinars/custom-visualizations](https://training.looker.com/series/recorded-webinars/custom-visualizations)

[https://training.looker.com/series/recorded-webinars](https://training.looker.com/series/recorded-webinars)


### Data Catalog

Data Catalog is a fully managed and scalable metadata management service that empowers organizations to quickly discover, understand, and manage all of their data.

[https://cloud.google.com/data-catalog/docs](https://cloud.google.com/data-catalog/docs)

Data Catalog is a fully managed and scalable metadata management service that empowers organizations to quickly discover, understand, and manage all of their data.

[https://www.youtube.com/watch?v=eUKqXZDXj78](https://www.youtube.com/watch?v=eUKqXZDXj78)


### Cloud Life Sciences

Cloud Life Sciences is a suite of services and tools for managing, processing, and transforming life sciences data. It also enables advanced insights and operational workflows using highly scalable and compliant infrastructure. Cloud Life Sciences includes features such as the Cloud Life Sciences API and extract-transform-load (ETL) tools, and more.

[https://cloud.google.com/life-sciences/docs](https://cloud.google.com/life-sciences/docs)


### Firestore


#### Introduction

Firestore is a NoSQL document database built for automatic scaling, high performance, and ease of application development. While the Firestore interface has many of the same features as traditional databases, as a NoSQL database it differs from them in the way it describes relationships between data objects.

[https://cloud.google.com/firestore/docs](https://cloud.google.com/firestore/docs)

Cloud Firestore is a horizontally scaling document-model NoSQL database in the cloud.

[https://www.youtube.com/watch?v=v_hR4K4auoQ](https://www.youtube.com/watch?v=v_hR4K4auoQ)

Firestore can be used to build a serverless, scalable, mobile, syncing, analytical, IoT app. Firestore provides a powerful data back end for apps development from kilobyte to petabyte scale.

[https://www.youtube.com/watch?v=ah5tQ7yOh2s](https://www.youtube.com/watch?v=ah5tQ7yOh2s)

Cloud Firestore database service makes it easy for developers to scale new and existing applications, while adding real-time client data synchronization and offline mode capabilities.

[https://www.youtube.com/watch?v=9FRTk05PhRc](https://www.youtube.com/watch?v=9FRTk05PhRc)


#### Datastore

Firestore in Datastore mode is a NoSQL document database built for automatic scaling, high performance, and ease of application development.

Firestore is the newest version of Datastore and introduces [several improvements over Datastore](https://cloud.google.com/datastore/docs/firestore-or-datastore#in_native_mode). 

Existing Datastore users can access these improvements by creating a new Firestore in Datastore mode database instance. In the future, all existing Datastore databases will be [automatically upgraded to Firestore in Datastore mode](https://cloud.google.com/datastore/docs/upgrade-to-firestore).

While the Datastore mode interface has many of the same features as traditional databases, as a NoSQL database it differs from them in the way it describes relationships between data objects.

[https://cloud.google.com/datastore/docs](https://cloud.google.com/datastore/docs)

More explanations.

[https://www.youtube.com/watch?v=SYG-BgXoJFQ](https://www.youtube.com/watch?v=SYG-BgXoJFQ)


### Memorystore

Memorystore for Redis is a fully managed Redis service for the Google Cloud. Applications running on Google Cloud can achieve extreme performance by leveraging the highly scalable, available, secure Redis service without the burden of managing complex Redis deployments.

[https://cloud.google.com/memorystore/docs/redis](https://cloud.google.com/memorystore/docs/redis)

Cloud Memorystore for Redis provides a fully managed in-memory data store service built on scalable, more secure, and highly available infrastructure managed by Google.

[https://www.youtube.com/watch?v=sVpoAdbh2nU](https://www.youtube.com/watch?v=sVpoAdbh2nU)


### Firebase


#### Introduction

[Firebase](https://firebase.google.com/) is an app dev platform built on the [Google Cloud Platform](https://cloud.google.com/products) providing services and cross-platform SDKs. Firebase provides tools to develop high-quality apps, grow the  user base, and monetize the business while focusing on the users.

[https://firebase.google.com/docs/](https://firebase.google.com/docs/)

Youtube channel for firebase.

[https://www.youtube.com/playlist?list=PLOU2XLYxmsIJDw-9-88_LlOs0yR4b4Znv](https://www.youtube.com/playlist?list=PLOU2XLYxmsIJDw-9-88_LlOs0yR4b4Znv)

GCP & Firebase. Firebase projects are GCP Projects.

[https://www.youtube.com/watch?v=xbmYmgBEj4o](https://www.youtube.com/watch?v=xbmYmgBEj4o)

Cloud Functions, and Cloud Firestore. 

[https://www.youtube.com/watch?v=zR6CsTLTPsk](https://www.youtube.com/watch?v=zR6CsTLTPsk)

A list of URLs related to firebase.

[https://github.com/jthegedus/awesome-firebase](https://github.com/jthegedus/awesome-firebase)


#### Cloud Storage for Firebase

Developers use the Firebase SDKs for Cloud Storage to upload and download files directly from clients. If the network connection is poor, the client is able to retry the operation right where it left off, saving your users time and bandwidth.

[https://firebase.google.com/docs/storage/](https://firebase.google.com/docs/storage/)


#### Firebase Realtime Database

Store and sync data with our NoSQL cloud database. Data is synced across all clients in real time, and remains available when your app goes offline. The Firebase Realtime Database is a cloud-hosted database. Data is stored as JSON and synchronized in realtime to every connected client. When you build cross-platform apps with our iOS, Android, and JavaScript SDKs, all of your clients share one Realtime Database instance and automatically receive updates with the newest data.

[https://firebase.google.com/docs/database/](https://firebase.google.com/docs/database/)


#### Cloud Firestore or Realtime Database

Firebase offers two cloud-based, client-accessible database solutions that support real time data syncing:



*   Cloud Firestore is Firebase's newest database for mobile app development. It builds on the successes of the Realtime Database with a new, more intuitive data model. Cloud Firestore also features richer, faster queries and scales further than the Realtime Database.
*   Realtime Database is Firebase's original database. It's an efficient, low-latency solution for mobile apps that require synced states across clients in real time.

[https://firebase.google.com/docs/database/rtdb-vs-firestore](https://firebase.google.com/docs/database/rtdb-vs-firestore)


#### Firebase Authentication

Most apps need to know the identity of a user. Knowing a user's identity allows an app to securely save user data in the cloud and provide the same personalized experience across all of the user's devices. Firebase Authentication provides backend services, easy-to-use SDKs, and ready-made UI libraries to authenticate users to your app. It supports authentication using passwords, phone numbers, popular federated identity providers like Google, Facebook and Twitter, and more. Firebase Authentication integrates tightly with other Firebase services, and it leverages industry standards like OAuth 2.0 and OpenID Connect, so it can be easily integrated with your custom backend.

[https://firebase.google.com/docs/auth/](https://firebase.google.com/docs/auth/)


#### Cloud Functions for Firebase

Cloud Functions for Firebase is a serverless framework that lets you automatically run backend code in response to events triggered by Firebase features and HTTPS requests. Your JavaScript or TypeScript code is stored in Google's cloud and runs in a managed environment. There's no need to manage and scale your own servers.

[https://firebase.google.com/docs/functions/](https://firebase.google.com/docs/functions/)


#### Cloud Storage for Firebase

Cloud Storage for Firebase is a powerful, simple, and cost-effective object storage service built for Google scale. The Firebase SDKs for Cloud Storage add Google security to file uploads and downloads for your Firebase apps, regardless of network quality. You can use our SDKs to store images, audio, video, or other user-generated content. On the server, you can use [Google Cloud Storage](https://cloud.google.com/storage), to access the same files.

[https://firebase.google.com/docs/storage](https://firebase.google.com/docs/storage)


#### Firebase Test Lab

Firebase Test Lab is a cloud-based app-testing infrastructure. With one operation, you can test your Android or iOS app across a wide variety of devices and device configurations, and see the results—including logs, videos, and screenshots—in the Firebase console.

[https://firebase.google.com/docs/test-lab/](https://firebase.google.com/docs/test-lab/)


#### Qwiklabs


##### Build Apps

Firebase is a backend-as-service (Bass) platform for creating mobile and web applications. In this quest you will learn to build serverless web apps, import data into a serverless database, and build a Google Assistant application with Firebase and its Google Cloud integrations.

[Build Apps & Websites with Firebase](https://www.qwiklabs.com/quests/148?catalog_rank=%7B%22rank%22%3A6%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&search_id=7467888)


##### Hugo

In this lab you will create a pipeline for deploying websites based on Hugo, a static website builder. You will store the website content in Cloud Source Repositories and deploy the website with Firebase, then use Cloud Build to create a pipeline to automatically deploy new content that is committed to the repository.

[Deploy a Hugo Website with Cloud Build and Firebase Pipeline](https://www.qwiklabs.com/focuses/14353?catalog_rank=%7B%22rank%22%3A1%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&parent=catalog&search_id=7467907)


### Choosing Which Database to Use

Database choice and comparison charts and methods. \
[https://cloud.google.com/products/databases](https://cloud.google.com/products/databases)
