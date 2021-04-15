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

