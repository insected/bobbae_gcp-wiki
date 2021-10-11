
[DevOps](https://cloud.google.com/devops/) is an organizational and cultural movement that aims to increase software delivery velocity, improve service reliability, and build shared ownership among software stakeholders. 

The goal of [DevOps](https://en.wikipedia.org/wiki/DevOps) is to build better, faster and more responsive software by bringing Development and Operations teams together. [DevOps](https://devops-research.com/) is not a methodology or [a suite of tools](https://en.wikipedia.org/wiki/DevOps_toolchain) but a cultural shift to remove the barriers between Dev and Ops in order to meet the need for shorter and more frequent software deliveries.

The [DevOps](   https://cloud.google.com/docs/tutorials?q=big%20data   ) cultural shift depends on continuously optimizing workflow, architecture, and infrastructure in order to deliver high-quality applications.

## Cloud Build

[Cloud Build](Cloud-Build) is a service that executes your builds on Google Cloud Platform's infrastructure.

## DevSecOps

[DevSecOps](https://resources.github.com/whitepapers/Architects-guide-to-DevOps/) isn’t just about development and operations teams. If you want to take full [advantage of the agility](https://tech.gsa.gov/guides/understanding_differences_agile_devsecops/) and responsiveness of a DevOps approach, [IT security](Security) and [privacy](Privacy) must also [play an integrated role](https://techbeacon.com/security/devsecops-realities-app-dev-teams-must-accept) in the [full life cycle of your apps](https://github.blog/2020-08-13-secure-at-every-step-a-guide-to-devsecops-shifting-left-and-gitops/).


DevSecOps is a culture shift in the software industry that aims to bake security into the rapid-release cycles that are typical of modern application development and deployment, also known as the DevOps movement. Embracing this [shift-left mentality](https://smartbear.com/learn/automated-testing/shifting-left-in-testing/) requires organizations to bridge the gap that usually exists between development and security teams to the point where many of the security processes are automated and handled by the development team itself.

### Security and Privacy

Please review some [security topics](Security) and [privacy issues](Privacy) from the [DevSecOps point of view](https://www.csoonline.com/article/3245748/what-is-devsecops-developing-more-secure-applications.html).

### Binary Authorization

[Binary Authorization](https://cloud.google.com/binary-authorization) is a deploy-time security control that ensures only trusted container images are deployed on Google Kubernetes Engine (GKE) or Cloud Run. With Binary Authorization, you can require images to be signed by trusted authorities during the development process and then enforce signature validation when deploying. By enforcing validation, you can gain tighter control over your container environment by ensuring only verified images are integrated into the build-and-release process.

## DevOps Research and Assessment

[Google’s DORA team](https://www.devops-research.com/research.html) conducted a six-year research program which validated a number of technical, process, measurement, and cultural capabilities that drive higher software delivery and organizational performance. Explore DORA’s research program and discover these capabilities, how to implement them, and how to overcome common obstacles.


## Hybrid Cloud DevOps

Running in a hybrid environment means that some of your processing happens on Google Cloud and other processing remains on-premises. [Anthos](Anthos) helps you manage both an on-premises [Kubernetes](Kubernetes) cluster and a cluster running on Google Cloud.
Google Kubernetes Engine (GKE) is the Kubernetes management and orchestration system for containers and Kubernetes clusters that run within Google's public cloud services.
Anthos clusters on [VMware](VMWare) runs privately on your own servers with regulated access to help meet your requirements for on-premises data processing.

## GitOps 

[GitOps](GitOps) is a way of implementing Continuous Deployment for cloud native applications. 





## CICD Tools

Many tools available: Jenkins X, Tekton, Docker, Helm, Skaffold, ChartMuseum, Knative, Prow, etc.

[https://www.youtube.com/watch?v=jXPn36d5Tog](https://www.youtube.com/watch?v=jXPn36d5Tog)

Building Kubernetes applications can require spending a lot of time on building containers, deploying them, and waiting to see changes. 


### Skaffold

[Skaffold](https://skaffold.dev/) handles the workflow for building, pushing and deploying your application.



[https://www.youtube.com/watch?v=TYx0BTyFtmc](https://www.youtube.com/watch?v=TYx0BTyFtmc)


### Jenkins 

[Jenkins](https://www.jenkins.io/) is one of the most popular CI systems in the world. 

[https://www.youtube.com/watch?v=IDoRWieTcMc](https://www.youtube.com/watch?v=IDoRWieTcMc)

Running Jenkins on Kubernetes.

https://cloud.google.com/architecture/jenkins-on-kubernetes-engine-tutorial

### JenkinsX

[Jenkins X](https://jenkins-x.io/) provides pipeline automation, built-in [GitOps](GitOps).

Try [this tutorial installing and deploying](https://itnext.io/deploy-a-basic-python-application-using-jenkins-x-kubernetes-4adace2fe345) a python app to kubernetes via jenkins X.


### Spinnaker

Use [Spinnaker](Spinnaker) to build a container based CI/CD pipeline leveraging Google Cloud Platform  tools.



[https://www.youtube.com/watch?v=DQIu373gSKU](https://www.youtube.com/watch?v=DQIu373gSKU)

#### Automating Canary Analysis on Google Kubernetes Engine with Spinnaker

https://cloud.google.com/architecture/automated-canary-analysis-kubernetes-engine-spinnaker

#### Spinnaker vs Jenkins

https://www.opsmx.com/blog/jenkins-vs-spinnaker/


### ArgoCD

[Argo CD](https://argoproj.github.io/argo-cd/) is a declarative, [GitOps](GitOps) continuous delivery tool for Kubernetes.


[https://www.youtube.com/watch?v=35Qimb_AZ8U](https://www.youtube.com/watch?v=35Qimb_AZ8U)

https://faun.pub/exploring-argocd-for-deployment-in-gke-or-any-kubernetes-cluster-aa935839d1fe





### Bamboo

Atlassian CICD tool.

https://www.atlassian.com/software/bamboo

### Travis

Travis CI enables your team to test and ship your apps.

https://travis-ci.org/

### Tekton

[Tekton](https://tekton.dev/
) is a cloud native continuous integration and delivery (CI/CD) solution. It allows developers to build, test, and deploy across cloud providers and on-premise systems. [Tekton](https://cloud.google.com/tekton
) is a powerful yet flexible Kubernetes-native open-source framework for creating continuous integration and delivery (CI/CD) systems. It lets you [build, test, and deploy across multiple cloud providers or on-premises systems](https://martinheinz.dev/blog/45
) by abstracting away the underlying implementation details.


## Build Tools

### Kaniko

[kaniko](https://github.com/GoogleContainerTools/kaniko
) is a tool to build container images from a Dockerfile, inside a container or Kubernetes cluster.



### buildah

[Buildah](https://github.com/containers/buildah
) is a tool that facilitates building [Open Container Initiative](https://opencontainers.org/)  (OCI) container images.



### pouch

[Pouch](https://github.com/alibaba/pouch
) is a Alibaba container engine.


### k3c

[K3c](https://github.com/ibuildthecloud/k3c
) is a Lightweight local container engine for container development.


### Buildkit

[BuildKit](https://github.com/moby/buildkit
) is a toolkit  for converting source code to build artifacts. It is party of [Moby Project](https://github.com/moby/moby).



### podmon

[Podman](https://podman.io/
) is a daemonless container engine for developing, managing, and running OCI Containers on your Linux System.



### Jib

[Jib](https://cloud.google.com/blog/products/application-development/introducing-jib-build-java-docker-images-better) is a tool to Build optimized containers for your Java applications.

[https://www.youtube.com/watch?v=p36tv1YWIfU](https://www.youtube.com/watch?v=p36tv1YWIfU)

### ko


[Ko](https://github.com/google/ko
) lets you Build and deploy Go applications on Kubernetes.

## Testing

A successful DevOps [testing strategy](https://smartbear.com/blog/devops-testing-strategy-best-practices-tools/
) is one aimed at building, testing and releasing software faster and more frequently. If you're lucky enough to start out in a "greenfield" organization without an established coding culture, it's a good idea to try to create and automate your software delivery pipeline upfront.



### Chaos Monkey

[Chaos Monkey](https://netflix.github.io/chaosmonkey/) is responsible for randomly terminating instances in production to ensure that engineers implement their services to be resilient to instance failures.


### Distributed load testing using Google Kubernetes Engine

https://cloud.google.com/architecture/distributed-load-testing-using-gke

## Building Containers without docker

https://blog.alexellis.io/building-containers-without-docker/

## DataOps vs MLOps

[DataOps](DataOps) takes the practices and values of DevOps and extends it to data analytics workflows and goals. It applies the focus on collaboration and shared responsibility and shifts it to the engineers and admins that collect, store, analyze, secure, and deliver data.

* [DataOps](https://en.wikipedia.org/wiki/DataOps) is an automated, process-oriented methodology, used by analytic and data teams, to improve the quality and reduce the cycle time of data analytics.

* [MLOps](MLOps) is a practice for collaboration and communication between data scientists and operations professionals to help manage the production of ML lifecycle. MLOps looks to increase automation and [improve the quality of production ML](https://towardsdatascience.com/devsecops-vs-dataops-vs-mlops-93b49f0282b8)  while also focusing on business and regulatory requirements.


## Ops terminology

https://thenewstack.io/dataops-and-the-problem-with-ops-terminology/

## SRE

[SRE](SRE) is what you get when you treat operations as if it's a software problem.

## Examples



### Testing Cloud Functions using Cloud Build and Terraform

https://cloud.google.com/architecture/system-testing-cloud-functions-using-cloud-build-and-terraform

### GitOps-style continuous delivery with Cloud Build

https://cloud.google.com/kubernetes-engine/docs/tutorials/gitops-cloud-build

### Creating and managing build triggers

https://cloud.google.com/build/docs/automating-builds/create-manage-triggers

### Building from github repository

https://cloud.google.com/build/docs/automating-builds/build-repos-from-github


### Mirroring a repository

https://cloud.google.com/source-repositories/docs/mirroring-repositories


### DevSecOps Case Study

https://cloud.google.com/architecture/partners/a-hybrid-cloud-native-devsecops-pipeline-with-jfrog-artifactory-and-gke-on-prem


## Qwiklabs

[DevOps Essentials](https://www.qwiklabs.com/quests/96?catalog_rank=%7B%22rank%22%3A3%2C%22num_filters%22%3A1%2C%22has_search%22%3Atrue%7D&search_id=7467726)


https://www.qwiklabs.com/quests/141



### SRE, SLI, SLA, SLO


https://www.qwiklabs.com/focuses/4186?parent=catalog
