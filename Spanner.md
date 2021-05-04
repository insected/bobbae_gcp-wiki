

[Cloud Spanner](https://cloud.google.com/spanner) is a  managed relational database with unlimited scale, strong consistency, and up to 99.999% availability. 

[Cloud Spanner](https://cloud.google.com/spanner)    optimizes performance by automatically sharding the data based on request load and size of the data. As a result, you can spend less time worrying about how to scale your database and instead focus on [scaling your business](https://www.youtube.com/watch?v=bUSU1e9j8wc&list=PLIivdWyY5sqJPSoX2R4mRq_wyg0JTjrAG&index=1).


Cloud Spanner is a relational database service that offers transactional consistency at [global scale](https://www.google.com/amp/s/techcrunch.com/2018/12/19/googles-cloud-spanner-database-adds-new-features-and-regions/amp/), [schemas](https://cloud.google.com/spanner/docs/schema-and-data-model), SQL (ANSI 2011 with extensions), and automatic, synchronous replication for high availability.



[Cloud Spanner](https://www.youtube.com/watch?v=IfsTINNCooY) can [help you create time-sensitive, mission critical applications](https://www.youtube.com/watch?v=5bjYk6Hhd10) at scale. 





Cloud Spanner is one of [Distributed SQL Databases](https://www.google.com/amp/s/www.infoworld.com/article/3406458/the-best-distributed-relational-databases.amp.html).

In general, a [Distributed SQL Database](https://en.m.wikipedia.org/wiki/Distributed_SQL) is a single logical database deployed across multiple physical nodes in a single data center or across many data centers if need be; all of which allow it to deliver elastic scale and bulletproof resilience.





[Original paper on Spanner](https://static.googleusercontent.com/media/research.google.com/en//archive/spanner-osdi2012.pdf) explains [details](https://thedataguy.in/internals-of-google-cloud-spanner/) of its design. 

## Architecture

A Spanner deployment is called a universe. Given that Spanner manages data globally, there will be only a handful of running universes.

Spanner is organized as a set of zones, where each zone is the rough analog of a deployment of [Bigtable](Bigtable) servers.

Zones are the unit of administrative deployment. The set of zones is also the set of locations across
which data can be replicated. 

Zones can be added to or removed from a running system as new datacenters are
brought into service and old ones are turned off, respectively. 

Zones are also the unit of physical isolation: there
may be one or more zones in a datacenter, for example, if different applications’ data must be partitioned across
different sets of servers in the same datacenter.

A zone has one zonemaster and between one hundred and several thousand spanservers. The former assigns
data to spanservers; the latter serve data to clients. 

The per-zone location proxies are used by clients to locate
the spanservers assigned to serve their data. The universe master and the placement driver are currently singletons. 

The universe master is primarily a console that displays status information about all the zones for interactive debugging. 


The placement driver handles automated movement of data across zones on the timescale of minutes. 

The placement driver periodically communicates with the spanservers to find data that needs to be moved, either to meet updated replication constraints or to balance load.

### Spanserver

At the bottom, each spanserver is responsible for between 100 and 1000 instances of a data structure called a tablet. 

A
tablet is similar to Bigtable’s tablet abstraction, in that it implements a bag of the following mappings:

```
  (key:string, timestamp:int64) → string

```

Unlike [Bigtable](Bigtable), Spanner assigns timestamps to data, which is an important way in which Spanner is more like a multi-version database than a key-value store.  


A tablet’s state is stored in set of [B-tree-like](https://en.m.wikipedia.org/wiki/B-tree) files and a write-ahead log, all on a distributed file system called
[Colossus](https://www.google.com/amp/s/cloudblog.withgoogle.com/products/storage-data-transfer/a-peek-behind-colossus-googles-file-system/amp/)  (the successor to the Google File System).  

To support replication, each spanserver implements a single [Paxos](https://www.cs.rutgers.edu/~pxk/417/notes/paxos.html)   state machine on top of each tablet.


The [Paxos](https://medium.com/distributed-knowledge/paxos-consensus-for-beginners-1b8519d3360f)    state machines are used to implement a consistently replicated bag of mappings. 

The key-value
mapping state of each replica is stored in its corresponding tablet. Writes must initiate the Paxos protocol at the
leader; reads access state directly from the underlying tablet at any replica that is sufficiently up-to-date. 

The
set of replicas is collectively a Paxos group. 

At every replica that is a leader, each spanserver implements a lock table to implement concurrency control. The lock table contains the state for two-phase locking: it maps ranges of keys to lock states.

### Split

Spanner is global database system, per region we’ll get minimum of 3 shards. 

Each shard will be in each zone. 

In Spanner terms a shard is called as Split. 

If your provision 1 Node Spanner cluster, you’ll get 2 more Nodes on the different zone which are invisible to you. 

And the Compute and Storage layers are de-coupled. Paxos algorithm is used to maintain one leader at a time and rest of the nodes will be the followers.

<img src="https://thedataguy.in/assets/Internals%20of%20Google%20Cloud%20Spanner1.jpg" width="600">

Based on the partitions, we’ll have more Splits(shards) in the storage layer. 

Each shard will be replicated to the other Zones. 

For eg: if you have a shard called S1 on Zone A, it’ll be replicated to Zone B and C. 

The replication works based on Leader follower method. 

So the Paxos will help to maintain the quorum and will help to select a new Leader during the failure. 

If you are writing something on this Split, the Spanner APIs are aware of the Leaders. 

So the write directly goes to the Zone where it has the Leader Split. 

Each Split has its own leader zone.



<img src="https://thedataguy.in/assets/Internals%20of%20Google%20Cloud%20Spanner2.jpg" width="600">



## Strong Consistency

Spanner, as most [ACID](https://en.m.wikipedia.org/wiki/ACID) databases, it uses the [2PC](https://en.m.wikipedia.org/wiki/Two-phase_commit_protocol) (Two phase commit), and it uses Paxos groups to mitigate the "anti-availability" shortcoming. 

At the highest level of abstraction, Spanner is a database that shards data across many sets of Paxos state machines in datacenters spread all over the world.

Spanner provides synchronous cross-datacenter replication and strong consistency and usability of traditional SQL databases. 

### Google F1 

[F1](https://research.google/pubs/pub41344/) is a distributed relational database built to support the Google AdWords business.  

F1 is built using Spanner to replace an implementation based on MySQL.

## External Consistency, Linearizability, Serializability

Cloud Spanner provides clients with the strictest concurrency-control guarantees for transactions, which is called external consistency. Under external consistency, the system behaves as if all transactions were executed sequentially, even though Cloud Spanner actually runs them across multiple servers (and possibly in multiple datacenters) for higher performance and availability. 

In addition if one transaction completes before another transaction starts to commit, the system guarantees that clients can never see a state that includes the effect of the second transaction but not the first. 

Intuitively, Cloud Spanner is semantically indistinguishable from a single-machine database. 

Even though it provides such strong guarantees, Cloud Spanner enables applications to achieve performance comparable to databases that provide weaker guarantees. 

Cloud Spanner provides [external consistency](https://www.youtube.com/watch?v=QdkS6ZjeR7Q), which is a stronger property than linearizability, because linearizability does not say anything about the behavior of transactions.

<img src="https://accelazh.github.io/images/ddia-linearizability.png" width="700">

Linearizability is a property of concurrent objects that support atomic read and write operations. 

In a database, an "object" would typically be a single row or even a single cell. 

External consistency is a property of transaction-processing systems, where clients dynamically synthesize transactions that contain multiple read and write operations on arbitrary objects. 


Cloud Spanner provides external [consistency](https://aphyr.com/posts/313-strong-consistency-models), which is a stricter property than serializability. 

A transaction-processing system is serializable if it executes transactions in a manner that is indistinguishable from a system in which the transactions are executed serially. 

Cloud Spanner also guarantees that the serial order is consistent with the order in which the transactions can be observed to commit.

In a system that provides serializability but not external consistency, even though the customer executed T1 and then T2 sequentially, the system would be permitted to reorder them, which could cause the debit to incur a penalty due to insufficient funds.





## TrueTime

Spanner is very keen in syncronizing and maintains the same time across all the nodes over the global datacenters. 

Their hardwares are built with Atomic Clocks to maintain the time. 

If you take a look at the Server Hardware Rack, the Server is having 4 time servers. 

2 Servers are connected with GPS and the remaining 2 are connect with Automic Oscillators. 

There are 2 different brands of Oscillators for better failover processing. 

The GPS time servers will sync with Oscillators to synchronize the time across the global datacenters with every 30sec interval.

<img src="https://thedataguy.in/assets/Internals%20of%20Google%20Cloud%20Spanner3.jpg" width="600">

TrueTime is a highly available, distributed clock that is provided to applications on all Google servers. 

TrueTime enables applications to generate monotonically increasing timestamps: an application can compute a timestamp T that is guaranteed to be greater than any timestamp T' if T' finished being generated before T started being generated. 

This guarantee holds across all servers and all timestamps.

[https://cloud.google.com/spanner/docs/true-time-external-consistency](https://cloud.google.com/spanner/docs/true-time-external-consistency)

<img src="https://thedataguy.in/assets/Internals%20of%20Google%20Cloud%20Spanner9.jpg" height="600">

https://www.youtube.com/watch?v=iKQhPwbzzxU


Some databases support similar timestamp capabilities [without TrueTime](https://www.cockroachlabs.com/blog/living-without-atomic-clocks/).








## Example: Build realtime inventory management systems with Cloud Spanner

Build  an inventory ledger solution that streamlines the order-to-shipping process using Cloud Spanner, a scalable, globally consistent database service. The single source of truth enables seamless customer experiences across channels and real-time decisioning at scale. 

[https://www.youtube.com/watch?v=8kj_uA5vJfo](https://www.youtube.com/watch?v=8kj_uA5vJfo)

## Migrating to Spanner

https://www.youtube.com/watch?v=FNeGQUqMa_c

## Migrating from Oracle OLTP to Cloud Spanner

https://cloud.google.com/architecture/migrating-oracle-to-cloud-spanner

## Tutorials

[https://cloud.google.com/spanner/docs/tutorials](https://cloud.google.com/spanner/docs/tutorials)

## Optimizing Applications, Schemas, and Query Design on Cloud Spanner

Discuss techniques for monitoring Cloud Spanner to identify performance bottlenecks. 

https://www.youtube.com/watch?v=DxrdatA_ULk

### Emulator

The [Cloud SDK](https://cloud.google.com/sdk) provides a local, in-memory emulator, which you can use to develop and test your applications for free without creating a GCP Project or a billing account. As the emulator stores data only in memory, all state, including data, schema, and configs, is lost on restart. The emulator offers the same APIs as the Cloud Spanner production service and is intended for local development and testing, not for production deployments.

The emulator supports all languages of the client libraries. You can also use the emulator with the gcloud command-line tool and REST APIs.

The emulator is also available as an open source project in [GitHub](https://github.com/GoogleCloudPlatform/cloud-spanner-emulator).

## Perspectives

[Big Data](Big-Data) technology evolves over time.








## Databases, ETL, ELT and tools.

[https://cube.dev/blog/category/data-stack/](https://cube.dev/blog/category/data-stack/)







## Qwiklabs


### Quick Start

[Cloud Spanner: Qwik Start](https://www.qwiklabs.com/focuses/1774?catalog_rank=%7B%22rank%22%3A1%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&parent=catalog&search_id=7467628)


### Java Client

In this lab, you will set up a Cloud Spanner instance, create a database and schema, then run sample queries on a dataset. Helpful Cloud Spanner information is provided along the way to help you get the most out of this powerful database service.

[Querying Cloud Spanner With a Java Client](https://www.qwiklabs.com/focuses/2189?catalog_rank=%7B%22rank%22%3A3%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&parent=catalog&search_id=7467628)


### Leaderboard

In this lab, you will learn how to set up a Cloud Spanner instance. You will go through the steps of creating a database and schema that can be used for a gaming leaderboard. You'll start by creating a Players table for storing player information and a Scores table to store player scores.

[Cloud Spanner: Create a Gaming Leaderboard with C#](https://www.qwiklabs.com/focuses/1815?catalog_rank=%7B%22rank%22%3A4%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&parent=catalog&search_id=7467628)


### Backend

In this lab, you develop a backend service for an online Quiz application to process user feedback and save scores.

[App Dev: Developing a Backend Service - Java](https://www.qwiklabs.com/focuses/1128?catalog_rank=%7B%22rank%22%3A9%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&parent=catalog&search_id=7467628)


### Python

This lab concentrates on the backend service, putting together Pub/Sub, Natural Language, and Spanner services and APIs to collect and analyze feedback and scores from an online Quiz application.

[App Dev: Developing a Backend Service - Python](https://www.qwiklabs.com/focuses/1107?catalog_rank=%7B%22rank%22%3A10%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&parent=catalog&search_id=7467628)
