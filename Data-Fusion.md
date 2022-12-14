[Data Fusion]( https://cloud.google.com/data-fusion  ) is a fully managed, cloud-native, scalable data integration platform. It is a
GUI based data integration service for building and managing data pipelines.


https://medium.com/google-cloud/designing-a-data-lake-on-gcp-with-data-fusion-and-composer-e2ea0a753525

Data Fusion is built using open source project [CDAP](https://github.com/cdapio/cdap), and this open core ensures data pipeline portability for users. CDAP’s broad integration with on-premises and public cloud platforms gives Cloud Data Fusion users the ability to break down silos and deliver insights that were previously inaccessible.


https://cloud.google.com/data-fusion


CDAP is an integrated, open source application development platform for the Hadoop ecosystem that provides developers with data and application abstractions to simplify and accelerate application development, address a broader range of real-time and batch use cases, and deploy applications into production while satisfying enterprise requirements.

https://github.com/cdapio/cdap

Under the hood, Data Fusion executes pipelines on a Dataproc cluster. Data Fusion automatically converts GUI based pipelines into Dataproc jobs for execution whenever a pipeline is executed. It supports two execution engine options: MapReduce and Apache Spark.


### CDAP Example Apps

https://github.com/cdapio/cdap-apps

## Modern, more secure data lakes on Google Cloud

Cloud Data Fusion helps users build scalable, distributed data lakes on Google Cloud by integrating data from siloed on-premises platforms. Customers can leverage the scale of the cloud to centralize data and drive more value out of their data as a result. 

https://towardsdatascience.com/building-a-data-lake-on-gcp-with-cdap-6271c264f22e

The self-service capabilities of Cloud Data Fusion increase process visibility and lower the overall cost of operational support.

https://cloud.google.com/data-fusion/plugins


## Choosing Dataflow, Dataprep, Dataproc or Data Fusion

<!--
[[https://storage.googleapis.com/gweb-cloudblog-publish/images/9.19.41_AM.max-800x800.png]]
-->

https://wisdomplexus.com/blogs/dataproc-vs-dataflow-vs-dataprep/


## Wrangler UI

https://datadice.medium.com/the-wrangler-user-interface-of-cloud-data-fusion-21e96cfe1b2d

## Agile data warehouses with BigQuery

Cloud Data Fusion can help organizations better understand their customers by breaking down data silos and enabling development of agile, cloud-based data warehouse solutions in [BigQuery](BigQuery). A trusted, unified view of customer engagement and behavior unlocks the ability to drive a better customer experience, which leads to higher retention and higher revenue per customer.

https://cloud.google.com/data-fusion/docs/tutorials/replicating-data/mysql-to-bigquery

## Unified analytics environment

Many users today want to establish a unified analytics environment across a myriad of expensive, on-premises data marts. Employing a wide range of disconnected tools and stop-gap measures creates data quality and security challenges. Cloud Data Fusion’s vast variety of connectors, visual interfaces, and abstractions centered around business logic helps in lowering TCO, promoting self-service and standardization, and reducing repetitive work.


## Data Fusion Features

https://cloud.google.com/data-fusion#section-10

### UDD

https://medium.com/cdapio/a-definitive-guide-to-wrangler-user-defined-directive-udd-b1dc2d795ce6

### Upload UDDs through REST API

https://jtaras.medium.com/cloud-data-fusion-upload-udds-through-the-rest-api-32d015de1e22

### Data Fusion  Secure Store

https://jtaras.medium.com/cloud-data-fusion-adding-a-service-account-to-the-secure-store-8fb987af917a

## CCAI

https://cloud.google.com/blog/products/data-analytics/contact-center-ai-insights-made-easy-with-cloud-data-fusion


## Ephemeral Data Fusion using Terraform

https://jtaras.medium.com/cloud-data-fusion-using-terraform-to-run-ephemeral-data-fusion-instances-8fef704d2011

## Examples

### Import CSV data into BigQuery using Data Fusion

https://codelabs.developers.google.com/codelabs/batch-csv-cdf-bq


### End-to-end automated Analytics 

https://medium.com/google-cloud/from-zero-to-hero-end-to-end-automated-analytics-workload-using-cloud-functions-data-fusion-28670e5e7c74

### Cloud Storage upload trigger Data Fusion ETL Pipelines

https://jtaras.medium.com/google-data-fusion-using-cloud-storage-file-uploads-to-trigger-data-fusion-etl-pipelines-cec3325c78e7

### Config driven Pipeline

https://jtaras.medium.com/cloud-data-fusion-building-config-driven-pipelines-a40d23e9d011

### Creating reusable pipeline

https://cloud.google.com/data-fusion/docs/tutorials/reusable-pipeline

### Connect SAP data via Cloud Data Fusion

https://cloud.google.com/blog/products/data-analytics/cloud-data-fusion-helps-consolidate-sap-and-non-sap-datasets

### Google Cloud Cortex Framework

https://cloud.google.com/solutions/cortex


https://cloud.google.com/blog/products/sap-google-cloud/faster-time-to-value-with-the-google-cloud-cortex-framework

### SAP SLT Replication plugin

https://cloud.google.com/data-fusion/docs/how-to/use-sap-slt-plugin

### Reverse ETL


https://jtaras.medium.com/cloud-data-fusion-reverse-etl-from-bigquery-to-cloudsql-e8aa1e804ba5

## Tutorials


https://cloud.google.com/data-fusion/docs/tutorials

### Using Cloud Vision API from Data Fusion

https://cloud.google.com/blog/products/data-analytics/connecting-data-fusion-to-the-vision-api-via-oauth-restful-apis

### Customize compute profiles at Runtime

https://jtaras.medium.com/cloud-data-fusion-customizing-compute-profiles-at-runtime-6420f9b185ba

### Update deployed pipelines through REST API

https://jtaras.medium.com/cloud-data-fusion-update-deployed-pipelines-through-rest-api-2be0ad25e25f