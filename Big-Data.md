
[Big data](https://en.m.wikipedia.org/wiki/Big_data) is a field that treats ways to analyze, systematically extract information from, or otherwise deal with data sets that are too large or complex to be dealt with by traditional data-processing application software. Data with many fields (columns) offer greater statistical power, while data with higher complexity (more attributes or columns) may lead to a higher false discovery rate.

[Big data](https://www.guru99.com/bigdata-tutorials.html) was originally associated with three key concepts: volume, variety, and velocity. The analysis of big data presents challenges in sampling, and thus previously allowing for only observations and sampling. Therefore, big data often includes data with sizes that exceed the capacity of traditional software to process within an acceptable time and value.

Current usage of the term big data tends to refer to the use of predictive analytics, user behavior analytics, or certain other advanced data analytics methods that extract value from big data, and seldom to a particular size of data set. 

<img src="https://upload.wikimedia.org/wikipedia/commons/e/ee/Big_Data.png" width="500">

The world's technological per-capita capacity to store information has roughly doubled every 40 months since the 1980s.

Based on an IDC report prediction, the global data volume was predicted to grow exponentially from 4.4 [zettabytes](https://en.m.wikipedia.org/wiki/Byte#Multiple-byte_units) to 44 zettabytes between 2013 and 2020. By 2025, IDC predicts there will be 163 zettabytes of data.



The term [Big Data may refer](https://towardsdatascience.com/how-big-is-big-data-3fb14d5351ba) to a dataset which is too large or too complex for ordinary computing devices to process. As such, it is relative to the available computing power on the market. If you look at recent history of data, then in 1999 we had a total of 1.5 exabytes of data and 1 gigabyte was considered big data. Already in 2006, total data was estimated at 160 exabytes level — 1000% more in 7 years. In our Zettabyte Era 1 gigabyte is no longer big data really, and it makes sense to talk about big data starting with at least 1 terabyte. If we were to put that in more mathematical terms, then it seems natural to talk about Big Data with regard to datasets which exceed total data created in the world divided by 1000³.

## Hadoop 

[Apache Hadoop](https://en.m.wikipedia.org/wiki/Apache_Hadoop) is a [collection of open-source software utilities](https://techvidvan.com/tutorials/apache-hadoop-tutorials/) that facilitates using a network of many computers to solve problems involving massive amounts of data and computation. It provides a software framework for distributed storage and processing of big data using the [MapReduce](https://research.google/pubs/pub62/) programming model. Hadoop was originally designed for computer clusters built from commodity hardware, which is still the common use.  

The main Hadoop components are:

* HDFS, a unit for storing big data across multiple nodes in a distributed fashion based on a master-slave architecture.
* NameNode, the master daemon that maintains and manages the DataNodes (slave nodes), recording the metadata of all the files stored in the cluster and every change performed on the file system metadata.
* DataNodes, the slave daemons running on each slave machine that store the actual data, serve read and write requests from clients and manage data blocks.
* YARN, which performs all processing activities by allocating resources and scheduling tasks through two major daemons – ResourceManager and NodeManager.
* ResourceManager, a cluster-level component running on top of YARN for managing resources and scheduling applications.
* NodeManager, a node-level component running on each slave machine for managing containers, monitoring resource utilization in each container, node health and log management.
* MapReduce, which performs all the necessary computations and data processing across the Hadoop cluster.

[Dataproc](Dataproc) is a Google managed [Apache Spark](https://spark.apache.org/) and [Apache Hadoop](https://hadoop.apache.org/) service that [scales](https://cloud.google.com/dataproc/docs/concepts/configuring-clusters/scaling-clusters).

[Some](https://www.teradata.com/Blogs/Why-Hadoop-Failed-and-Where-We-Go-from-Here) [claim](https://www.datanami.com/2017/03/13/hadoop-failed-us-tech-experts-say/)  Hadoop has [some](https://www.singlestore.com/blog/hadoop-the-chronicle-of-an-expected-decline/) [issues](https://towardsdatascience.com/what-happened-to-hadoop-what-should-you-do-now-2876f68dbd1d) and [limitations](https://medium.com/@bharvi.vyas123/6-major-hadoop-limitations-with-their-solutions-1cae1d3936e1).  

There have been [many deprecated](https://www.zdnet.com/article/apache-software-foundation-retires-slew-of-hadoop-related-projects) and [retired](https://en.wikipedia.org/wiki/Apache_Attic) projects among a [very large list of projects](https://en.wikipedia.org/wiki/List_of_Apache_Software_Foundation_projects) and [incubator projects](http://incubator.apache.org/projects/).



## Spark

[Apache Spark](https://en.m.wikipedia.org/wiki/Apache_Spark) is an open-source unified analytics engine for large-scale data processing. Spark provides an interface for programming entire clusters with implicit data parallelism and fault tolerance. Originally developed at the University of California, Berkeley's AMPLab, the Spark codebase was later donated to the Apache Software Foundation.

[Apache Spark](https://thenewstack.io/the-good-bad-and-ugly-apache-spark-for-data-science-work/) has its architectural foundation in the resilient distributed dataset (RDD), a read-only multiset of data items distributed over a cluster of machines, that is maintained in a fault-tolerant way.

The Dataframe API was released as an abstraction on top of the RDD, followed by the Dataset API.

[Apache Spark](https://www.datanami.com/2019/04/03/apache-spark-is-great-but-its-not-perfect/) and its RDDs were developed in 2012 in response to [limitations](https://www.google.com/amp/s/data-flair.training/blogs/13-limitations-of-hadoop/amp/) in the [MapReduce](https://en.m.wikipedia.org/wiki/MapReduce) cluster computing paradigm, which forces a particular linear dataflow structure on distributed programs: MapReduce programs read input data from disk, map a function across the data, reduce the results of the map, and store reduction results on disk.  Hadoop and Spark are [different platforms](https://www.infoworld.com/article/3236869/what-is-apache-spark-the-big-data-platform-that-crushed-hadoop.html), each implementing various technologies that can work separately and together.

Spark's RDDs function as a working set for distributed programs that offers a (deliberately) restricted form of distributed shared memory.

The main Spark components are: 

* Spark Core, the base engine for large-scale parallel and distributed data processing, responsible for memory management and fault recovery, scheduling, distributing and monitoring jobs on a cluster and interacting with storage systems.
* Spark Streaming for processing real-time streaming data, enabling high-throughput and fault-tolerant stream processing of live data streams.
* Spark SQL for integrating relational processing with the functional programming API.
* GraphX, an API for graphs and graph-parallel computation.
* MLlib, a machine learning library for performing machine learning.

## Perspectives on Big Data

In the Big Data  chronicles, [The Google File System paper in 2003](https://research.google/pubs/pub51/) marked a seminal moment for software development. It was one of the first times Google detailed the technical underpinnings that helped it catapult from clever idea to global force.

The following year in 2004, Google shared [another paper on MapReduce](https://research.google/pubs/pub62), further cementing the genealogy of big data. 

[MapReduce](https://en.m.wikipedia.org/wiki/MapReduce) was a new technique to move computation to data, and it allowed large web companies including Google to operate with enormous amounts of information, such as the entire internet. 

Soon after that, Doug Cutting, Hadoop’s initial creator, began to implement MapReduce and the Hadoop Distributed File System while at Yahoo, and in 2006 Hadoop 0.1.0 was released.

Six years later in 2012, Hadoop 1.0 became available.

By 2017, the Hadoop hype [has come and gone](https://0x0fff.com/hadoop-the-end-of-an-era/).

Did Google unintentionally send the industry  [on a more than a decade long head-fake](https://garyorenstein.medium.com/did-google-send-the-big-data-industry-on-a-10-year-head-fake-9c94d553925a)?

There's now [BigQuery](BigQuery) and [Spanner](Spanner). There's a [Shift to Distributed SQL](https://medium.com/@garyorenstein/the-shift-to-distributed-sql-232c04dec1f7).


[Often](https://www.chrisstucchio.com/blog/2013/hadoop_hatred.html) the data you may use isn't [really that big](https://veekaybee.github.io/2017/03/20/hadoop-or-laptop/) or do not need to be that [big](https://hbr.org/2013/12/you-may-not-need-big-data-after-all).

[Big data ethics](https://en.m.wikipedia.org/wiki/Big_data_ethics) also known as simply data ethics refers to systemizing, defending, and recommending concepts of right and wrong conduct in relation to data, in particular personal data.

