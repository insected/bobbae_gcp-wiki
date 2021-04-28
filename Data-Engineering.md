  * [Data Engineering](#data-engineering)
    + [Overview](#overview)
    + [Database options](#database-options)
    + [Cloud SQL](#cloud-sql)
    + [SQL](#sql)
      - [Tutorials](#tutorials)
    + [Cloud Bigtable](#cloud-bigtable)
    + [Cloud Dataproc](#cloud-dataproc)
    + [Cloud Pub/Sub](#cloud-pub-sub)
    + [BigQuery](#bigquery)
    + [Cloud Spanner](#cloud-spanner)
    + [Cloud Data Fusion](#cloud-data-fusion)
      - [Introduction](#introduction)
      - [CDAP](#cdap)
      - [Qwiklab](#qwiklab)
        * [Codeless Pipelines](#codeless-pipelines)
    + [Dataflow](#dataflow)
    + [Cloud Dataprep](#cloud-dataprep)
    + [Cloud Composer](#cloud-composer)
    + [Google Data Studio](#google-data-studio)
    + [Datalab](#datalab)
      - [Introduction](#introduction-1)
      - [Datalab Quickstart](#datalab-quickstart)
      - [Working with Notebooks](#working-with-notebooks)
    + [Looker](#looker)
    + [Data Catalog](#data-catalog)
    + [Cloud Life Sciences](#cloud-life-sciences)
    + [Firestore](#firestore)
    + [Datastore](#datastore)
    + [Memorystore](#memorystore)
    + [Firebase](#firebase)
- [Choosing Which Database to Use](#choosing-which-database-to-use)

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

[Data Studio](https://datastudio.google.com) is a free tool that turns your data into informative, easy to read, easy to share, and fully customizable dashboards and reports. 

[https://support.google.com/datastudio#topic=6267740](https://support.google.com/datastudio#topic=6267740)

Demonstration of Data Studio.

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

