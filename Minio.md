# MinIO quickstart


MinIO is a High Performance Object Storage released under Apache License v2.0. It is API compatible with Amazon S3 cloud storage service. Use MinIO to build high performance infrastructure for machine learning, analytics and application data workloads.


https://docs.min.io/docs/minio-quickstart-guide.html

MinIO is a cloud-native application designed to scale in a sustainable manner in multi-tenant environments. Orchestration platforms provide perfect launchpad for MinIO to scale

https://docs.min.io/docs/minio-deployment-quickstart-guide.html

MinIO Client (mc) provides a modern alternative to UNIX commands like ls, cat, cp, mirror, diff, find etc. It supports filesystems and Amazon S3 compatible cloud storage service (AWS Signature v2 and v4).

https://docs.min.io/docs/minio-client-quickstart-guide.html

# Erasure Code

MinIO protects data against hardware failures and silent data corruption using erasure code and checksums. With the highest level of redundancy, you may lose up to half (N/2) of the total drives and still be able to recover the data.

https://docs.min.io/docs/minio-erasure-code-quickstart-guide.html

### Reed-Solomon

Erasure code is a mathematical algorithm to reconstruct missing or corrupted data. MinIO uses Reed-Solomon code to shard objects into variable data and parity blocks. For example, in a 12 drive setup, an object can be sharded to a variable number of data and parity blocks across all the drives - ranging from six data and six parity blocks to ten data and two parity blocks.


# Distributed MinIO

MinIO in distributed mode lets you pool multiple drives (even on different machines) into a single object storage server. As drives are distributed across several nodes, distributed MinIO can withstand multiple node failures and yet ensure full data protection.


https://docs.min.io/docs/distributed-minio-quickstart-guide.html

# Kubernetes

https://docs.min.io/docs/deploy-minio-on-kubernetes.html

# MinIO and TLS

https://docs.min.io/docs/how-to-secure-access-to-minio-server-with-tls.html

# Server side encryption

https://docs.min.io/docs/minio-security-overview.html

# SDK
https://docs.min.io/docs/golang-client-quickstart-guide.html

# Multi-tenant
https://docs.min.io/docs/multi-tenant-minio-deployment-guide.html

# disaggregated Spark and Hadoop Hive with MinIO

https://docs.min.io/docs/disaggregated-spark-and-hadoop-hive-with-minio.html

# Cookbooks

https://docs.min.io/docs/minio-client-quickstart-guide.html

# JuiceFS

JuiceFS is a POSIX-compatible shared filesystem specifically designed to work in the cloud.

https://juicefs.com/?hl=en
