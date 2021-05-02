
## Google Cloud Platform


### Introduction

Google Cloud Platform offers four main kinds of services: Compute, Storage, Big Data, and Machine Learning. 

[https://cloud.google.com/docs/overview/](https://cloud.google.com/docs/overview/)

https://www.youtube.com/watch?v=vmOMataJZWw

GCP also includes Google App Engine, Google Compute Engine, Google Kubernetes Engine, Google Cloud Storage, Google Cloud SQL, and BigQuery. You will learn about important resource and policy management tools, such as the Google Cloud Resource Manager hierarchy and Google Cloud Identity and Access Management.

[https://cloud.google.com/products](https://cloud.google.com/products)

Here are some very high level diagrams and references for various GCP services.

[https://gcp.solutions/](https://gcp.solutions/)

This video is an Introduction to GCP.

[https://www.youtube.com/watch?v=4D3X6Xl5c_Y](https://www.youtube.com/watch?v=4D3X6Xl5c_Y)


#### Regions and Zones

<img src="https://storage.googleapis.com/gweb-cloudblog-publish/images/gcp_global_presence.max-1600x1600.jpg" width="800">

Google Cloud consists of a set of physical assets, such as computers and hard disk drives, and virtual resources, such as virtual machines (VMs), that are contained in [Google's data centers](https://cloud.withgoogle.com/infrastructure/explore) around the globe. 

https://cloud.google.com/about/locations

Each data center location is in a region. Regions are available in Asia, Australia, Europe, North America, and South America. Each region is a collection of zones, which are isolated from each other within the region. Each zone is identified by a name that combines a letter identifier with the name of the region. For example, zone a in the East Asia region is named asia-east1-a. This distribution of resources provides several benefits, including redundancy in case of failure and reduced latency by locating resources closer to clients. 

https://www.youtube.com/watch?v=XZmGGAbHqa0

https://cloud.google.com/architecture/scalable-and-resilient-apps

This distribution also introduces some rules about how resources can be used together. When architecting your apps in GCP, it’s important to understand [regions and zones](https://cloud.google.com/compute/docs/regions-zones/global-regional-zonal-resources), as well as the resources that are regional or zonal. While some of the core resources in GCP are global, others may be restricted by region or zone. 

<img src="https://cloud.google.com/docs/images/overview/regions-zones.svg" width="700">


Regional resources can be used anywhere within the same region, while zonal resources can be used anywhere within the same zone. 

[https://cloud.google.com/compute/docs/regions-zones/global-regional-zonal-resources](https://cloud.google.com/compute/docs/regions-zones/global-regional-zonal-resources)


#### GCP Youtube Channel

Google produced videos that help you learn about GCP are collected in this channel.

https://www.youtube.com/googlecloudplatform/


#### GCP Useful Links


Review this [Curated list of URLs](GCP-Learning-Links) related to GCP.

[https://github.com/GoogleCloudPlatform/awesome-google-cloud](https://github.com/GoogleCloudPlatform/awesome-google-cloud)

A list of industry specific solutions.

[https://cloud.google.com/solutions](https://cloud.google.com/solutions)

A list GCP Architecture references.

[https://gcp.solutions/](https://gcp.solutions/)

A list of samples.

[https://cloud.google.com/docs/samples](https://cloud.google.com/docs/samples)

#### Summary of GCP Services

[https://github.com/gregsramblings/google-cloud-4-words](https://github.com/gregsramblings/google-cloud-4-words)

<img src="https://static.packt-cdn.com/products/9781838647438/graphics/2622d854-c8a6-4189-99a7-c55e31bc5fae.png" width="400">


### Compare Platforms

Here are some comparisons to [AWS](https://aws.amazon.com/), [Azure](https://azure.microsoft.com/), [Openstack](https://www.openstack.org/) and On-prem.

[https://cloud.google.com/docs/compare](https://cloud.google.com/docs/compare)


### Google Cloud setup checklist

This checklist helps you set up Google Cloud for scalable, production-ready enterprise workloads. The checklist is designed for administrators who are trusted with complete control over the company's Google Cloud resources.

[https://cloud.google.com/docs/enterprise/onboarding-checklist](https://cloud.google.com/docs/enterprise/onboarding-checklist)


### Basic Tools


#### Cloud SDK

Google Cloud SDK is a set of tools that you can use to manage resources and applications hosted on Google Cloud. These include the [gcloud](https://cloud.google.com/sdk/gcloud/reference), [gsutil](https://cloud.google.com/storage/docs/gsutil), and [bq](https://cloud.google.com/bigquery/bq-command-line-tool) command line tools. The gcloud command-line tool is downloaded along with the Cloud SDK; a comprehensive guide to the gcloud CLI can be found in [gcloud command-line tool overview](https://cloud.google.com/sdk/gcloud).

[https://cloud.google.com/sdk/docs](https://cloud.google.com/sdk/docs)

Learn more about the integrated command line tools to help manage resources and apps on Google Cloud. Try the Google Cloud SDK: Qwik Start lab here:[ http://bit.ly/2vm0rKN](https://www.youtube.com/redirect?q=http%3A%2F%2Fbit.ly%2F2vm0rKN&event=video_description&v=69MdTXgA6Ws&redir_token=QUFFLUhqbnUzMVJzQ3NQZExmdExPV2d4eC1JV2lMcjJpd3xBQ3Jtc0trNHZBRWt0Wmtmelp3OVlCVTJyNFNBSGd3WEp2SWI5aE0zcWZ6bE4xaU8wcDZSVG9WeEVoUmVJY24wdi13VTBzVml4aWFGNUlaZTBIZWpqY2ZBbmlXdHpYNUI1bzRpa2stZVh4MFRkMHdzcW5yOGs0WQ%3D%3D)

[https://www.youtube.com/watch?v=69MdTXgA6Ws](https://www.youtube.com/watch?v=69MdTXgA6Ws)


#### Cloud Shell

Google Cloud Shell is an interactive shell environment for Google Cloud Platform that makes it easy for you to learn and experiment with GCP and manage your projects and resources from your web browser.

[https://cloud.google.com/shell/docs](https://cloud.google.com/shell/docs)

[https://www.youtube.com/watch?v=d7bXH_2X760](https://www.youtube.com/watch?v=d7bXH_2X760)


### Tutorials

A list of updated tutorials on GCP.

[https://cloud.google.com/docs/tutorials](https://cloud.google.com/docs/tutorials)

A list of short tutorials on getting started with GCP.

[https://cloud.google.com/gcp/getting-started](https://cloud.google.com/gcp/getting-started)

###  Essentials videos

https://www.youtube.com/playlist?list=PLIivdWyY5sqKh1gDR0WpP9iIOY00IE0xL

### Whitepapers

Google Cloud whitepapers explain the technology underlying our products and services or examine topics such as security, architecture, and total cost of ownership. The whitepapers listed here are written by Googlers, independent analysts, customers, and partners.

[https://cloud.google.com/whitepapers/](https://cloud.google.com/whitepapers/)



### Qwiklabs


#### GCP Essentials

GCP Essentials Qwiklab Quest. A Quest is a bunch of Qwiklabs collected under a topic.

[Google Cloud Essentials](https://www.qwiklabs.com/quests/23?catalog_rank=%7B%22rank%22%3A6%2C%22num_filters%22%3A1%2C%22has_search%22%3Atrue%7D&search_id=7467715)


#### Cloud Architecture

This fundamental-level quest is unique amongst the other Qwiklabs offerings. The labs have been curated to give IT professionals hands-on practice with topics and services that appear in the [Google Cloud Certified Professional Cloud Architect](https://cloud.google.com/certification/cloud-architect) Certification.

[Cloud Architecture](https://www.qwiklabs.com/quests/24?catalog_rank=%7B%22rank%22%3A10%2C%22num_filters%22%3A1%2C%22has_search%22%3Atrue%7D&search_id=7467715)


#### Cloud Engineering

This quest is unique amongst the other Qwiklabs offerings. The labs have been curated to give IT professionals hands-on practice with topics and services that appear in the Google Cloud Certified Associate Cloud Engineer Certification. 

[Cloud Engineering](https://www.qwiklabs.com/quests/66?catalog_rank=%7B%22rank%22%3A9%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&search_id=7468028)


#### Manage Cloud Environments

This fundamental-level quest is unique amongst the other Qwiklabs offerings. The labs have been curated to give IT professionals hands-on practice with topics and services that appear in the [Google Cloud Certified Professional Cloud Architect](https://cloud.google.com/certification/cloud-architect) Certification. 

[Deploy and Manage Cloud Environments with Google Cloud](https://www.qwiklabs.com/quests/121?catalog_rank=%7B%22rank%22%3A1%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&search_id=7467754)




