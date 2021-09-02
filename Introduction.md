[Google Cloud](  https://www.youtube.com/watch?v=4D3X6Xl5c_Y ) consists of a set of [physical assets]( https://www.google.com/about/datacenters/  ), such as computers and hard disk drives, and virtual resources, such as [virtual machines](VM) (VMs), that are contained in Google's [data centers](  https://blog.google/inside-google/infrastructure/how-data-center-security-works/ ) around [the globe](  https://cloud.withgoogle.com/infrastructure  ).

[Google Cloud Platform](https://cloud.google.com/) offers four main kinds of [products](https://cloud.google.com/products) and [services](  https://gcp.solutions/ ): [Compute](Compute), [Storage](Storage), [Big Data](Big-Data), and [Machine Learning](Machine-Learning). 


[GCP](https://www.youtube.com/watch?v=vmOMataJZWw) also [includes](  https://www.youtube.com/channel/UCJS9pqu9BzkAMNTmzNMNhvg/playlists  ) Google [App Engine](App-Engine), Google [Compute Engine](Compute), Google [Kubernetes Engine](GKE), Google [Cloud Storage](Storage), Google [Cloud SQL]( CloudSQL  ), and [BigQuery](BigQuery). You will learn about important resource and policy management tools, such as the Google [Cloud Resource Manager](  https://cloud.google.com/resource-manager ) hierarchy and Google Cloud [Identity and Access Management](  IAM). 

GCP has benefitted from [fundamental research ](https://research.google/) that continue to influence the  product development.

## Getting Started

https://console.cloud.google.com/getting-started


## Regions and Zones



Each [data center](https://www.youtube.com/watch?v=XZmGGAbHqa0) location is in a region. Regions are available in Asia, Australia, Europe, North America, and South America. Each region is a collection of zones, which are [isolated from each other](https://cloud.google.com/architecture/scalable-and-resilient-apps) within the region. Each zone is identified by a name that combines a letter identifier with the name of the region. For example, zone a in the East Asia region is named asia-east1-a. This distribution of resources provides several benefits, including redundancy in case of failure and reduced latency by locating resources closer to clients. 


This distribution also introduces some rules about how resources can be used together. When architecting your apps in GCP, it’s important to understand [regions and zones](https://cloud.google.com/compute/docs/regions-zones/global-regional-zonal-resources), as well as the resources that are regional or zonal. While some of the core resources in GCP are global, others may be restricted by [region or zone](https://cloud.google.com/compute/docs/regions-zones/global-regional-zonal-resources). 



Regional resources can be used anywhere within the same region, while zonal resources can be used anywhere within the same zone. 

## What makes GCP Different?

https://cloud.google.com/free/docs/what-makes-google-cloud-platform-different


## GCP Youtube Channel

[Google produced videos](https://www.youtube.com/googlecloudplatform/) that help you learn about GCP are collected in this channel.


## GCP Useful Links


Review this [awesome](https://github.com/GoogleCloudPlatform/awesome-google-cloud) list of [ resources](GCP-Learning-Links) related to GCP.

Review the lists of [industry specific solutions](https://cloud.google.com/solutions) and GCP [Architecture reference solutions](https://gcp.solutions/) and  [samples](https://cloud.google.com/docs/samples).


### Summary of GCP Services

Summary of google cloud services in [4 words](https://github.com/gregsramblings/google-cloud-4-words).




## Compare Platforms

[Here are some comparisons](https://cloud.google.com/docs/compare) to [AWS](AWS), [Azure](https://azure.microsoft.com/), [Openstack](https://www.openstack.org/) and On-prem.



## Google Cloud setup checklist

This [checklist](https://cloud.google.com/docs/enterprise/onboarding-checklist) helps you set up Google Cloud for scalable, production-ready enterprise workloads. The checklist is designed for administrators who are trusted with complete control over the company's Google Cloud resources.



## Basic Tools


### Cloud SDK

Google [Cloud SDK](https://cloud.google.com/sdk/docs) is a set of tools that you can use to manage resources and applications hosted on Google Cloud. These include the [gcloud](https://cloud.google.com/sdk/gcloud/reference), [gsutil](https://cloud.google.com/storage/docs/gsutil), and [bq](https://cloud.google.com/bigquery/bq-command-line-tool) command line tools. The [gcloud command-line tool](https://dominicusin.github.io/2019/07/25/gcloud-cheat-sheet.html) is downloaded along with the Cloud SDK; a comprehensive guide to the gcloud CLI can be found in [gcloud command-line tool overview](https://cloud.google.com/sdk/gcloud).


Learn more about the integrated [command line tools](https://www.youtube.com/watch?v=69MdTXgA6Ws) to help manage resources and apps on Google Cloud. Try the [Google Cloud SDK: Qwik Start lab](http://bit.ly/2vm0rKN).




### Cloud Shell

Google [Cloud Shell](https://cloud.google.com/shell/docs) is an [interactive shell](   https://www.youtube.com/watch?v=d7bXH_2X760 ) environment for Google Cloud Platform that makes it easy for you to learn and experiment with GCP and manage your projects and resources from your web browser.


## Tutorials

A list of short tutorials on [getting started](https://cloud.google.com/gcp/getting-started) with [GCP](  https://cloud.google.com/docs/tutorials ).


## Whitepapers

[Google Cloud whitepapers](https://cloud.google.com/whitepapers/) explain the technology underlying gcp products and services or examine topics such as security, architecture, and total cost of ownership. 

## Cloud Architecture Center

https://cloud.google.com/architecture/

## Compare AWS and Azure services to GCP

https://cloud.google.com/free/docs/aws-azure-gcp-service-comparison


### AWS

[AWS](AWS)

### Survey of other cloud providers


https://geekflare.com/cloud-hosting-platform/

## Videos

https://www.youtube.com/googlecloud

https://www.youtube.com/channel/UCJS9pqu9BzkAMNTmzNMNhvg

## Newsletter

https://www.gcpweekly.com/

## Podcasts

https://gcppodcast.com/

https://kubernetespodcast.com/

https://softwareengineeringdaily.com/category/all-episodes/exclusive-content/Podcast/

## Blogs

https://cloud.google.com/blog/products/gcp

https://cloud.google.com/blog/products/data-analytics

https://firebase.googleblog.com/

https://medium.com/google-cloud


## Qwiklabs


[Google Cloud Essentials](https://www.qwiklabs.com/quests/23?catalog_rank=%7B%22rank%22%3A6%2C%22num_filters%22%3A1%2C%22has_search%22%3Atrue%7D&search_id=7467715)

[Cloud Architecture](https://www.qwiklabs.com/quests/24?catalog_rank=%7B%22rank%22%3A10%2C%22num_filters%22%3A1%2C%22has_search%22%3Atrue%7D&search_id=7467715)

[Cloud Engineering](https://www.qwiklabs.com/quests/66?catalog_rank=%7B%22rank%22%3A9%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&search_id=7468028)





