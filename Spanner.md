# Spanner

## Introduction 

Cloud Spanner is a fully managed, mission-critical, relational database service that offers transactional consistency at global scale, schemas, SQL (ANSI 2011 with extensions), and automatic, synchronous replication for high availability.

[https://cloud.google.com/spanner/docs](https://cloud.google.com/spanner/docs)

Original paper on Spanner. 

[https://static.googleusercontent.com/media/research.google.com/en//archive/spanner-osdi2012.pdf](https://static.googleusercontent.com/media/research.google.com/en//archive/spanner-osdi2012.pdf)


## External Consistency, Linearizability, Serializability

Cloud Spanner provides clients with the strictest concurrency-control guarantees for transactions, which is called external consistency. Under external consistency, the system behaves as if all transactions were executed sequentially, even though Cloud Spanner actually runs them across multiple servers (and possibly in multiple datacenters) for higher performance and availability. In addition if one transaction completes before another transaction starts to commit, the system guarantees that clients can never see a state that includes the effect of the second transaction but not the first. Intuitively, Cloud Spanner is semantically indistinguishable from a single-machine database. Even though it provides such strong guarantees, Cloud Spanner enables applications to achieve performance comparable to databases that provide weaker guarantees. 

Cloud Spanner provides external consistency, which is a stronger property than linearizability, because linearizability does not say anything about the behavior of transactions.

Linearizability is a property of concurrent objects that support atomic read and write operations. In a database, an "object" would typically be a single row or even a single cell. External consistency is a property of transaction-processing systems, where clients dynamically synthesize transactions that contain multiple read and write operations on arbitrary objects. Linearizability can be viewed as a special case of external consistency, where a transaction can only contain a single read or write operation on a single object.

Cloud Spanner provides external consistency, which is a stricter property than serializability. A transaction-processing system is serializable if it executes transactions in a manner that is indistinguishable from a system in which the transactions are executed serially. Cloud Spanner also guarantees that the serial order is consistent with the order in which the transactions can be observed to commit.

In a system that provides serializability but not external consistency, even though the customer executed T1 and then T2 sequentially, the system would be permitted to reorder them, which could cause the debit to incur a penalty due to insufficient funds.

https://aphyr.com/posts/313-strong-consistency-models

## TrueTime

TrueTime is a highly available, distributed clock that is provided to applications on all Google servers. TrueTime enables applications to generate monotonically increasing timestamps: an application can compute a timestamp T that is guaranteed to be greater than any timestamp T' if T' finished being generated before T started being generated. This guarantee holds across all servers and all timestamps.

[https://cloud.google.com/spanner/docs/true-time-external-consistency](https://cloud.google.com/spanner/docs/true-time-external-consistency)


## Cloud Spanner 101

[https://www.youtube.com/watch?v=IfsTINNCooY](https://www.youtube.com/watch?v=IfsTINNCooY)

Cloud Spanner is a fully managed relational database with unlimited scale, strong consistency, and up to 99.999% availability. Cloud Spanner can help you create time-sensitive, mission critical applications at scale. 

[https://www.youtube.com/watch?v=5bjYk6Hhd10](https://www.youtube.com/watch?v=5bjYk6Hhd10)

Build  an inventory ledger solution that streamlines the order-to-shipping process using Cloud Spanner, a scalable, globally consistent database service. The single source of truth enables seamless customer experiences across channels and real-time decisioning at scale. 

[https://www.youtube.com/watch?v=8kj_uA5vJfo](https://www.youtube.com/watch?v=8kj_uA5vJfo)


#### Tutorials

[https://cloud.google.com/spanner/docs/tutorials](https://cloud.google.com/spanner/docs/tutorials)


## Perspectives

A Shift to Distributed SQL.

[https://medium.com/@garyorenstein/the-shift-to-distributed-sql-232c04dec1f7](https://medium.com/@garyorenstein/the-shift-to-distributed-sql-232c04dec1f7)

Databases, ETL, ELT and tools.

[https://cube.dev/blog/category/data-stack/](https://cube.dev/blog/category/data-stack/)


## Qwiklabs


##### Quick Start

[Cloud Spanner: Qwik Start](https://www.qwiklabs.com/focuses/1774?catalog_rank=%7B%22rank%22%3A1%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&parent=catalog&search_id=7467628)


##### Java Client

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
