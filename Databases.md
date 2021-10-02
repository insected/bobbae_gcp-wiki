https://en.wikipedia.org/wiki/Database

## GCP Databases


There are many GCP databases: [BigQuery](BigQuery), [Bigtable](Bigtable), [Cloud SQL](  Cloud-SQL 
 ), [Datastore](Datastore), [Firebase](Firebase), [Firestore](Firestore), [Spanner](Spanner), and [Memorystore](Memorystore).

## Cloud Databases

* [GCP Database Products](https://cloud.google.com/products/databases)
* [AWS Database products](https://aws.amazon.com/products/databases/) 
* [Azure databases](https://azure.microsoft.com/en-us/product-categories/databases/)
* [Oracle databases](https://www.oracle.com/database/)
* [IBM  DB2 database](https://www.ibm.com/cloud/db2-on-cloud)
* [SAP HANA Cloud](   https://www.sap.com/products/hana/cloud.html )


## Database paradigms

https://www.youtube.com/watch?v=W2Z7fbCLSTw


## SQL, NoSQL, NewSQL

[Structured Query Language](SQL) (SQL) is the standard language for data manipulation in a DBMS.

A [NoSQL](https://en.wikipedia.org/wiki/NoSQL) (originally referring to "non-SQL" or "non-relational") database provides a mechanism for storage and retrieval of data that is modeled in means other than the tabular relations used in relational databases. Such databases have existed since the late 1960s, but the name "NoSQL" was only coined in the early 21st century, triggered by the needs of Web 2.0 companies. NoSQL databases are increasingly used in big data and real-time web applications. NoSQL systems are also sometimes called "Not only SQL" to emphasize that they may support SQL-like query languages or sit alongside SQL databases in polyglot-persistent architectures.

[NewSQL](https://en.wikipedia.org/wiki/NewSQL) is a class of relational database management systems that seek to provide the scalability of NoSQL systems for online transaction processing (OLTP) workloads while maintaining the ACID guarantees of a traditional database system.

[https://www.virtual-dba.com/differences-between-sql-nosql-and-newsql/](https://www.virtual-dba.com/differences-between-sql-nosql-and-newsql/)


Many enterprise systems that handle high-profile data (e.g., financial and order processing systems) are too large for conventional relational databases, but have transactional and consistency requirements that are not practical for NoSQL systems. The only options previously available for these organizations were to either purchase more powerful computers or to develop custom middleware that distributes requests over conventional DBMS. Both approaches feature high infrastructure costs and/or development costs. NewSQL systems attempt to reconcile the conflicts.

[HTAP](https://en.wikipedia.org/wiki/Hybrid_transactional/analytical_processing)  is an emerging application architecture that "breaks the wall" between transaction processing and analytics. It enables more informed and "in business real time" decision making. It may combine support for both [OLTP](https://en.wikipedia.org/wiki/Online_transaction_processing) and [OLAP](https://en.wikipedia.org/wiki/Online_analytical_processing).


[https://www.youtube.com/watch?v=ZS_kXvOeQ5Y](https://www.youtube.com/watch?v=ZS_kXvOeQ5Y)


A [distributed SQL](https://en.wikipedia.org/wiki/Distributed_SQL) database is a single relational database which [replicates data across multiple servers](https://www.infoworld.com/article/3564543/beyond-nosql-the-case-for-distributed-sql.html). [Distributed SQL](https://www.cockroachlabs.com/blog/what-is-distributed-sql/) databases are strongly consistent and most [support consistency](https://www.nextplatform.com/2021/01/25/after-three-decades-you-can-finally-have-a-distributed-sql-database/) across racks, data centers, and wide area networks including cloud availability zones and cloud geographic zones.

## Databases vs file systems

https://www.guru99.com/difference-between-file-system-and-dbms.html

## OLTP vs. OLAP

https://www.holistics.io/blog/the-rise-and-fall-of-the-olap-cube/

## ELT vs ETL

https://www.informatica.com/blogs/etl-vs-elt-whats-the-difference.html

## Data lakes vs Data warehouses

https://aws.amazon.com/big-data/datalakes-and-analytics/what-is-a-data-lake/

## ACID, BASE, CAP

A database transaction can be either a single operation or a sequence of operations, but is treated as a single logical operation on the data by the database. The properties of these transactions provide certain guarantees to the application developer. The acronym ACID was coined by Andreas Reuter and Theo Härder in 1983 to describe them.

[https://medium.com/@pranabj.aec/acid-cap-and-base-cc73dee43f8c](https://medium.com/@pranabj.aec/acid-cap-and-base-cc73dee43f8c)

The CAP theorem dictates that the three desirable properties, consistency, availability and partition tolerance cannot be offered simultaneously. Let’s study if its possible to achieve two of these three properties.



http://dist-prog-book.com/chapter/6/acidic-to-basic-how-the-database-ph-has-changed.html

## Serializability, linearizability, and locality

[https://aphyr.com/posts/333-serializability-linearizability-and-locality](https://aphyr.com/posts/333-serializability-linearizability-and-locality)

Linearizability (also known as atomic consistency, strong consistency, immediate consistency) describes reads and writes on a single object (stores a single value). it doesn’t involve multiple objects. It doesn’t involve “transaction”, which groups multiple objects. It treats each operation as an atom, i.e. to take effect in a single time point, rather than a timespan.

https://accelazh.github.io/storage/Linearizability-Vs-Serializability-And-Distributed-Transactions-Copy


Serializability is an isolation level for database transactions. It comes from database community area, where is a different area that Linearizability originates.

Serializability describes multiple transactions, where a transaction is usually composed of multiple operations on multiple objects.

## MVCC


Multiversion concurrency control (MCC or MVCC), is a concurrency control method commonly used by database management systems to provide concurrent access to the database and in programming languages to implement transactional memory.

https://wikipedia.org/wiki/Multiversion_concurrency_control


## Distributed Consensus Protocols

[Distributed consensus problem](Distributed-Consensus) requires agreement among a number of processes (or agents) for a single data value. Some of the processes (agents) may fail or be unreliable in other ways, so consensus protocols must be fault tolerant or resilient. 


## Database of Databases

[https://dbdb.io/browse](https://dbdb.io/browse)

