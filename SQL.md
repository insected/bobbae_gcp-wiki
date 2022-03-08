[Structured Query Language](   https://wikipedia.org/wiki/SQL ) (SQL) is the standard language for data manipulation in a [database](Databases). [Structured Query Language](https://en.wikipedia.org/wiki/SQL) is a domain-specific language used in programming and designed for managing data held in a [relational database management system](https://en.wikipedia.org/wiki/Relational_database#RDBMS) .


### Data Definition Language

[Data Definition Language](https://en.wikipedia.org/wiki/Data_definition_language) (DDL) allows you to create objects like Schemas, Tables in the database.

### Data Control Language

[Data Control Language](https://en.wikipedia.org/wiki/Data_control_language) (DCL) allows you to manipulate and manage access rights on database objects.

### Data Manipulation Language

[Data Manipulation Language](https://en.wikipedia.org/wiki/Data_manipulation_language) (DML) is used for searching, inserting, updating, and deleting data.

### Quickstart using Cloud SQL

https://cloud.google.com/sql/docs/mysql/quickstart

## Relational Databases

A [relational database](https://en.wikipedia.org/wiki/Relational_database
) is a digital database based on the relational model of data, as proposed by E. F. Codd in 1970. A software system used to maintain relational databases is a [relational database management system](https://en.wikipedia.org/wiki/Relational_database#RDBMS) (RDBMS). Many relational database systems have an option of using the SQL  for querying and maintaining the database.



### CloudSQL

[CloudSQL](CloudSQL)  is a fully managed service that makes it easy to set up, manage, and administer relational databases: PostgreSQL, MySQL, and SQL Server.

### BigQuery

[BigQuery](BigQuery)  is Google Cloud's [fully managed](https://www.youtube.com/watch?v=kKBnFsNWwYM), petabyte-scale, and  analytics [data warehouse](https://cloud.google.com/solutions/bigquery-data-warehouse)  that lets you run [analytics over vast amounts](https://cloud.google.com/blog/topics/developers-practitioners/bigquery-explained-blog-series)  of data in near real time. 

### Spanner

[Cloud Spanner](Spanner) is a  [managed relational database](https://www.youtube.com/watch?v=IFbydfGV2lQ) with [unlimited scale, strong consistency, and up to 99.999% availability](https://www.youtube.com/watch?v=5bjYk6Hhd10). 

### Similar to SQL

Incomplete SQL compatible implementations.

#### SQL on Hadoop

Apache Hive, Sqoop, Impala, Drill, Phoenix, Spark SQL. Presto, CitusData, Jethro, HAWQ, Big SQL, PolyBase, 

https://www.xplenty.com/blog/12-sql-on-hadoop-tools/


#### KQL

https://squaredup.com/blog/kusto-101-a-jumpstart-guide-to-kql/


#### CQL

https://cassandra.apache.org/doc/latest/cassandra/cql/

#### HiveQL

https://www.tutorialspoint.com/hive/hiveql_select_where.htm


#### Spark SQL

https://spark.apache.org/sql/

#### Apache Drill

https://drill.apache.org/

#### Presto

https://prestodb.io/

#### Apache Impala

https://impala.apache.org/

#### Apache Phoenix

https://phoenix.apache.org/

#### Apache Kudu

https://kudu.apache.org/

#### Apache Hue

https://github.com/cloudera/hue

### SQL Alternatives

https://en.wikipedia.org/wiki/SQL#Alternatives

## NewSQL

[NewSQL](https://en.wikipedia.org/wiki/NewSQL) databases retained all the aspects of the relational model, the predefined schema and the use of SQL, and sought to solve the problem of scale either in-memory or  clever distributed architecture.  In the latter case it may be referred to as [Distributed SQL](https://www.cockroachlabs.com/blog/what-is-distributed-sql/
).



### Distributed SQL

[Distributed SQL](https://en.wikipedia.org/wiki/Distributed_SQL) is a single logical database deployed across multiple physical nodes in a single data center or across many data centers to deliver elastic scale and resilience.

https://www.cockroachlabs.com/blog/what-is-distributed-sql/


## NoSQL

[NoSQL](https://en.wikipedia.org/wiki/NoSQL) databases  are non tabular, and store data differently than relational tables. NoSQL databases come in a variety of types based on their data model and provide flexible schemas and scale easily with large amounts of data and high user loads.

### Types of NoSQL databases

#### Document database

[Document oriented databases](https://en.wikipedia.org/wiki/Document-oriented_database) store data in documents similar to JSON (JavaScript Object Notation) objects. Each document contains pairs of fields and values. The values can typically be a variety of types including things like strings, numbers, booleans, arrays, or objects. Examples: MongoDB, Datastore, Firestore, Couchbase, Elasticsearch.

#### Key value database

[Key-value databases](https://en.wikipedia.org/wiki/Key%E2%80%93value_database) are a simpler type of database where each item contains keys and values. A value can typically only be retrieved by referencing its key, so learning how to query for a specific key-value pair is typically simple. Key-value databases are great for use cases where you need to store large amounts of data. Examples: Redis, LMDB, LevelDB, Riak

#### Wide column database

[Wide-column stores](https://en.wikipedia.org/wiki/Wide-column_store) store data in tables, rows, and dynamic columns. Wide-column stores provide a lot of flexibility over relational databases because each row is not required to have the same columns. Many consider wide-column stores to be two-dimensional key-value databases. Wide-column stores are great for when you need to store large amounts of data and you can predict what your query patterns will be. Examples: Cassandra, Bigtable, HBase, DynamoDB

#### Graph database


[Graph databases](https://en.wikipedia.org/wiki/Graph_database) store data in nodes and edges. Nodes typically store information about people, places, and things while edges store information about the relationships between the nodes. Graph databases excel in use cases where you need to traverse relationships to look for patterns such as social networks, fraud detection, and recommendation engines. Examples are [Neo4j](https://en.wikipedia.org/wiki/Neo4j), [AWS Neptune](https://en.wikipedia.org/wiki/Amazon_Neptune), [JanusGraph](https://en.wikipedia.org/wiki/JanusGraph) and [AllegroGraph](https://en.wikipedia.org/wiki/AllegroGraph).

### Neo4j Aura on Google cloud

https://neo4j.com/cloud/aura-google-cloud/

## GraphQL

[GraphQL](  GraphQL ) is a query language for APIs and a runtime for fulfilling the queries with your existing data. 

## SQL Related tools

### Sqlcommenter

https://cloud.google.com/blog/topics/developers-practitioners/introducing-sqlcommenter-open-source-orm-auto-instrumentation-library

### SQL and Dataframe

https://towardsdatascience.com/sql-jinja-is-not-enough-why-we-need-dataframes-4d71a191936d

### Cloud SQL Insights

https://cloud.google.com/blog/products/databases/get-ahead-of-database-performance-issues-with-cloud-sql-insights

### New Relic

https://docs.newrelic.com/docs/integrations/google-cloud-platform-integrations/gcp-integrations-list/google-cloud-sql-monitoring-integration/

## SQL Tutorials


- https://www.coursera.org/learn/sql-for-data-science
- https://www.w3schools.com/sql/
- https://www.guru99.com/sql.html
- https://www.tutorialspoint.com/sql/index.htm
- https://www.youtube.com/watch?v=HXV3zeQKqGY
- https://www.khanacademy.org/computing/computer-programming/sql

### SQL Examples

https://sqlzoo.net/

### Qwiklabs

https://www.qwiklabs.com/quests/52/

