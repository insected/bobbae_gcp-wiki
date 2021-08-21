

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


### OLTP vs. OLAP

https://www.holistics.io/blog/the-rise-and-fall-of-the-olap-cube/

### ACID, BASE, CAP

[https://medium.com/@pranabj.aec/acid-cap-and-base-cc73dee43f8c](https://medium.com/@pranabj.aec/acid-cap-and-base-cc73dee43f8c)

http://dist-prog-book.com/chapter/6/acidic-to-basic-how-the-database-ph-has-changed.html

### Serializability, linearizability, and locality

[https://aphyr.com/posts/333-serializability-linearizability-and-locality](https://aphyr.com/posts/333-serializability-linearizability-and-locality)


https://accelazh.github.io/storage/Linearizability-Vs-Serializability-And-Distributed-Transactions-Copy

### Distributed Consensus Protocols

[https://www.alibabacloud.com/blog/a-brief-analysis-of-consensus-protocol-from-logical-clock-to-raft_594675](https://www.alibabacloud.com/blog/a-brief-analysis-of-consensus-protocol-from-logical-clock-to-raft_594675)

https://www.sofastack.tech/en/projects/sofa-jraft/consistency-raft-jraft/

https://www.hashicorp.com/resources/raft-consul-consensus-protocol-explained


https://www.geeksforgeeks.org/raft-consensus-algorithm/

### DHT, CRDT and Models for relaxed Consistency

http://dist-prog-book.com/chapter/7/langs-consistency.html


### Distributed Systems

https://github.com/bobbae/gcp/wiki/Fallacies#8-fallacies-of-distributed-computing

### Database of Databases

[https://dbdb.io/browse](https://dbdb.io/browse)

