

[Cloud Spanner](https://cloud.google.com/spanner) is a  [managed relational database](https://www.youtube.com/watch?v=IFbydfGV2lQ) with [unlimited scale, strong consistency, and up to 99.999% availability](https://www.youtube.com/watch?v=5bjYk6Hhd10). 

[Cloud Spanner](https://www.youtube.com/watch?v=bUSU1e9j8wc)    optimizes performance by [automatically sharding the data based on request load and size](https://www.youtube.com/watch?v=amcf6W2Xv6M) of the data. 


[Cloud Spanner](https://www.youtube.com/watch?v=C75kpQszAjs) is a relational database service that offers transactional consistency at [global scale](https://techcrunch.com/2018/12/19/googles-cloud-spanner-database-adds-new-features-and-regions/), [schemas](https://cloud.google.com/spanner/docs/schema-and-data-model), SQL (ANSI 2011 with extensions), and automatic, synchronous replication for high availability.

[Cloud Spanner](https://www.youtube.com/watch?v=IfsTINNCooY) can [help you create time-sensitive, mission critical applications](https://www.youtube.com/watch?v=5bjYk6Hhd10) at scale.  In terms of [CAP theorem](https://en.wikipedia.org/wiki/CAP_theorem) the consensus is that  [Spanner is CP with good A](https://cloud.google.com/blog/products/databases/inside-cloud-spanner-and-the-cap-theorem).

[Cloud Spanner](https://www.youtube.com/watch?v=sOtlaH-QlxM) is one of the [Distributed SQL Databases](https://www.infoworld.com/article/3406458/the-best-distributed-relational-databases.amp.html).
In general, a [Distributed SQL Database](https://wikipedia.org/wiki/Distributed_SQL) is [a single logical database](https://www.youtube.com/watch?v=9PsSIVUbtWo) deployed across multiple physical nodes in a single data center or across many data centers if need be; all of which allow it to deliver elastic scale and bulletproof resilience.
[Original paper on Spanner](https://static.googleusercontent.com/media/research.google.com/en//archive/spanner-osdi2012.pdf) explains [details](https://thedataguy.in/internals-of-google-cloud-spanner/) of its [design](https://www.youtube.com/watch?v=nvlt0dA7rsQ). 


https://cloud.google.com/blog/topics/developers-practitioners/what-cloud-spanner

## Architecture


A [Spanner](http://disa.fi.muni.cz/wp-content/uploads/Spanner.pdf) deployment is called a [universe](https://www.datasciencecentral.com/profiles/blogs/google-spanner-the-future-of-nosql). Given that Spanner manages data globally, there will be only a handful of running universes.
Spanner is organized as a set of [zones](https://jayendrapatil.com/google-cloud-spanner/), where each zone is the rough analog of a deployment of [Bigtable](Bigtable) servers.
Zones are the unit of administrative deployment. The set of zones is also the set of locations across
which data can be replicated. 
Zones can be added to or removed from a running system as new datacenters are
brought into service and old ones are turned off, respectively. 



Zones are also the unit of [physical isolation](https://anantja.in/spanner/): there
may be one or more zones in a datacenter, for example, if different applications’ data must be partitioned across
different sets of servers in the same datacenter.


A zone has [one zonemaster and between one hundred and several thousand spanservers](https://www.researchgate.net/figure/Spanner-server-organization_fig5_289881173). The former assigns
data to spanservers; the latter serve data to clients. 
The per-zone location proxies are used by clients to locate
the spanservers assigned to serve their data. The universe master and the placement driver are currently singletons. 
The universe master is primarily a console that displays status information about all the zones for interactive debugging. 
The placement driver handles automated movement of data across zones on the timescale of minutes. 
The placement driver periodically communicates with the spanservers to find data that needs to be moved, either to meet updated replication constraints or to balance load.

### Spanserver

At the bottom, [each spanserver is responsible for between 100 and 1000 instances of a data structure called a tablet](https://anantja.in/static/35879ee8585f94ae399c30384ef02599/748b0/2.png). 
A tablet is similar to Bigtable’s tablet abstraction, in that it implements a bag of the following mappings:

```
  (key:string, timestamp:int64) → string

```

Unlike [Bigtable](Bigtable), Spanner assigns timestamps to data, which is an important way in which Spanner is more like a multi-version database than a key-value store.  
A tablet’s state is stored in set of [B-tree-like](https://wikipedia.org/wiki/B-tree) files and a write-ahead log, all on a distributed file system called
[Colossus](https://cloudblog.withgoogle.com/products/storage-data-transfer/a-peek-behind-colossus-googles-file-system)  (the successor to the Google File System).  
To support replication, each spanserver implements a single [Paxos](https://www.cs.rutgers.edu/~pxk/417/notes/paxos.html)   state machine on top of each tablet.
The [Paxos](https://medium.com/distributed-knowledge/paxos-consensus-for-beginners-1b8519d3360f)    state machines are used to implement a consistently replicated bag of mappings. 
The key-value
mapping state of each replica is stored in its corresponding tablet. Writes must initiate the [Paxos](https://en.m.wikipedia.org/wiki/Paxos_(computer_science)) protocol at the
leader; reads access state directly from the underlying tablet at any replica that is sufficiently up-to-date. 
The
set of replicas is collectively a Paxos group. 
At every replica that is a leader, each spanserver implements a lock table to implement concurrency control. The lock table contains the state for two-phase locking: it maps ranges of keys to lock states.

### Split

Spanner is global database system, per region we’ll get minimum of 3 shards. 
Each shard will be in each zone. 
In Spanner terms a shard is called as [Split](  https://cloud.google.com/spanner/docs/schema-and-data-model#database-splits ). 
If your provision 1 Node Spanner cluster, you’ll get 2 more Nodes on the different zone which are invisible to you. 
And the Compute and Storage layers are de-coupled. Paxos algorithm is used to maintain one leader at a time and rest of the nodes will be the followers.
Based on the partitions, we’ll have more Splits(shards) in the storage layer. 
Each shard will be replicated to the other Zones. 
For eg: if you have a shard called S1 on Zone A, it’ll be replicated to Zone B and C. 
The replication works based on Leader follower method. 
So the Paxos will help to maintain the quorum and will help to select a new Leader during the failure. 
If you are writing something on this Split, the Spanner APIs are aware of the Leaders. 
So the write directly goes to the Zone where it has the Leader Split. 
Each Split has its own leader zone.


## CAP

https://cloud.google.com/blog/products/databases/inside-cloud-spanner-and-the-cap-theorem

## Strong Consistency

Spanner, as most [ACID](https://wikipedia.org/wiki/ACID) databases, it uses the [2PC](https://en.m.wikipedia.org/wiki/Two-phase_commit_protocol) (Two phase commit), and it uses Paxos groups to mitigate the "anti-availability" shortcoming. 
At the highest level of abstraction, Spanner is a database that shards data across many sets of Paxos state machines in datacenters spread all over the world.
Spanner provides synchronous cross-datacenter replication and strong consistency and usability of traditional SQL databases. 

### Google F1 

[F1](https://research.google/pubs/pub41344/) is a distributed relational database built to support the Google AdWords business.  

F1 is built using Spanner to replace an implementation based on MySQL.

## Transactions

https://cloud.google.com/spanner/docs/transactions

## External Consistency, Linearizability, Serializability

Cloud Spanner provides clients with the strictest concurrency-control guarantees for transactions, which is called external consistency. Under external consistency, the system behaves as if all transactions were executed sequentially, even though Cloud Spanner actually runs them across multiple servers (and possibly in multiple datacenters) for higher performance and availability. 
In addition if one transaction completes before another transaction starts to commit, the system guarantees that clients can never see a state that includes the effect of the second transaction but not the first. 
Intuitively, Cloud Spanner is semantically indistinguishable from a single-machine database. 
Even though it provides such strong guarantees, Cloud Spanner enables applications to achieve performance comparable to databases that provide weaker guarantees. 
Cloud Spanner provides [external consistency](https://www.youtube.com/watch?v=QdkS6ZjeR7Q), which is a stronger property than linearizability, because linearizability does not say anything about the behavior of transactions.


Linearizability is a property of concurrent objects that support atomic read and write operations. 
In a database, an "object" would typically be a single row or even a single cell. 
External consistency is a property of transaction-processing systems, where clients dynamically synthesize transactions that contain multiple read and write operations on arbitrary objects. 
Cloud Spanner provides external [consistency](https://aphyr.com/posts/313-strong-consistency-models), which is a stricter property than serializability. 
A transaction-processing system is serializable if it executes transactions in a manner that is indistinguishable from a system in which the transactions are executed serially. 
[Cloud Spanner](https://blog.searce.com/internals-of-google-cloud-spanner-5927e4b83b36) also guarantees that the serial order is consistent with the order in which the transactions can be observed to commit.
In a system that provides serializability but not external consistency, even though the customer executed T1 and then T2 sequentially, the system would be permitted to reorder them, which could cause the debit to incur a penalty due to insufficient funds.


https://jepsen.io/consistency


## TrueTime

Spanner is very keen in [synchronizing](https://medium.com/google-cloud/google-cloud-spanner-technical-overview-e3e37d81ea60) and maintains the same time across all the nodes over the global datacenters. 
The hardware components are built with Atomic Clocks to maintain the time. 
If you take a look at the Server Hardware Rack, the Server is having 4 time servers. 
2 Servers are connected with GPS and the remaining 2 are connect with Automic Oscillators. 
There are 2 different brands of Oscillators for better failover processing. 
The GPS time servers will sync with Oscillators to synchronize the time across the global datacenters with every 30sec interval.


TrueTime is a highly available, distributed clock that is provided to applications on all Google servers. 
TrueTime enables applications to generate monotonically increasing timestamps: an application can compute a timestamp T that is guaranteed to be greater than any timestamp T' if T' finished being generated before T started being generated. 
This guarantee holds across all servers and all timestamps.

[https://cloud.google.com/spanner/docs/true-time-external-consistency](https://cloud.google.com/spanner/docs/true-time-external-consistency)


https://www.youtube.com/watch?v=iKQhPwbzzxU


Some databases support similar timestamp capabilities [without TrueTime](https://www.cockroachlabs.com/blog/living-without-atomic-clocks/).




## JSON data type

https://cloud.google.com/blog/products/databases/manage-semi-structured-data-in-cloud-spanner-with-json



## Examples

### Build realtime inventory management systems with Cloud Spanner

Build  an inventory ledger solution that streamlines the order-to-shipping process using Cloud Spanner, a scalable, globally consistent database service. The single source of truth enables seamless customer experiences across channels and real-time decisioning at scale. 

[https://www.youtube.com/watch?v=8kj_uA5vJfo](https://www.youtube.com/watch?v=8kj_uA5vJfo)

### Provisioning Spanner with terraform

https://cloud.google.com/blog/topics/developers-practitioners/provisioning-cloud-spanner-using-terraform

## Migrating to Spanner

https://www.youtube.com/watch?v=FNeGQUqMa_c

https://cloud.google.com/architecture/migrating-mysql-to-spanner

## Migrating from Oracle OLTP to Cloud Spanner

https://cloud.google.com/architecture/migrating-oracle-to-cloud-spanner

## Tutorials

[https://cloud.google.com/spanner/docs/tutorials](https://cloud.google.com/spanner/docs/tutorials)

## Optimizing Applications, Schemas, and Query Design on Cloud Spanner

Discuss [techniques for monitoring Cloud Spanner](https://www.youtube.com/watch?v=DxrdatA_ULk) to identify performance bottlenecks. 


The [Cloud Spanner SQL query optimizer](https://cloud.google.com/spanner/docs/query-optimizer/overview) converts a declarative SQL statement, that describes what data the query wants, into an imperative execution plan, that describes one way to precisely obtain that data. The process of transforming a declarative statement into a query execution plan involves performing transformations to tree structures used to represent the query. It is expected that the optimizer, in the process of producing an execution plan, preserves the logical meaning of the original SQL query so that the correct rows are returned.


[This page](https://cloud.google.com/spanner/docs/schema-design) describes best practices for designing Cloud Spanner schemas to avoid hotspots and for loading data into Cloud Spanner. Pay attention to [query limits](https://cloud.google.com/spanner/quotas#query_limits) and [limits in CRUD operations](https://cloud.google.com/spanner/quotas#limits_for_creating_reading_updating_and_deleting_data).

### Spanner Emulator

The [Cloud SDK](https://cloud.google.com/sdk) provides a local, in-memory emulator, which you can use to develop and test your applications for free without creating a GCP Project or a billing account. As the emulator stores data only in memory, all state, including data, schema, and configs, is lost on restart. The emulator offers the same APIs as the Cloud Spanner production service and is intended for local development and testing, not for production deployments.
The [emulator](https://cloud.google.com/spanner/docs/emulator) supports all languages of the client libraries. You can also use the emulator with the gcloud command-line tool and REST APIs.
The emulator is also available as an open source project in [GitHub](https://github.com/GoogleCloudPlatform/cloud-spanner-emulator).


https://cloud.google.com/blog/topics/developers-practitioners/deployment-models-cloud-spanner-emulator

## BigQuery Spanner federation 

BigQuery Spanner federation  enables BigQuery to query data residing in Spanner in real-time, without copying or moving data.
https://cloud.google.com/bigquery/docs/cloud-spanner-federated-queries


### Replicating from Cloud Spanner to BigQuery at scale

https://cloud.google.com/blog/topics/developers-practitioners/replicating-cloud-spanner-bigquery-scale



## Point in time recovery

https://cloud.google.com/spanner/docs/pitr





## Databases, ETL, ELT and tools.

[https://cube.dev/blog/category/data-stack/](https://cube.dev/blog/category/data-stack/)

## Using Spanner to store game states

https://cloud.google.com/architecture/best-practices-cloud-spanner-gaming-database

## Spanner SQL Best practices

https://cloud.google.com/spanner/docs/sql-best-practices

## Examples

### Spanner Node.js example with Cloud Run

https://cloud.google.com/blog/topics/developers-practitioners/deploying-cloud-spanner-based-nodejs-application

###  Reduce latency with Cloud Spanner multi-region leader placement

https://cloud.google.com/blog/topics/developers-practitioners/reduce-latency-with-cloud-spanner-multi-region-leader-placement


### DynamoDB to Cloud Spanner via HarbourBridge

https://cloud.google.com/blog/products/databases/migrating-to-cloud-spanner-from-dynamodb-via-harbourbridge


## Qwiklabs


### Quick Start

[Cloud Spanner: Qwik Start](https://www.qwiklabs.com/focuses/1774?parent=catalog)


### Java Client

In this lab, you will set up a Cloud Spanner instance, create a database and schema, then run sample queries on a dataset. Helpful Cloud Spanner information is provided along the way to help you get the most out of this powerful database service.

[Querying Cloud Spanner With a Java Client](https://www.qwiklabs.com/focuses/2189?parent=catalog)


### Leaderboard

In this lab, you will learn how to set up a Cloud Spanner instance. You will go through the steps of creating a database and schema that can be used for a gaming leaderboard. You'll start by creating a Players table for storing player information and a Scores table to store player scores.

[Cloud Spanner: Create a Gaming Leaderboard with C#](https://www.qwiklabs.com/focuses/1815?parent=catalog)


### Backend

In this lab, you develop a backend service for an online Quiz application to process user feedback and save scores.

[App Dev: Developing a Backend Service - Java](https://www.qwiklabs.com/focuses/1128?parent=catalog)


### Python

This lab concentrates on the backend service, putting together Pub/Sub, Natural Language, and Spanner services and APIs to collect and analyze feedback and scores from an online Quiz application.

[App Dev: Developing a Backend Service - Python](https://www.qwiklabs.com/focuses/1107?parent=catalog)
