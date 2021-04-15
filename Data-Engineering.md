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

Data engineering is a set of operations aimed at creating interfaces and mechanisms for the flow and access of information. It takes dedicated specialists – data engineers – to maintain data so that it remains available and usable by others. In short, data engineers set up and operate the organization’s data infrastructure preparing it for further analysis by data analysts and scientists.

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
SQL is commonly pronounced “sequel.” Its most popular variants are MySQL, PostgreSQL, and SQLite - a version of SQL which is commonly used for prototyping. It introduced the concept of accessing many records with one single command, using SQL Queries.

#### Tutorials

[https://www.youtube.com/watch?v=HXV3zeQKqGY](https://www.youtube.com/watch?v=HXV3zeQKqGY)

[https://www.freecodecamp.org/news/best-sql-database-tutorial/](https://www.freecodecamp.org/news/best-sql-database-tutorial/)


### Cloud Bigtable

https://github.com/bobbae/gcp/wiki/Bigtable

### Cloud Dataproc

https://github.com/bobbae/gcp/wiki/Dataproc

### Cloud Pub/Sub

https://github.com/bobbae/gcp/wiki/PubSub

### BigQuery

https://github.com/bobbae/gcp/wiki/BigQuery

### Cloud Spanner

https://github.com/bobbae/gcp/wiki/Spanner

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

https://github.com/bobbae/gcp/wiki/Dataflow

### Cloud Dataprep

https://github.com/bobbae/gcp/wiki/Dataprep

### Cloud Composer

https://github.com/bobbae/gcp/wiki/Composer

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


https://github.com/bobbae/gcp/wiki/Looker

### Data Catalog

Data Catalog is a fully managed and scalable metadata management service that empowers organizations to quickly discover, understand, and manage all of their data.

[https://cloud.google.com/data-catalog/docs](https://cloud.google.com/data-catalog/docs)

Data Catalog is a fully managed and scalable metadata management service that empowers organizations to quickly discover, understand, and manage all of their data.

[https://www.youtube.com/watch?v=eUKqXZDXj78](https://www.youtube.com/watch?v=eUKqXZDXj78)


### Cloud Life Sciences

Cloud Life Sciences is a suite of services and tools for managing, processing, and transforming life sciences data. It also enables advanced insights and operational workflows using highly scalable and compliant infrastructure. Cloud Life Sciences includes features such as the Cloud Life Sciences API and extract-transform-load (ETL) tools, and more.

[https://cloud.google.com/life-sciences/docs](https://cloud.google.com/life-sciences/docs)


### Firestore

https://github.com/bobbae/gcp/wiki/Firestore

### Datastore

https://github.com/bobbae/gcp/wiki/Datastore


### Memorystore

https://github.com/bobbae/gcp/wiki/Memorystore


### Firebase

https://github.com/bobbae/gcp/wiki/Firebase


# Choosing Which Database to Use

Database choice and comparison charts and methods. 
[https://cloud.google.com/products/databases](https://cloud.google.com/products/databases)

