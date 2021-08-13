

## Introduction

[DevOps](https://cloud.google.com/devops/) is an organizational and cultural movement that aims to increase software delivery velocity, improve service reliability, and build shared ownership among software stakeholders. 

The goal of [DevOps](https://en.wikipedia.org/wiki/DevOps) is to build better, faster and more responsive software by bringing Development and Operations teams together. [DevOps](https://devops-research.com/) is not a methodology or [a suite of tools](https://en.wikipedia.org/wiki/DevOps_toolchain) but a cultural shift to remove the barriers between Dev and Ops in order to meet the need for shorter and more frequent software deliveries.


This will allow your organization to respond in a more agile manner to changing business requirements. The [DevOps](   https://cloud.google.com/docs/tutorials?q=big%20data   ) cultural shift depends on continuously optimizing workflow, architecture, and infrastructure in order to deliver high-quality applications.



## DevSecOps

[DevSecOps](https://resources.github.com/whitepapers/Architects-guide-to-DevOps/) isn’t just about development and operations teams. If you want to take full [advantage of the agility](https://tech.gsa.gov/guides/understanding_differences_agile_devsecops/) and responsiveness of a DevOps approach, [IT security](Security) and [privacy](Privacy) must also [play an integrated role](https://techbeacon.com/security/devsecops-realities-app-dev-teams-must-accept) in the [full life cycle of your apps](https://github.blog/2020-08-13-secure-at-every-step-a-guide-to-devsecops-shifting-left-and-gitops/).


DevSecOps is a culture shift in the software industry that aims to bake security into the rapid-release cycles that are typical of modern application development and deployment, also known as the DevOps movement. Embracing this shift-left mentality requires organizations to bridge the gap that usually exists between development and security teams to the point where many of the security processes are automated and handled by the development team itself.

### Security and Privacy

Please review some [security topics](Security) and [privacy issues](Privacy) from the [DevSecOps point of view](https://www.csoonline.com/article/3245748/what-is-devsecops-developing-more-secure-applications.html).




### DevSecOps Case Study

https://cloud.google.com/architecture/partners/a-hybrid-cloud-native-devsecops-pipeline-with-jfrog-artifactory-and-gke-on-prem

### Binary Authorization

Binary Authorization is a deploy-time security control that ensures only trusted container images are deployed on Google Kubernetes Engine (GKE) or Cloud Run. With Binary Authorization, you can require images to be signed by trusted authorities during the development process and then enforce signature validation when deploying. By enforcing validation, you can gain tighter control over your container environment by ensuring only verified images are integrated into the build-and-release process.


https://cloud.google.com/binary-authorization

## DevOps Research and Assessment

[Google’s DORA team](https://www.devops-research.com/research.html) conducted a six-year research program which validated a number of technical, process, measurement, and cultural capabilities that drive higher software delivery and organizational performance. Explore DORA’s research program and discover these capabilities, how to implement them, and how to overcome common obstacles.


## Hybrid Cloud DevOps

Running in a hybrid environment means that some of your processing happens on Google Cloud and other processing remains on-premises. Anthos helps you manage both an on-premises Kubernetes cluster and a cluster running on Google Cloud.
Google Kubernetes Engine (GKE) is the Kubernetes management and orchestration system for containers and Kubernetes clusters that run within Google's public cloud services.
Anthos clusters on VMware runs privately on your own servers with regulated access to help meet your requirements for on-premises data processing.
## GitOps 



[GitOps](https://www.gitops.tech/) is a way of implementing Continuous Deployment for cloud native applications. It focuses on a developer-centric experience when operating infrastructure, by using tools developers are already familiar with, including Git and Continuous Deployment tools.

The core idea of [GitOps](https://www.weave.works/technologies/gitops/) is having a Git repository that always contains declarative descriptions of the infrastructure currently desired in the production environment and an automated process to make the production environment match the described state in the repository. If you want to deploy a new application or update an existing one, you only need to update the repository - the automated process handles everything else. It’s like having cruise control for managing your applications in production.


GitOps is a way to do application delivery. It works by using [Git](https://git-scm.com/) as a single source of truth for [declarative infrastructure and applications](https://en.wikipedia.org/wiki/Infrastructure_as_code), together with tools ensuring the _actual state_ of infrastructure and applications converges towards the _desired state_ declared in Git. With Git at the center of your delivery pipelines, developers can make pull requests to accelerate and simplify application deployments and operations tasks to your infrastructure or container-orchestration system (e.g. [Kubernetes](https://kubernetes.io/)).

The term GitOps was [first coined by Weaveworks](https://www.weave.works/blog/gitops-operations-by-pull-request), and its key concept is using a Git repository to store the environment state that you want. 

[https://github.com/weaveworks/awesome-gitops](https://github.com/weaveworks/awesome-gitops)


#### GitOps style continuous delivery with Cloud Build

https://cloud.google.com/kubernetes-engine/docs/tutorials/gitops-cloud-build


### KubeStack

Terraform [GitOps Framework](https://www.kubestack.com/).



### Cloud Build Tutorial

This tutorial explains how to manage infrastructure as code with [Terraform](https://cloud.google.com/docs/terraform) and [Cloud Build](https://cloud.google.com/cloud-build) using the popular [GitOps](https://thenewstack.io/what-is-gitops-and-why-it-might-be-the-next-big-thing-for-devops/) methodology. 

Use [Cloud Build](https://cloud.google.com/cloud-build), a Google Cloud [continuous integration service, to automatically apply Terraform manifests to your environment](https://cloud.google.com/solutions/managing-infrastructure-as-code).



### Gitlab Gitops with Anthos

[https://www.youtube.com/watch?v=npc08ggdTOw](https://www.youtube.com/watch?v=npc08ggdTOw)


## CICD Tools

Many tools available: Jenkins X, Tekton, Docker, Helm, Skaffold, ChartMuseum, Knative, Prow, etc.

[https://www.youtube.com/watch?v=jXPn36d5Tog](https://www.youtube.com/watch?v=jXPn36d5Tog)

Building Kubernetes applications can require spending a lot of time on building containers, deploying them, and waiting to see changes. 


### Skaffold

Skaffold handles the workflow for building, pushing and deploying your application.

https://skaffold.dev/

[https://www.youtube.com/watch?v=TYx0BTyFtmc](https://www.youtube.com/watch?v=TYx0BTyFtmc)


### Jenkins 

Jenkins is one of the most popular CI systems in the world. 

[https://www.youtube.com/watch?v=IDoRWieTcMc](https://www.youtube.com/watch?v=IDoRWieTcMc)

Running Jenkins on Kubernetes.

https://cloud.google.com/architecture/jenkins-on-kubernetes-engine-tutorial

### JenkinsX

Jenkins X provides pipeline automation, built-in GitOps.


https://jenkins-x.io/

Try [this tutorial installing and deploying](https://itnext.io/deploy-a-basic-python-application-using-jenkins-x-kubernetes-4adace2fe345) a python app to kubernetes via jenkins X.


### Spinnaker

Build a container based CI/CD pipeline leveraging Google Cloud Platform  tools along with open source tool Spinnaker for deployment. 

[https://www.youtube.com/watch?v=DQIu373gSKU](https://www.youtube.com/watch?v=DQIu373gSKU)

#### Automating Canary Analysis on Google Kubernetes Engine with Spinnaker

https://cloud.google.com/architecture/automated-canary-analysis-kubernetes-engine-spinnaker

### ArgoCD

Argo CD is a declarative, GitOps continuous delivery tool for Kubernetes.


[https://www.youtube.com/watch?v=35Qimb_AZ8U](https://www.youtube.com/watch?v=35Qimb_AZ8U)







### Bamboo

Atlassian CICD tool.

https://www.atlassian.com/software/bamboo

### Travis

Travis CI enables your team to test and ship your apps.

https://travis-ci.org/

### Tekton

Tekton is a cloud native continuous integration and delivery (CI/CD) solution. It allows developers to build, test, and deploy across cloud providers and on-premise systems. Tekton is a powerful yet flexible Kubernetes-native open-source framework for creating continuous integration and delivery (CI/CD) systems. It lets you build, test, and deploy across multiple cloud providers or on-premises systems by abstracting away the underlying implementation details.

https://cloud.google.com/tekton

https://tekton.dev/

https://martinheinz.dev/blog/45

## Build Tools

### Kaniko

kaniko is a tool to build container images from a Dockerfile, inside a container or Kubernetes cluster.


https://github.com/GoogleContainerTools/kaniko

### buildah

a tool that facilitates building [Open Container Initiative](https://opencontainers.org/)  (OCI) container images.

https://github.com/containers/buildah


### pouch

Alibaba container engine.

https://github.com/alibaba/pouch

### k3c

Lightweight local container engine for container development.

https://github.com/ibuildthecloud/k3c

### Buildkit

BuildKit is a toolkit  for converting source code to build artifacts. It is party of [Moby Project](https://github.com/moby/moby).


https://github.com/moby/buildkit

### podmon

Podman is a daemonless container engine for developing, managing, and running OCI Containers on your Linux System.

https://podman.io/


### Jib

Build optimized containers for your Java applications.

[https://www.youtube.com/watch?v=p36tv1YWIfU](https://www.youtube.com/watch?v=p36tv1YWIfU)

### ko

https://github.com/google/ko

Build and deploy Go applications on Kubernetes.

## Testing

A successful DevOps testing strategy is one aimed at building, testing and releasing software faster and more frequently. If you're lucky enough to start out in a "greenfield" organization without an established coding culture, it's a good idea to try to create and automate your software delivery pipeline upfront.

https://smartbear.com/blog/devops-testing-strategy-best-practices-tools/


### Chaos Monkey

Chaos Monkey is responsible for randomly terminating instances in production to ensure that engineers implement their services to be resilient to instance failures.

[https://netflix.github.io/chaosmonkey/](https://netflix.github.io/chaosmonkey/)

### Distributed load testing using Google Kubernetes Engine


https://cloud.google.com/architecture/distributed-load-testing-using-gke

## Building Containers without docker

https://blog.alexellis.io/building-containers-without-docker/


## DataOps vs MLOps


[DataOps](https://en.wikipedia.org/wiki/DataOps) takes the practices and values of DevOps and extends it to data analytics workflows and goals. It applies the focus on collaboration and shared responsibility and shifts it to the engineers and admins that collect, store, analyze, secure, and deliver data.

* DataOps is an automated, process-oriented methodology, used by analytic and data teams, to improve the quality and reduce the cycle time of data analytics.

* [MLOps](MLOps) is a practice for collaboration and communication between data scientists and operations professionals to help manage the production of ML lifecycle. MLOps looks to increase automation and [improve the quality of production ML](https://towardsdatascience.com/devsecops-vs-dataops-vs-mlops-93b49f0282b8)  while also focusing on business and regulatory requirements.









## Ops terminology

https://thenewstack.io/dataops-and-the-problem-with-ops-terminology/

## Qwiklabs

[DevOps Essentials](https://www.qwiklabs.com/quests/96?catalog_rank=%7B%22rank%22%3A3%2C%22num_filters%22%3A1%2C%22has_search%22%3Atrue%7D&search_id=7467726)


https://www.qwiklabs.com/quests/141

### SRE, SLI, SLA, SLO

https://www.qwiklabs.com/focuses/4186?parent=catalog
