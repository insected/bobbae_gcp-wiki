[Dataproc](https://cloud.google.com/dataproc/docs) is a managed [Apache Spark](Spark) and [Apache Hadoop](Hadoop) service that lets you take advantage of open source data tools for [batch processing](https://cloud.google.com/dataproc/docs/tutorials/bigquery-connector-mapreduce-example), [querying](https://cloud.google.com/dataproc/docs/tutorials/presto-dataproc), [streaming](https://cloud.google.com/architecture/using-apache-spark-dstreams-with-dataproc-and-pubsub), and [machine learning](https://cloud.google.com/dataproc/docs/tutorials/bigquery-sparkml). 

## Migrating Hadoop to Dataproc

Enterprises are migrating their existing on-premises Apache Hadoop and Spark clusters over to Dataproc to manage costs and unlock the power of elastic scale. 

[https://www.youtube.com/watch?v=h1LvACJWjKc](https://www.youtube.com/watch?v=h1LvACJWjKc)

## Metastore

[Dataproc Metastore](https://www.google.com/amp/s/cloudblog.withgoogle.com/products/data-analytics/cloud-hive-metastore-now-available/amp/ ) is a managed [Hive metastore](   https://lakefs.io/hive-metastore-why-its-still-here-and-what-can-replace-it/ ) that can be used as a [centralized metadata repository]( 
 https://cloud.google.com/dataproc-metastore/docs  ) that can be shared among various ephemeral Dataproc clusters running different [open source components](https://cloud.google.com/dataproc/docs/concepts/components/overview#available_optional_components ).

## Component Gateway

[Component Gateway](https://cloud.google.com/dataproc/docs/concepts/accessing/dataproc-gateways ) provides secure access to web endpoints for Dataproc default and [optional components](https://cloud.google.com/dataproc/docs/concepts/components/overview#available_optional_components ).



## Big Data analytics with Dataproc

[https://programmaticponderings.com/2018/12/11/big-data-analytics-with-java-and-python-using-cloud-dataproc-googles-fully-managed-spark-and-hadoop-service/](https://programmaticponderings.com/2018/12/11/big-data-analytics-with-java-and-python-using-cloud-dataproc-googles-fully-managed-spark-and-hadoop-service/)


## Migrating Hadoop to GCP

[https://www.youtube.com/watch?v=YK_-yS9y_0k](https://www.youtube.com/watch?v=YK_-yS9y_0k)

### AWS EMR vs Dataproc

https://hackernoon.com/why-dataproc-googles-managed-hadoop-and-spark-offering-is-a-game-changer-9f0ed183fda3

## Basic introduction to Apache Hadoop

[https://www.youtube.com/watch?v=OoEpfb6yga8](https://www.youtube.com/watch?v=OoEpfb6yga8)

### Map reduce job example

You can [see how to]( https://www.linode.com/docs/guides/how-to-install-and-set-up-hadoop-cluster/) create a small three node Hadoop cluster and submit map reduce example.

### MrJob

[mrjob](https://mrjob.readthedocs.io/) lets you write MapReduce jobs in Python 2.7/3.4+ and run them on several platforms. 



## Dataproc Hadoop Data Storage

Dataproc integrates with Apache Hadoop and the Hadoop Distributed File System (HDFS). 

[https://cloud.google.com/dataproc/docs/concepts/dataproc-hdfs](https://cloud.google.com/dataproc/docs/concepts/dataproc-hdfs)


## Creating Dataproc cluster

https://medium.com/google-cloud/creating-a-dataproc-cluster-considerations-gotchas-resources-930294ddb7f3

## Hive

[Apache Hive](https://hive.apache.org/) is a data warehouse software project built on top of Apache Hadoop for providing data query and analysis. 

[https://www.youtube.com/watch?v=cMziv1iYt28](https://www.youtube.com/watch?v=cMziv1iYt28)

[Using Apache Hive on Dataproc](https://cloud.google.com/architecture/using-apache-hive-on-cloud-dataproc ).

Apache Hive is considered [similar]( https://blog.clairvoyantsoft.com/bigquery-fundamentals-and-its-benefits-over-hive-hadoop-c3d53e4d2b8f ) to BigQuery.


## Hadoop Pig 

[Apache Pig](http://pig.apache.org/) is a platform for analyzing large data sets that consists of a high-level language for expressing data analysis programs, coupled with infrastructure for evaluating these programs.

[https://www.youtube.com/watch?v=Hve24pRW_Ps](https://www.youtube.com/watch?v=Hve24pRW_Ps) 


## Hive vs Pig vs SQL

[https://www.whizlabs.com/blog/hive-vs-pig-vs-sql/](https://www.whizlabs.com/blog/hive-vs-pig-vs-sql/)


## Pig Latin SQL Challenge

Doing ETL in SQL or [Pig Latin](https://pig.apache.org/docs/latest/basic.html) to give more detailed feel for why one might prefer one or the other in solving actual common problems:

[http://www.olric.org/2019/09/pig-latin-sql-challenge-or-window.html?m=1](http://www.olric.org/2019/09/pig-latin-sql-challenge-or-window.html?m=1)


## Sawzall

A perspective on Sawzall DSL (domain specific language) over Google map/reduce and Pig DSL over Hadoop map/reduce.

[http://glinden.blogspot.com/2007/04/yahoo-pig-and-google-sawzall.html?m=1](http://glinden.blogspot.com/2007/04/yahoo-pig-and-google-sawzall.html?m=1)

And finally a perspective on replacing Sawzell within Google.

[http://www.unofficialgoogledatascience.com/2015/12/replacing-sawzall-case-study-in-domain.html?m=1](http://www.unofficialgoogledatascience.com/2015/12/replacing-sawzall-case-study-in-domain.html?m=1)


## Tutorials



[https://cloud.google.com/dataproc/docs/tutorials](https://cloud.google.com/dataproc/docs/tutorials)



[Write Spark Scala Jobs (From Spark to DataProc)](https://cloud.google.com/dataproc/docs/tutorials/spark-scala)



[Hadoop to GCP](https://cloud.google.com/blog/products/data-analytics/goodbye-hadoop-building-a-streaming-data-processing-pipeline-on-google-cloud) 


[Machine Learning with Spark on Google Cloud Dataproc](https://www.qwiklabs.com/focuses/3390?parent=catalog )


[Distributed Image Processing in Cloud Dataproc](https://www.qwiklabs.com/focuses/5834?parent=catalog)

[Using Apache Spark DStreams with Dataproc and Pub/Sub](https://cloud.google.com/architecture/using-apache-spark-dstreams-with-dataproc-and-pubsub)

[Cloud Bigtable map reduce word count example with Dataproc](https://github.com/GoogleCloudPlatform/cloud-bigtable-examples/tree/master/java/dataproc-wordcount)

[Install and run a Jupyter notebook on a Dataproc cluster](https://cloud.google.com/dataproc/docs/tutorials/jupyter-notebook)

[Apache Spark and Jupyter Notebooks made easy with Dataproc component gateway](https://medium.com/google-cloud/apache-spark-and-jupyter-notebooks-made-easy-with-dataproc-component-gateway-fa91d48d6a5a)

[Cloud Dataproc example repository](https://github.com/GoogleCloudDataproc/cloud-dataproc)


## Big Data Hadoop Tutorial

https://www.guru99.com/bigdata-tutorials.html

<!--
### Hadoop dissent

https://adamdrake.com/command-line-tools-can-be-235x-faster-than-your-hadoop-cluster.html

### awk

https://livefreeordichotomize.com/2019/06/04/using_awk_and_r_to_parse_25tb/

### Hadoop fatigue


https://www.codetd.com/en/article/13077139

-->