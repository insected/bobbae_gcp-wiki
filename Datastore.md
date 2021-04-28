# Introduction

Datastore is a highly scalable NoSQL database for your applications. Datastore automatically handles sharding and replication, providing you with a highly available and durable database that scales automatically to handle your applications' load. Datastore provides a myriad of capabilities such as ACID transactions, SQL-like queries and indexes.  Cloud Datastore is built upon Google's Bigtable and Megastore technology. Datastore allows the user to create databases either in Native or Datastore Mode. Native Mode is designed for mobile and web apps, while Datastore Mode is designed for new server projects. Originally released as a feature in Google App Engine in 2008, Cloud Datastore was announced as a standalone product in 2013 during Google I/O. In 2018 at the Google Cloud Next conference, the second-generation Firestore database was opened to general availability, with a backward-compatibility mode. Google provides a path for automatically upgrading a legacy Datastore database to Firestore in Datastore mode. Cloud Datastore database has a SQL-like syntax called "GQL" (Google Query Language). GQL does not support the Join statement. Instead, one-to-many and many-to-many relationships can be accomplished using ReferenceProperty(). This shared-nothing approach allows disks to fail without the system failing. Switching from a relational database to Cloud Datastore requires a paradigm shift for developers when modeling their data.

https://cloud.google.com/datastore

# Firestore in Datastore mode

Firestore in Datastore mode is a NoSQL document database built for automatic scaling, high performance, and ease of application development.

Firestore is the newest version of Datastore and introduces [several improvements over Datastore](https://cloud.google.com/datastore/docs/firestore-or-datastore#in_native_mode). 

Existing Datastore users can access these improvements by creating a new Firestore in Datastore mode database instance. In the future, all existing Datastore databases will be [automatically upgraded to Firestore in Datastore mode](https://cloud.google.com/datastore/docs/upgrade-to-firestore).

While the Datastore mode interface has many of the same features as traditional databases, as a NoSQL database it differs from them in the way it describes relationships between data objects.

[https://cloud.google.com/datastore/docs](https://cloud.google.com/datastore/docs)

More explanations.

[https://www.youtube.com/watch?v=SYG-BgXoJFQ](https://www.youtube.com/watch?v=SYG-BgXoJFQ)

# Comparisons

## Azure Cosmos DB

Azure Cosmos DB is Microsoft's proprietary globally-distributed, multi-model database service "for managing data at planet-scale". It is schema-agnostic, horizontally scalable and generally classified as a NoSQL database.

https://azure.microsoft.com/en-us/services/cosmos-db/

## Amazon DynamoDB

Amazon DynamoDB is a fully managed proprietary NoSQL database service that supports key–value and document data structures.  DynamoDB exposes a similar data model to and derives its name from Dynamo, but has a different underlying implementation. Dynamo had a multi-leader design requiring the client to resolve version conflicts and DynamoDB uses synchronous replication across multiple data centers for high durability and availability.  It is presented as a evolution of Amazon SimpleDB.

https://aws.amazon.com/dynamodb/

## Amazon SimpleDB

Amazon SimpleDB is a distributed database written in Erlang by Amazon.com. It is used as a web service in concert with Amazon Elastic Compute Cloud (EC2) and Amazon S3 and is part of Amazon Web Services. 

https://aws.amazon.com/simpledb/

## Datastax Astra

DataStax Astra is a cloud-native Cassandra-as-a-Service Built on Apache Cassandra designed to simplify cloud-native application development.

https://www.datastax.com/products/datastax-astra

## MongoDB

MongoDB is a general purpose, document-based, distributed database built for modern application developers.

https://www.mongodb.com/
