

## Database Related topics

There are many GCP databases: [BigQuery](BigQuery), [Bigtable](Bigtable), [Cloud SQL](  Cloud-SQL 
 ), [Datastore](Datastore), [Firebase](Firebase), [Firestore](Firestore), [Spanner](Spanner), and [Memorystore](Memorystore).

### Cloud Databases

* [GCP Database Products](https://cloud.google.com/products/databases)
* [AWS Database products](https://aws.amazon.com/products/databases/) 
* [Azure databases](https://azure.microsoft.com/en-us/product-categories/databases/)
* [Oracle databases](https://www.oracle.com/database/)
* [IBM  DB2 database](https://www.ibm.com/cloud/db2-on-cloud)
* [SAP HANA Cloud](   https://www.sap.com/products/hana/cloud.html )

### SQL, NoSQL, NewSQL, distributed SQL

[Structured Query Language](SQL) (SQL) is the standard language for data manipulation in a DBMS.

A [NoSQL](https://en.wikipedia.org/wiki/NoSQL) (originally referring to "non-SQL" or "non-relational") database provides a mechanism for storage and retrieval of data that is modeled in means other than the tabular relations used in relational databases. Such databases have existed since the late 1960s, but the name "NoSQL" was only coined in the early 21st century, triggered by the needs of Web 2.0 companies. NoSQL databases are increasingly used in big data and real-time web applications. NoSQL systems are also sometimes called "Not only SQL" to emphasize that they may support SQL-like query languages or sit alongside SQL databases in polyglot-persistent architectures.

[NewSQL](https://en.wikipedia.org/wiki/NewSQL) is a class of relational database management systems that seek to provide the scalability of NoSQL systems for online transaction processing (OLTP) workloads while maintaining the ACID guarantees of a traditional database system.

[https://www.virtual-dba.com/differences-between-sql-nosql-and-newsql/](https://www.virtual-dba.com/differences-between-sql-nosql-and-newsql/)


Many enterprise systems that handle high-profile data (e.g., financial and order processing systems) are too large for conventional relational databases, but have transactional and consistency requirements that are not practical for NoSQL systems. The only options previously available for these organizations were to either purchase more powerful computers or to develop custom middleware that distributes requests over conventional DBMS. Both approaches feature high infrastructure costs and/or development costs. NewSQL systems attempt to reconcile the conflicts.

[HTAP](https://en.wikipedia.org/wiki/Hybrid_transactional/analytical_processing)  is an emerging application architecture that "breaks the wall" between transaction processing and analytics. It enables more informed and "in business real time" decision making. It may combine support for both [OLTP](https://en.wikipedia.org/wiki/Online_transaction_processing) and [OLAP](https://en.wikipedia.org/wiki/Online_analytical_processing).


[https://www.youtube.com/watch?v=ZS_kXvOeQ5Y](https://www.youtube.com/watch?v=ZS_kXvOeQ5Y)


A [distributed SQL](https://en.wikipedia.org/wiki/Distributed_SQL) database is a single relational database which [replicates data across multiple servers](https://www.infoworld.com/article/3564543/beyond-nosql-the-case-for-distributed-sql.html). [Distributed SQL](https://www.cockroachlabs.com/blog/what-is-distributed-sql/) databases are strongly consistent and most [support consistency](https://www.nextplatform.com/2021/01/25/after-three-decades-you-can-finally-have-a-distributed-sql-database/) across racks, data centers, and wide area networks including cloud availability zones and cloud geographic zones.

### Databases vs file systems

https://www.guru99.com/difference-between-file-system-and-dbms.html

### OLTP vs. OLAP

https://www.holistics.io/blog/the-rise-and-fall-of-the-olap-cube/

### ELT vs ETL

https://www.informatica.com/blogs/etl-vs-elt-whats-the-difference.html

### Data lakes vs Data warehouses

https://aws.amazon.com/big-data/datalakes-and-analytics/what-is-a-data-lake/

### ACID, BASE, CAP

A database transaction can be either a single operation or a sequence of operations, but is treated as a single logical operation on the data by the database. The properties of these transactions provide certain guarantees to the application developer. The acronym ACID was coined by Andreas Reuter and Theo Härder in 1983 to describe them.

[https://medium.com/@pranabj.aec/acid-cap-and-base-cc73dee43f8c](https://medium.com/@pranabj.aec/acid-cap-and-base-cc73dee43f8c)

The CAP theorem dictates that the three desirable properties, consistency, availability and partition tolerance cannot be offered simultaneously. Let’s study if its possible to achieve two of these three properties.



http://dist-prog-book.com/chapter/6/acidic-to-basic-how-the-database-ph-has-changed.html

### Serializability, linearizability, and locality

[https://aphyr.com/posts/333-serializability-linearizability-and-locality](https://aphyr.com/posts/333-serializability-linearizability-and-locality)

Linearizability (also known as atomic consistency, strong consistency, immediate consistency) describes reads and writes on a single object (stores a single value). it doesn’t involve multiple objects. It doesn’t involve “transaction”, which groups multiple objects. It treats each operation as an atom, i.e. to take effect in a single time point, rather than a timespan.

https://accelazh.github.io/storage/Linearizability-Vs-Serializability-And-Distributed-Transactions-Copy


Serializability is an isolation level for database transactions. It comes from database community area, where is a different area that Linearizability originates.

Serializability describes multiple transactions, where a transaction is usually composed of multiple operations on multiple objects.



### Distributed Consensus Protocols

A logical clock is an idea put forward by Lamport in 1987 to solve possible problems caused by clock inconsistency between different machines in a distributed system. 

[https://www.alibabacloud.com/blog/a-brief-analysis-of-consensus-protocol-from-logical-clock-to-raft_594675](https://www.alibabacloud.com/blog/a-brief-analysis-of-consensus-protocol-from-logical-clock-to-raft_594675)

Many distributed systems use state machine replication to synchronize data between copies, such as HDFS, Chubby, and Zookeeper.
Paxos is a consensus protocol algorithm developed by Lamport in the 1990s. ZAB (ZooKeeper Atomic BoardCast) is a consensus protocol used in ZooKeeper. Raft is a new consensus protocol developed by developers at Stanford University in 2014. The developers developed this new consensus protocol because they considered Paxos difficult to understand.

https://www.sofastack.tech/en/projects/sofa-jraft/consistency-raft-jraft/


Currently, the improved Paxos protocol has been used in many distributed products, such as Chubby, PaxosStore, Alibaba Cloud X-DB, and Ant Financial OceanBase. It is generally believed that the Raft protocol has lower performance than Paxos because it only allows committing entries in sequence. However, TiKV that uses Raft officially declares that it has made many optimizations on Raft and has significantly improved the performance of Raft. POLARDB is another Alibaba Cloud database that also uses Parallel-Raft (the improved version of Raft) to implement the parallel commit capability in Raft. I believe that more Paxos/Raft-based products will be available in the future and that more improvements will be made to Raft/Paxos.



https://www.hashicorp.com/resources/raft-consul-consensus-protocol-explained

Raft works by electing a leader in the cluster. The leader is responsible for accepting client requests and managing the replication of the log to other servers. The data flows only in one direction: from leader to other servers.


https://www.freecodecamp.org/news/in-search-of-an-understandable-consensus-algorithm-a-summary-4bc294c97e0d/

Raft uses randomized election timeouts to ensure that split votes are rare and that they are resolved quickly. To prevent split votes in the first place, election timeouts are chosen randomly from a fixed interval (e.g., 150–300ms). This spreads out the servers so that in most cases only a single server will time out; it wins the election and sends heartbeats before any other servers time out. The same mechanism is used to handle split votes. Each candidate restarts its randomized election timeout at the start of an election, and it waits for that timeout to elapse before starting the next election; this reduces the likelihood of another split vote in the new election.

https://www.geeksforgeeks.org/raft-consensus-algorithm/

In Raft, the leader handles inconsistencies by forcing the followers’ logs to duplicate its own. This means that conflicting entries in follower logs will be overwritten with entries from the leader’s log.

### DHT, CRDT and Models for relaxed Consistency

Many real-world systems, even global financial networks, choose availability over consistency, so that people can get on with business. There are different ways to go about this. Some of them, based on ‘coordination protocols’ are complicated to get right; they involve all sorts of special roles and rules.

A [distributed hash table](https://en.wikipedia.org/wiki/Distributed_hash_table) (DHT) is a distributed system that provides a lookup service similar to a hash table: key-value pairs are stored in a DHT, and any participating node can efficiently retrieve the value associated with a given key. 

A [conflict-free replicated data type](https://en.wikipedia.org/wiki/Conflict-free_replicated_data_type) (CRDT) is a data structure which can be replicated across multiple computers in a network, where the replicas can be updated independently and concurrently without coordination between the replicas, and where it is always mathematically possible to resolve inconsistencies that might come up.

CRDTs let you avoid conflict by defining rules about how changes are applied to a single data point.

http://dist-prog-book.com/chapter/7/langs-consistency.html

https://hackmd.io/@XYOAnQcjRD-lWNVnC2p2GA/S1KpBgA0V

### Redis CRDT


https://redis.com/redis-enterprise/technology/active-active-geo-distribution/

### Distributed Systems

https://github.com/bobbae/gcp/wiki/Fallacies#8-fallacies-of-distributed-computing

### Database of Databases

[https://dbdb.io/browse](https://dbdb.io/browse)

