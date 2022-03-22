## Kubernetes

[Kubernetes](Kubernetes)  is a portable, extensible, open-source platform for managing containerized workloads and services, that facilitates both declarative configuration and automation. 

https://cloud.google.com/blog/products/containers-kubernetes/the-rise-and-future-of-kubernetes-and-open-source-at-google


## Google Kubernetes Engine (GKE)

[GKE](https://cloud.google.com/kubernetes-engine) is Secured and fully managed [Kubernetes](Kubernetes) service with revolutionary [autopilot](https://cloud.google.com/kubernetes-engine/docs/concepts/autopilot-overview) mode of operation.

### Autopilot

https://cloud.google.com/kubernetes-engine/docs/concepts/autopilot-overview

https://cloud.google.com/blog/products/containers-kubernetes/introducing-gke-autopilot

https://cloud.google.com/kubernetes-engine/docs/concepts/autopilot-overview

https://cloud.google.com/blog/products/containers-kubernetes/partner-devops-and-security-solutions-for-gke-autopilot

https://medium.com/google-cloud/gke-autopilot-and-cloud-code-1da63bedd18e

### Backup for GKE


https://cloud.google.com/blog/products/storage-data-transfer/google-cloud-launches-backups-for-gke

### GKE Workload Metrics

[G​K​E workload metrics](https://cloud.google.com/stackdriver/docs/solutions/gke/managing-metrics#workload-metrics) provide way to monitor Kubernetes applications using Cloud Monitoring.

### VMs and GKE

https://medium.com/@kote.isaev/gotcha-of-cheaper-e2-medium-vms-at-google-cloud-d6aafcd8f347

### Quotas and Limits

https://cloud.google.com/kubernetes-engine/quotas

### GKE vs EKS vs AKS

https://www.stackrox.com/post/2021/01/eks-vs-gke-vs-aks-jan2021/

### Image streaming

https://cloud.google.com/blog/products/containers-kubernetes/introducing-container-image-streaming-in-gke

### Zero Trust

https://cloud.google.com/blog/products/identity-security/workload-credentials-for-gke-via-cas

### Using workload identity with GKE


Workload Identity allows workloads in your GKE clusters to impersonate Identity and Access Management (IAM) service accounts to access Google Cloud services. Workload Identity is enabled by default on Autopilot clusters.


https://cloud.google.com/kubernetes-engine/docs/how-to/workload-identity


https://debricked.com/blog/what-is-gke-workload-identity/

https://medium.com/zeotap-customer-intelligence-unleashed/gke-workload-identity-a-secure-way-for-gke-applications-to-access-gcp-services-f880f4e74e8c

### Terraform workload identity

https://registry.terraform.io/modules/terraform-google-modules/kubernetes-engine/google/latest/submodules/workload-identity

### Deploying Google Cloud Functions using GitHub Actions and Workload Identity authentication

https://blog.leandrotoledo.org/deploying-google-cloud-functions-using-github-actions-and-workload-identity-authentication/

### Port limit

https://gtseres.medium.com/how-to-expose-more-than-5-ports-for-a-loadbalancer-kservice-in-gcp-ee2a08c54e85


### GKE HA and Stateful Application, PVC

[Kubernetes](https://cloud.google.com/kubernetes-engine/docs/concepts/kubernetes-engine-overview) is a great tool to host your highly available applications but what happens when you have to work with [stateful workloads](https://www.youtube.com/watch?v=rRZtZX0PDFc)? 

### GKE Monitoring

https://www.containiq.com/post/gke-monitoring


### Batch on GKE

Batch on GKE (Batch) is a cloud-native solution for scheduling and managing batch workloads. With Batch, you can leverage the on-demand and flexible nature of cloud. Batch is based on Kubernetes and containers so your jobs are portable.

[https://cloud.google.com/kubernetes-engine/docs/concepts/batch](https://cloud.google.com/kubernetes-engine/docs/concepts/batch)

A video about using Batch on GKE.

[https://www.youtube.com/watch?v=qLSLs-ko3ik](https://www.youtube.com/watch?v=qLSLs-ko3ik)

## GKE Operations

A video about using Cloud Logging on [GKE](https://cloud.google.com/kubernetes-engine/docs/concepts/kubernetes-engine-overview).

[https://www.youtube.com/watch?v=IusP8jDfnt4](https://www.youtube.com/watch?v=IusP8jDfnt4)


### GKE Multi-cluster Services

https://cloud.google.com/kubernetes-engine/docs/concepts/multi-cluster-services

https://cloud.google.com/blog/products/containers-kubernetes/multi-cluster-kubernetes-with-gke-at-geotab

### Kubernetes applications on Google Cloud Marketplace

The Kubernetes apps in Cloud Marketplace include container images and configuration files, such as a kubectl configuration or a[ Helm chart](https://helm.sh/docs/topics/charts/). When you deploy an app from Cloud Marketplace, the Kubernetes resources are created in your cluster, and you can manage the resources as a group.

[https://cloud.google.com/marketplace/docs/kubernetes-apps](https://cloud.google.com/marketplace/docs/kubernetes-apps)



### Tutorials

#### How to create a GKE cluster

Creating a Google Kubernetes Engine (GKE) cluster using Terraform.

[https://www.youtube.com/watch?v=Vcv6GapxUCI](https://www.youtube.com/watch?v=Vcv6GapxUCI)

#### Using Terraform to manage Kubernetes on GCP

[HashCorp Terraform Kubernetes Tutorials](https://learn.hashicorp.com/tutorials/terraform/gke?in=terraform/kubernetes)

#### Create an App on GKE

https://ide.cloud.google.com/?walkthrough_tutorial_id=gke_cloud_code_create_app


#### Setting up GKE with Terraform Cloud

https://medium.com/@kuszner/setting-up-gke-with-terraform-cloud-bf9dfb5d1c8b

#### GKE and Ambassador

https://blog.searce.com/ambassador-with-google-kubernetes-engine-gke-d80571ef0525

