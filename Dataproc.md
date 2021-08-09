


## Introduction

[Dataproc](https://cloud.google.com/dataproc/docs) is a managed [Apache Spark](https://spark.apache.org/) and [Apache Hadoop](https://hadoop.apache.org/) service that lets you take advantage of open source data tools for batch processing, querying, streaming, and machine learning. 



Enterprises are migrating their existing on-premises Apache Hadoop and Spark clusters over to Dataproc to manage costs and unlock the power of elastic scale. 

[https://cloud.google.com/dataproc/docs/tutorials](https://cloud.google.com/dataproc/docs/tutorials)


[https://www.youtube.com/watch?v=h1LvACJWjKc](https://www.youtube.com/watch?v=h1LvACJWjKc)


[Dataproc Metastore](https://www.google.com/amp/s/cloudblog.withgoogle.com/products/data-analytics/cloud-hive-metastore-now-available/amp/ ) can be used as a [centralized metadata repository]( 
 https://cloud.google.com/dataproc-metastore/docs  ) that can be shared among various ephemeral Dataproc clusters running different [open source components](https://cloud.google.com/dataproc/docs/concepts/components/overview#available_optional_components ).






[Component Gateway](https://cloud.google.com/dataproc/docs/concepts/accessing/dataproc-gateways ) provides secure access to web endpoints for Dataproc default and [optional components](https://cloud.google.com/dataproc/docs/concepts/components/overview#available_optional_components ).

## Big Data analytics with Dataproc

[https://programmaticponderings.com/2018/12/11/big-data-analytics-with-java-and-python-using-cloud-dataproc-googles-fully-managed-spark-and-hadoop-service/](https://programmaticponderings.com/2018/12/11/big-data-analytics-with-java-and-python-using-cloud-dataproc-googles-fully-managed-spark-and-hadoop-service/)


## Migrating Hadoop to GCP

[https://www.youtube.com/watch?v=YK_-yS9y_0k](https://www.youtube.com/watch?v=YK_-yS9y_0k)


## Basic introduction to Apache Hadoop

[https://www.youtube.com/watch?v=OoEpfb6yga8](https://www.youtube.com/watch?v=OoEpfb6yga8)

You can [see how to]( https://www.linode.com/docs/guides/how-to-install-and-set-up-hadoop-cluster/) create a small three node Hadoop cluster and submit map reduce example.

## Apache Spark Tutorial

[https://www.youtube.com/watch?v=IQfG0faDrzE4](https://www.youtube.com/watch?v=IQfG0faDrzE4)  


## A Scala tutorial for Java programmers

[https://docs.scala-lang.org/tutorials/scala-for-java-programmers.html](https://docs.scala-lang.org/tutorials/scala-for-java-programmers.html)


## Some online courses to learn Hadoop and Spark

[https://medium.com/swlh/5-free-online-courses-to-learn-big-data-hadoop-and-spark-in-2019-a553e6ccfe30](https://medium.com/swlh/5-free-online-courses-to-learn-big-data-hadoop-and-spark-in-2019-a553e6ccfe30)




## Spark by Example

[https://sparkbyexamples.com/](https://sparkbyexamples.com/)


## Main Spark github source tree

[https://github.com/apache/spark](https://github.com/apache/spark)


## Spark examples source code

[https://github.com/apache/spark/tree/master/examples/src/main](https://github.com/apache/spark/tree/master/examples/src/main)


## Hadoop Data Storage

Dataproc integrates with Apache Hadoop and the Hadoop Distributed File System (HDFS). 

[https://cloud.google.com/dataproc/docs/concepts/dataproc-hdfs](https://cloud.google.com/dataproc/docs/concepts/dataproc-hdfs)


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