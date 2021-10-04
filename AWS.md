https://en.wikipedia.org/wiki/Amazon_Web_Services

[AWS](https://aws.amazon.com) is a subsidiary of Amazon providing on-demand cloud computing platforms and APIs on a metered pay-as-you-go basis. 

https://en.wikipedia.org/wiki/Amazon_Web_Services

## AWS services

https://www.youtube.com/watch?v=JIbIYCM48to

## GCP Fundamentals for AWS Professionals

https://google.qwiklabs.com/courses/1601

## Getting started with AWS

https://aws.amazon.com/getting-started/


### IAM
https://aws.amazon.com/iam/


## Overview of AWS

https://docs.aws.amazon.com/whitepapers/latest/aws-overview/amazon-web-services-cloud-platform.html



## Comparison of AWS, GCP and Azure

https://cloud.google.com/free/docs/aws-azure-gcp-service-comparison


## Compute Services

https://docs.aws.amazon.com/whitepapers/latest/aws-overview/compute-services.html

### Amazon EC2

[Amazon Elastic Compute Cloud](https://aws.amazon.com/ec2/) (Amazon EC2) is a web service that provides secure, resizable compute capacity in the cloud. 


### Amazon Lightsail

[Amazon Lightsail](https://amazonlightsail.com/) is designed to be the easiest way to launch and manage a virtual private server with AWS. Lightsail plans include everything you need to jumpstart your project – a virtual machine, SSD-based storage, data transfer, DNS management, and a static IP address.



### AWS App Runner

AWS App Runner is a fully managed service that makes it easy for developers to quickly deploy containerized web applications and APIs.


https://aws.amazon.com/apprunner/


### AWS Batch

[AWS Batch](https://aws.amazon.com/batch
) dynamically provisions the optimal quantity and type of compute resources (e.g., CPU or memory-optimized instances) based on the volume and specific resource requirements of the batch jobs submitted.  AWS Batch plans, schedules, and runs your batch computing workloads across the full range of AWS compute services and features, such as [Amazon Fargate](https://aws.amazon.com/fargate/), [Amazon EC2](https://aws.amazon.com/ec2/) and [Spot Instances](https://aws.amazon.com/ec2/spot/).



### AWS Elastic Beanstalk

[AWS Elastic Beanstalk](https://aws.amazon.com/elasticbeanstalk/
) is an easy-to-use service for deploying and scaling web applications and services developed with Java, .NET, PHP, Node.js, Python, Ruby, Go, and Docker on familiar servers such as Apache, Nginx, Passenger, and Internet Information Services (IIS).


### AWS Fargate


[AWS Fargate](https://aws.amazon.com/fargate/
) is a compute engine for [Amazon ECS](https://aws.amazon.com/ecs) that allows you to run containers without having to manage servers or clusters. 


### AWS Lambda

[AWS Lambda](https://aws.amazon.com/lambda/
) lets you run code without provisioning or managing servers. 


### AWS Outposts

[AWS Outposts](https://aws.amazon.com/outposts/
) bring native AWS services, infrastructure, and operating models to virtually any data center, co-location space, or on-premises facility. 




#### Comparison to GCP Anthos

https://www.qwinix.io/blog/aws-outposts-vs-google-cloud-anthos-forging-the-hybrid-cloud-future/


### AWS Wavelength

[AWS Wavelength](http://aws.amazon.com/wavelength
) is an AWS Infrastructure offering optimized for mobile edge computing applications. 

Wavelength Zones are AWS infrastructure deployments that embed AWS compute and storage services within communications service providers’ (CSP) datacenters at the edge of the 5G network, so application traffic from 5G devices can reach application servers running in Wavelength Zones without leaving the telecommunications network. This avoids the latency that would result from application traffic having to traverse multiple hops across the Internet to reach their destination, enabling customers to take full advantage of the latency and bandwidth benefits offered by modern 5G networks.





### VMware Cloud on AWS

[VMware Cloud](https://aws.amazon.com/vmware/
) on AWS is an integrated cloud offering jointly developed by AWS and VMware delivering a highly scalable, secure and innovative service that allows organizations to seamlessly migrate and extend their on-premises VMware vSphere-based environments to the AWS Cloud running on next-generation Amazon Elastic Compute Cloud (Amazon EC2) bare metal infrastructure. 




### Container Services

#### Amazon Elastic Container Service

[Amazon Elastic Container Service](https://aws.amazon.com/ecs/
) (Amazon ECS) is a highly scalable, high-performance container orchestration service that supports Docker containers and allows you to easily run and scale containerized applications on AWS. 




#### Amazon Elastic Kubernetes Service

[Amazon Elastic Kubernetes Service](https://aws.amazon.com/eks/
) (Amazon EKS) makes it easy to deploy, manage, and scale containerized applications using Kubernetes on AWS.




#### AWS App2Container

[AWS App2Container](http://aws.amazon.com/app2container
) (A2C) is a command-line tool for modernizing .NET and Java applications into containerized applications. 

A2C analyzes and builds an inventory of all applications running in virtual machines, on-premises or in the cloud. You simply select the application you want to containerize, and A2C packages the application artifact and identified dependencies into container images, configures the network ports, and generates the ECS task and Kubernetes pod definitions. A2C provisions, through CloudFormation, the cloud infrastructure and CI/CD pipelines required to deploy the containerized .NET or Java application into production. With A2C, you can easily modernize your existing applications and standardize the deployment and operations through containers.



#### Red Hat OpenShift Service on AWS

[Red Hat OpenShift Service on AWS](http://aws.amazon.com/rosa
) (ROSA) provides an integrated experience to use OpenShift. If you are already familiar with OpenShift, you can accelerate your application development process by leveraging familiar OpenShift APIs and tools for deployments on AWS.



## Application Integration

### Amazon Simple Queue Service

[Amazon Simple Queue Service](https://aws.amazon.com/sqs/
) (Amazon SQS) is a fully managed message queuing service that enables you to decouple and scale microservices, distributed systems, and serverless applications.



### Amazon MQ

[Amazon MQ](https://aws.amazon.com/amazon-mq/
) is a managed message broker service for Apache ActiveMQ and RabbitMQ that makes it easy to set up and operate message brokers in the cloud. 


### Amazon Simple Workflow Service

[Amazon Simple Workflow Service](https://aws.amazon.com/swf/
) (Amazon SWF) helps developers build, run, and scale background jobs that have parallel or sequential steps. 


### Amazon Simple Notification Service

[Amazon Simple Notification Service](https://aws.amazon.com/sns/
) (Amazon SNS) is a highly available, durable, secure, fully managed pub/sub messaging service that enables you to decouple microservices, distributed systems, and serverless applications.



### Amazon Managed Workflows for Apache Airflow (MWAA)

[Amazon Managed Workflows for Apache Airflow](http://aws.amazon.com/managed-workflows-for-apache-airflow
) (MWAA) is a managed orchestration service for Apache Airflow that makes it easier to set up and operate end-to-end data pipelines in the cloud at scale. 




### AWS Step Functions

[AWS Step Functions](https://aws.amazon.com/step-functions
) is a fully managed service that makes it easy to coordinate the components of distributed applications and microservices using visual workflows.


## Databases


### Amazon Aurora

[Amazon Aurora](https://aws.amazon.com/rds/aurora/
) is a MySQL and PostgreSQL compatible relational database engine that combines the speed and availability of high-end commercial databases with the simplicity and cost-eﬀectiveness of open source databases.



### Amazon SimpleDB

[Amazon SimpleDB](https://aws.amazon.com/simpledb/
) is a highly available NoSQL data store that offloads the work of database administration. Developers simply store and query data items via web services requests and Amazon SimpleDB does the rest.


There has been some talk of SimpleDB being superseded by DynamoDB (it is no longer being "iterated on", though Amazon does not plan to remove it). DynamoDB appears to be its successor.

### Amazon DynamoDB

[Amazon DynamoDB](https://aws.amazon.com/dynamodb/
) is a key-value and document database that delivers single-digit millisecond performance at any scale. It's a fully managed, multiregion, multimaster database with built-in security, backup and restore, and in-memory caching for internet-scale applications. DynamoDB can handle more than 10 trillion requests per day and support peaks of more than 20 million requests per second.



### Amazon ElastiCache

[Amazon ElastiCache](https://aws.amazon.com/elasticache/
) is a web service that makes it easy to deploy, operate, and scale an in-memory cache in the cloud. The service improves the performance of web applications by allowing you to retrieve information from fast, managed, in-memory caches, instead of relying entirely on slower disk-based databases. It supports Redis and Memcached.



### Amazon Keyspaces (for Apache Cassandra)

[Amazon Keyspaces](http://aws.amazon.com/keyspaces
) (for Apache Cassandra) is a scalable, highly available, and managed Apache Cassandra–compatible database service. 



### Amazon Neptune 

[Amazon Neptune](https://aws.amazon.com/neptune/
) is a fast, reliable, fully-managed graph database service that makes it easy to build and run applications that work with highly connected datasets. The core of Amazon Neptune is a purpose-built, high-performance graph database engine optimized for storing billions of relationships and querying the graph with milliseconds latency. 

Amazon Neptune supports popular graph models Property Graph and W3C's RDF, and their respective query languages Apache TinkerPop Gremlin and SPARQL, allowing you to easily build queries that efficiently navigate highly connected datasets. Neptune powers graph use cases such as recommendation engines, fraud detection, knowledge graphs, drug discovery, and network security.




### Amazon Relational Database Service

[Amazon Relational Database Service](https://aws.amazon.com/rds/
) (Amazon RDS) makes it easy to set up, operate, and scale a relational database in the cloud. It provides cost-efficient and resizable capacity while automating time-consuming administration tasks such as hardware provisioning, database setup, patching and backups. It frees you to focus on your applications so you can give them the fast performance, high availability, security and compatibility they need.

Amazon RDS is available on several database instance types - optimized for memory, performance or I/O - and provides you with six familiar database engines to choose from, including Amazon Aurora, PostgreSQL, MySQL, MariaDB, Oracle Database, and SQL Server. You can use the AWS Database Migration Service to easily migrate or replicate your existing databases to Amazon RDS.


#### AWS RDS or Aurora

https://aws.amazon.com/blogs/database/is-amazon-rds-for-postgresql-or-amazon-aurora-postgresql-a-better-choice-for-me/

### Amazon Quantum Ledger Database (QLDB)

[Amazon QLDB](https://aws.amazon.com/qldb/
) is a fully managed ledger database that provides a transparent, immutable, and cryptographically verifiable transaction log ‎owned by a central trusted authority. Amazon QLDB tracks each and every application data change and maintains a complete and verifiable history of changes over time.



### Amazon Timestream

[Amazon Timestream](https://aws.amazon.com/timestream/
) is a fast, scalable, fully managed time series database service for IoT and operational applications that makes it easy to store and analyze trillions of events per day at 1/10th the cost of relational databases. 




Amazon DocumentDB (with MongoDB compatibility)

[Amazon DocumentDB](https://aws.amazon.com/documentdb/
) (with MongoDB compatibility)  is a fast, scalable, highly available, and fully managed document database service that supports MongoDB workloads.



## Analytics

### Amazon EMR

[Amazon EMR](https://aws.amazon.com/emr
) is the industry-leading cloud big data platform for processing vast amounts of data using open source tools such as [Apache Spark](http://aws.amazon.com/emr/features/spark/), [Apache Hive](http://aws.amazon.com/emr/features/hive/), [Apache HBase](http://aws.amazon.com/emr/features/hbase/), [Apache Flink](http://aws.amazon.com/blogs/big-data/use-apache-flink-on-amazon-emr/), [Apache Hudi](http://aws.amazon.com/emr/features/hudi/), and [Presto](http://aws.amazon.com/emr/features/presto/).


#### EMR vs Dataproc

https://www.oreilly.com/content/spark-comparison-aws-vs-gcp/

### Amazon Kinesis

[Amazon Kinesis](https://aws.amazon.com/kinesis/
) makes it easy to collect, process, and analyze real-time, streaming data so you can get timely insights and react quickly to new information.


### Amazon Kinesis Data Firehose

[Amazon Kinesis Data Firehose](https://aws.amazon.com/kinesis/firehose/
) is the easiest way to reliably load streaming data into data stores and analytics tools. It can capture, transform, and load streaming data into Amazon S3, Amazon Redshift, Amazon Elasticsearch Service, and Splunk, enabling near real-time analytics with existing business intelligence tools and dashboards.


### Amazon Elasticsearch Service

[Amazon Elasticsearch](https://aws.amazon.com/elasticsearch-service/
) Service makes it easy to deploy, secure, operate, and scale Elasticsearch to search, analyze, and visualize data in real-time. 


### Amazon Redshift

[Amazon Redshift](https://aws.amazon.com/redshift/
) is the most widely used cloud data warehouse.


### Amazon QuickSight

[Amazon QuickSight](https://quicksight.aws/
) is a fast, cloud-powered business intelligence (BI) service that makes it easy for you to deliver insights to everyone in your organization. QuickSight lets you create and publish interactive dashboards that can be accessed from browsers or mobile devices. 


### AWS Lake Formation

[AWS Lake Formation](https://aws.amazon.com/lake-formation
) is a service that makes it easy to set up a secure data lake in days. A data lake is a centralized, curated, and secured repository that stores all your data, both in its original form and prepared for analysis. A data lake enables you to break down data silos and combine different types of analytics to gain insights and guide better business decisions.



### Amazon Athena

[Amazon Athena](https://aws.amazon.com/athena
) is an interactive query service that makes it easy to analyze data in Amazon S3 using standard SQL. Athena is serverless, so there is no infrastructure to manage, and you pay only for the queries that you run.




### AWS Data Pipeline

[AWS Data Pipeline](https://aws.amazon.com/datapipeline
) is a web service that helps you reliably process and move data between different AWS compute and storage services, as well as on-premises data sources, at specified intervals. 





## Networking and Content Delivery

### Amazon CloudFront

[Amazon CloudFront](https://aws.amazon.com/cloudfront/
) is a fast content delivery network (CDN) service that securely delivers data, videos, applications, and APIs to customers globally with low latency, high transfer speeds, all within a developer-friendly environment. CloudFront is integrated with AWS – both physical locations that are directly connected to the AWS global infrastructure, as well as other AWS services. CloudFront works seamlessly with services including AWS Shield for DDoS mitigation, Amazon S3, Elastic Load Balancing or Amazon EC2 as origins for your applications, and Lambda@Edge to run custom code closer to customers’ users and to customize the user experience.


### Amazon VPC

[Amazon Virtual Private Cloud](https://aws.amazon.com/vpc/
) (Amazon VPC) lets you provision a logically isolated section of the AWS Cloud where you can launch AWS resources in a virtual network that you define. You have complete control over your virtual networking environment, including selection of your own IP address range, creation of subnets, and configuration of route tables and network gateways. You can use both IPv4 and IPv6 in your VPC for secure and easy access to resources and applications.





### AWS VPN

[AWS Virtual Private Network](http://aws.amazon.com/vpn
) solutions establish secure connections between your on-premises networks, remote offices, client devices, and the AWS global network. AWS VPN is comprised of two services: AWS Site-to-Site VPN and AWS Client VPN. Each service provides a highly-available, managed, and elastic cloud VPN solution to protect your network traffic.


### AWS Direct Connect

[AWS Direct Connect](https://aws.amazon.com/directconnect/
) makes it easy to establish a dedicated network connection from your premises to AWS. Using AWS Direct Connect, you can establish private connectivity between AWS and your data center, office, or co-location environment, which in many cases can reduce your network costs, increase bandwidth throughput, and provide a more consistent network experience than Internet-based connections.

AWS Direct Connect lets you establish a dedicated network connection between your network and one of the AWS Direct Connect locations. Using industry standard 802.1Q virtual LANS (VLANs), this dedicated connection can be partitioned into multiple virtual interfaces. This allows you to use the same connection to access public resources, such as objects stored in Amazon S3 using public IP address space, and private resources such as EC2 instances running within a VPC using private IP address space, while maintaining network separation between the public and private environments. Virtual interfaces can be reconfigured at any time to meet your changing needs.


### Elastic Load Balancing

[Elastic Load Balancing](https://aws.amazon.com/elasticloadbalancing/
) (ELB) automatically distributes incoming application traffic across multiple targets, such as Amazon EC2 instances, containers, and IP addresses. It can handle the varying load of your application traffic in a single Availability Zone or across multiple Availability Zones. Elastic Load Balancing offers four types of load balancers that all feature the high availability, automatic scaling, and robust security necessary to make your applications fault tolerant.




### Amazon Route 53

[Amazon Route 53](https://aws.amazon.com/route53/
)  is a highly available and scalable cloud Domain Name System (DNS) web service. It is designed to give developers and businesses an extremely reliable and cost-effective way to route end users to Internet applications by translating human readable names, such as www.example.com, into the numeric IP addresses, such as 192.0.2.1, that computers use to connect to each other. Amazon Route 53 is fully compliant with IPv6 as well.


### AWS Global Accelerator

[AWS Global Accelerator](https://aws.amazon.com/global-accelerator/
) is a networking service that improves the availability and performance of the applications that you offer to your global users.

Today, if you deliver applications to your global users over the public internet, your users might face inconsistent availability and performance as they traverse through multiple public networks to reach your application. These public networks are often congested and each hop can introduce availability and performance risk. AWS Global Accelerator uses the highly available and congestion-free AWS global network to direct internet traffic from your users to your applications on AWS, making your users’ experience more consistent.


### AWS PrivateLink

[AWS PrivateLink](https://aws.amazon.com/privatelink/
) simplifies the security of data shared with cloud-based applications by eliminating the exposure of data to the public Internet. AWS PrivateLink provides private connectivity between VPCs, AWS services, and on-premises applications, securely on the Amazon network. AWS PrivateLink makes it easy to connect services across different accounts and VPCs to significantly simplify the network architecture.



### AWS Transit Gateway

[AWS Transit Gateway](https://aws.amazon.com/transit-gateway/
) is a service that enables customers to connect their Amazon Virtual Private Clouds (VPCs) and their on-premises networks to a single gateway. As you grow the number of workloads running on AWS, you need to be able to scale your networks across multiple accounts and Amazon VPCs to keep up with the growth. Today, you can connect pairs of Amazon VPCs using peering. However, managing point-to-point connectivity across many Amazon VPCs, without the ability to centrally manage the connectivity policies, can be operationally costly and cumbersome. For on-premises connectivity, you need to attach your AWS VPN to each individual Amazon VPC. This solution can be time consuming to build and hard to manage when the number of VPCs grows into the hundreds.

With AWS Transit Gateway, you only have to create and manage a single connection from the central gateway in to each Amazon VPC, on-premises data center, or remote office across your network. Transit Gateway acts as a hub that controls how traffic is routed among all the connected networks which act like spokes. This hub and spoke model significantly simplifies management and reduces operational costs because each network only has to connect to the Transit Gateway and not to every other network. Any new VPC is simply connected to the Transit Gateway and is then automatically available to every other network that is connected to the Transit Gateway. This ease of connectivity makes it easy to scale your network as you grow.




### AWS App Mesh

[AWS App Mesh](https://aws.amazon.com/app-mesh/
) makes it easy to monitor and control microservices running on AWS. App Mesh standardizes how your microservices communicate, giving you end-to-end visibility and helping to ensure high-availability for your applications.


### AWS Cloud Map

[AWS Cloud Map](https://aws.amazon.com/cloud-map/
) is a cloud resource discovery service. With Cloud Map, you can define custom names for your application resources, and it maintains the updated location of these dynamically changing resources. This increases your application availability because your web service always discovers the most up-to-date locations of its resources.




### Amazon API Gateway

[Amazon API Gateway](https://aws.amazon.com/api-gateway/) is a fully managed service that makes it easy for developers to create, publish, maintain, monitor, and secure APIs at any scale. With a few clicks in the AWS Management Console, you can create an API that acts as a “front door” for applications to access data, business logic, or functionality from your back-end services, such as workloads running on Amazon EC2, code running on AWS Lambda, or any web application. Amazon API Gateway handles all the tasks involved in accepting and processing up to hundreds of thousands of concurrent API calls, including traffic management, authorization and access control, monitoring, and API version management.

 

## Storage

### Amazon Simple Storage Service
 
[Amazon Simple Storage Service](https://aws.amazon.com/s3/
) (Amazon S3) is an object storage service that offers industry-leading scalability, data availability, security, and performance. This means customers of all sizes and industries can use it to store and protect any amount of data for a range of use cases, such as websites, mobile applications, backup and restore, archive, enterprise applications, IoT devices, and big data analytics. Amazon [S3](S3) provides easy-to-use management features so you can organize your data and configure finely-tuned access controls to meet your specific business, organizational, and compliance requirements. Amazon [S3](S3) is designed for 99.999999999% (11 9's) of durability, and stores data for millions of applications for companies all around the world.



### Amazon S3 Glacier

[Amazon S3 Glacier](https://aws.amazon.com/glacier/
) is a secure, durable, and extremely low-cost storage service for data archiving and long-term backup. It is designed to deliver 99.999999999% durability, and provides comprehensive security and compliance capabilities that can help meet even the most stringent regulatory requirements. Amazon S3 Glacier provides query-in-place functionality, allowing you to run powerful analytics directly on your archive data at rest. You can store data for as little as $1 per terabyte per month, a significant savings compared to on-premises solutions. To keep costs low yet suitable for varying retrieval needs, Amazon S3 Glacier provides three options for access to archives, from a few minutes to several hours, and S3 Glacier Deep Archive provides two access options ranging from 12 to 48 hours.


### Amazon Elastic Block Store

[Amazon Elastic Block Store](https://aws.amazon.com/ebs/
) (Amazon EBS) provides persistent block storage volumes for use with Amazon EC2 instances in the AWS Cloud. Each Amazon EBS volume is automatically replicated within its Availability Zone to protect you from component failure, offering high availability and durability. Amazon EBS volumes offer the consistent and low-latency performance needed to run your workloads. With Amazon EBS, you can scale your usage up or down within minutes—all while paying a low price for only what you provision.


### Amazon Elastic File System

[Amazon Elastic File System](https://aws.amazon.com/efs/
) (Amazon EFS) provides a simple, scalable, elastic file system for Linux-based workloads for use with AWS Cloud services and on-premises resources. It is built to scale on demand to petabytes without disrupting applications, growing and shrinking automatically as you add and remove files, so your applications have the storage they need – when they need it. It is designed to provide massively parallel shared access to thousands of Amazon EC2 instances, enabling your applications to achieve high levels of aggregate throughput and IOPS with consistent low latencies. Amazon EFS is a fully managed service that requires no changes to your existing applications and tools, providing access through a standard file system interface for seamless integration. Amazon EFS is a regional service storing data within and across multiple Availability Zones (AZs) for high availability and durability. You can access your file systems across AZs and AWS Regions and share files between thousands of Amazon EC2 instances and on-premises servers via AWS Direct Connect or AWS VPN.

You can mount an Amazon EFS file system in your virtual private cloud (VPC), through the Network File System versions 4.0 and 4.1 (NFSv4) protocol. 


### Amazon FSx for Lustre

[Amazon FSx](https://aws.amazon.com/fsx/lustre
) for Lustre is a fully managed file system that is optimized for compute-intensive workloads, such as high performance computing, machine learning, and media data processing workflows. Many of these applications require the high-performance and low latencies of scale-out, parallel file systems. Operating these file systems typically requires specialized expertise and administrative overhead, requiring you to provision storage servers and tune complex performance parameters. With Amazon FSx, you can launch and run a Lustre file system that can process massive data sets at up to hundreds of gigabytes per second of throughput, millions of IOPS, and sub-millisecond latencies.


### Amazon FSx for Windows File Server

[Amazon FSx for Windows File Server](https://aws.amazon.com/fsx/windows
) provides a fully managed native Microsoft Windows file system so you can easily move your Windows-based applications that require file storage to AWS. Built on Windows Server, Amazon FSx provides shared file storage with the compatibility and features that your Windows-based applications rely on, including full support for the SMB protocol and Windows NTFS, Active Directory (AD) integration, and Distributed File System (DFS). Amazon FSx uses SSD storage to provide the fast performance your Windows applications and users expect, with high levels of throughput and IOPS, and consistent sub-millisecond latencies. This compatibility and performance is particularly important when moving workloads that require Windows shared file storage, like CRM, ERP, and .NET applications, as well as home directories.



### AWS Backup

[AWS Backup](http://aws.amazon.com/backup
) enables you to centralize and automate data protection across AWS services. AWS Backup offers a cost-effective, fully managed, policy-based service that further simplifies data protection at scale. AWS Backup also helps you support your regulatory compliance or business policies for data protection. Together with AWS Organizations, AWS Backup enables you to centrally deploy data protection policies to configure, manage, and govern your backup activity across your organization’s AWS accounts and resources, including Amazon Elastic Compute Cloud (Amazon EC2) instances, Amazon Elastic Block Store (Amazon EBS) volumes, Amazon Relational Database Service (Amazon RDS) databases (including Amazon Aurora clusters), Amazon DynamoDB tables, Amazon Elastic File System (Amazon EFS) file systems, Amazon FSx for Lustre file systems, Amazon FSx for Windows File Server file systems, and AWS Storage Gateway volumes.


### AWS Storage Gateway

The [AWS Storage Gateway](https://aws.amazon.com/storagegateway/
) is a hybrid storage service that enables your on-premises applications to seamlessly use AWS cloud storage. You can use the service for backup and archiving, disaster recovery, cloud data processing, storage tiering, and migration. Your applications connect to the service through a virtual machine or hardware gateway appliance using standard storage protocols, such as NFS, SMB and iSCSI. The gateway connects to AWS storage services, such as Amazon S3, S3 Glacier, and Amazon EBS, providing storage for files, volumes, and virtual tapes in AWS. The service includes a highly-optimized data transfer mechanism, with bandwidth management, automated network resilience, and efficient data transfer, along with a local cache for low-latency on-premises access to your most active data.







## Machine Learning



### Amazon SageMaker

[Amazon SageMaker](https://aws.amazon.com/sagemaker
) is a fully-managed service that enables developers and data scientists to quickly and easily build, train, and deploy machine learning models at any scale. SageMaker removes all the barriers that typically slow down developers who want to use machine learning.




### Amazon SageMaker Ground Truth

[Amazon SageMaker Ground Truth](https://aws.amazon.com/sagemaker/groundtruth
) helps you build highly accurate training datasets for machine learning quickly. SageMaker Ground Truth offers easy access to public and private human labelers and provides them with built-in workflows and interfaces for common labeling tasks. Additionally, SageMaker Ground Truth can lower your labeling costs by up to 70% using automatic labeling, which works by training Ground Truth from data labeled by humans so that the service learns to label data independently.



### TensorFlow on AWS

[TensorFlow](https://aws.amazon.com/tensorflow
) enables developers to quickly and easily get started with deep learning in the cloud. The framework has broad support in the industry and has become a popular choice for deep learning research and application development, particularly in areas such as computer vision, natural language understanding and speech translation.


### Apache MXNet on AWS

[Apache MXNet](https://aws.amazon.com/mxnet
) on AWS is a fast and scalable training and inference framework with an easy-to-use, concise API for machine learning.


### Amazon Elastic Inference

[Amazon Elastic Inference](https://aws.amazon.com/machine-learning/elastic-inference/
)allows you to attach low-cost GPU-powered acceleration to Amazon EC2 and Amazon SageMaker instances to reduce the cost of running deep learning inference by up to 75%. Amazon Elastic Inference supports TensorFlow, Apache MXNet, PyTorch, and ONNX models.


### AWS Inferentia

[AWS Inferentia](https://aws.amazon.com/machine-learning/inferentia
) is a machine learning inference chip designed to deliver high performance at low cost. AWS Inferentia will support the TensorFlow, Apache MXNet, and PyTorch deep learning frameworks, as well as models that use the ONNX format.


### Amazon Forecast

[Amazon Forecast](https://aws.amazon.com/forecast/
) is a fully managed service that uses machine learning to deliver highly accurate forecasts.


### Amazon Fraud Detector

[Amazon Fraud Detector](http://aws.amazon.com/fraud-detector
) is a fully managed service that uses machine learning (ML) and more than 20 years of fraud detection expertise from Amazon, to identify potentially fraudulent activity so customers can catch more online fraud faster.


### Amazon Personalize

[Amazon Personalize](https://aws.amazon.com/personalize/
) is a machine learning service that makes it easy for developers to create individualized recommendations for customers using their applications.


### Amazon Rekognition

[Amazon Rekognition](https://aws.amazon.com/rekognition
) makes it easy to add image and video analysis to your applications using proven, highly scalable, deep learning technology that requires no machine learning expertise to use. 


### Amazon Comprehend


[Amazon Comprehend](https://aws.amazon.com/comprehend
) is a natural language processing (NLP) service that uses machine learning to find insights and relationships in text. 


### Amazon Lex

[Amazon Lex](https://aws.amazon.com/lex
) is a service for building conversational interfaces into any application using voice and text. Lex provides the advanced deep learning functionalities of automatic speech recognition (ASR) for converting speech to text, and natural language understanding (NLU) to recognize the intent of the text, to enable you to build applications with highly engaging user experiences and lifelike conversational interactions. With Amazon Lex, the same deep learning technologies that power Amazon Alexa are now available to any developer to build sophisticated, natural language, conversational bots (“chatbots”).


### Amazon Polly

[Amazon Polly](https://aws.amazon.com/polly
) is a service that turns text into lifelike speech. Polly lets you create applications that talk, enabling you to build entirely new categories of speech-enabled products. Polly is an Amazon artificial intelligence (AI) service that uses advanced deep learning technologies to synthesize speech that sounds like a human voice. 


### Amazon Textract

[Amazon Textract](https://aws.amazon.com/textract/
) is a service that automatically extracts text and data from scanned documents. Amazon Textract goes beyond simple optical character recognition (OCR) to also identify the contents of fields in forms and information stored in tables.


### Amazon Transcribe

[Amazon Transcribe](https://aws.amazon.com/transcribe
) is an automatic speech recognition (ASR) service that makes it easy for developers to add speech-to-text capability to their applications. Using the Amazon Transcribe API, you can analyze audio files stored in Amazon S3 and have the service return a text file of the transcribed speech. You can also send a live audio stream to Amazon Transcribe and receive a stream of transcripts in real time.



### Amazon Translate

[Amazon Translate](https://aws.amazon.com/translate
) is a neural machine translation service that delivers fast, high-quality, and affordable language translation. 




## Internet of Things


### AWS IoT Greengrass

[AWS IoT Greengrass](https://aws.amazon.com/greengrass/
) seamlessly extends AWS to devices so they can act locally on the data they generate, while still using the cloud for management, analytics, and durable storage. 


### AWS IoT Core

[AWS IoT Core](https://aws.amazon.com/iot-core
) is a managed cloud service that lets connected devices easily and securely interact with cloud applications and other devices. AWS IoT Core can support billions of devices and trillions of messages, and can process and route those messages to AWS endpoints and to other devices reliably and securely. 



### AWS IoT Analytics

[AWS IoT Analytics](https://aws.amazon.com/iot-analytics/
) is a fully-managed service that makes it easy to run and operationalize sophisticated analytics on massive volumes of IoT data without having to worry about the cost and complexity typically required to build an IoT analytics platform. 


### FreeRTOS

[FreeRTOS](https://aws.amazon.com/freertos
) is an operating system for microcontrollers that makes small, low-power edge devices easy to program, deploy, secure, connect, and manage. 



## Migration


### AWS Transfer Family

[AWS Transfer Family](http://aws.amazon.com/aws-transfer-family
) provides fully managed support for file transfers directly into and out of Amazon S3 or Amazon EFS. With support for Secure File Transfer Protocol (SFTP), File Transfer Protocol over SSL (FTPS), and File Transfer Protocol (FTP), the AWS Transfer Family helps you seamlessly migrate your file transfer workflows to AWS by integrating with existing authentication systems, and providing DNS routing with Amazon Route 53 so nothing changes for your customers and partners, or their applications. 


### AWS Snow Family

The [AWS Snow](http://aws.amazon.com/snow
) Family helps customers that need to run operations in austere, non-data center environments, and in locations where there's lack of consistent network connectivity.



http://aws.amazon.com/snowcone

https://aws.amazon.com/snowball

https://aws.amazon.com/snowmobile

### AWS DataSync

[AWS DataSync](https://aws.amazon.com/datasync
) is a data transfer service that makes it easy for you to automate moving data between on-premises storage and Amazon S3 or Amazon Elastic File System (Amazon EFS). 


### AWS Application Migration Service

[AWS Application Migration Service](http://aws.amazon.com/application-migration-service
) (AWS MGN) allows you to quickly realize the benefits of migrating applications to the cloud without changes and with minimal downtime.




### AWS Database Migration Service

[AWS Database Migration Service](https://aws.amazon.com/dms
) helps you migrate databases to AWS easily and securely. The source database remains fully operational during the migration, minimizing downtime to applications that rely on the database. 

