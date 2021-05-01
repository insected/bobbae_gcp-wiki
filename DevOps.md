[[https://tech.gsa.gov/assets/img/guides/DevSecOps.png]]


## Introduction

[DevOps](https://cloud.google.com/devops/) is an organizational and cultural movement that aims to increase software delivery velocity, improve service reliability, and build shared ownership among software stakeholders. 

## DevSecOps

DevOps isn’t just about development and operations teams. If you want to take full advantage of the agility and responsiveness of a DevOps approach, [IT security](https://www.redhat.com/en/topics/security) must also play an integrated role in the full life cycle of your apps.

https://www.devsecops.org/

https://tech.gsa.gov/guides/understanding_differences_agile_devsecops/


## Security

https://github.com/bobbae/gcp/wiki/Security


## DevOps Research and Assessment

https://devops-research.com/

## Hybrid Cloud DevOps

Running in a hybrid environment means that some of your processing happens on Google Cloud and other processing remains on-premises. Anthos helps you manage both an on-premises Kubernetes cluster and a cluster running on Google Cloud.

Google Kubernetes Engine (GKE) is the Kubernetes management and orchestration system for containers and Kubernetes clusters that run within Google's public cloud services.

Anthos clusters on VMware runs privately on your own servers with regulated access to help meet your requirements for on-premises data processing.

### Case Study

https://cloud.google.com/architecture/partners/a-hybrid-cloud-native-devsecops-pipeline-with-jfrog-artifactory-and-gke-on-prem



## GitOps 

GitOps is a way to do application delivery. It works by using [Git](https://git-scm.com/) as a single source of truth for [declarative infrastructure and applications](https://en.wikipedia.org/wiki/Infrastructure_as_code), together with tools ensuring the _actual state_ of infrastructure and applications converges towards the _desired state_ declared in Git. With Git at the center of your delivery pipelines, developers can make pull requests to accelerate and simplify application deployments and operations tasks to your infrastructure or container-orchestration system (e.g. [Kubernetes](https://kubernetes.io/)).

The term GitOps was [first coined by Weaveworks](https://www.weave.works/blog/gitops-operations-by-pull-request), and its key concept is using a Git repository to store the environment state that you want. 

[https://github.com/weaveworks/awesome-gitops](https://github.com/weaveworks/awesome-gitops)


### Cloud Build Tutorial

This tutorial explains how to manage infrastructure as code with [Terraform](https://cloud.google.com/docs/terraform) and [Cloud Build](https://cloud.google.com/cloud-build) using the popular [GitOps](https://thenewstack.io/what-is-gitops-and-why-it-might-be-the-next-big-thing-for-devops/) methodology. 

Use [Cloud Build](https://cloud.google.com/cloud-build), a Google Cloud continuous integration service, to automatically apply Terraform manifests to your environment.

[https://cloud.google.com/solutions/managing-infrastructure-as-code](https://cloud.google.com/solutions/managing-infrastructure-as-code)


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

### JenkinsX

Jenkins X provides pipeline automation, built-in GitOps.


https://jenkins-x.io/


### Spinnaker

Build a container based CI/CD pipeline leveraging Google Cloud Platform  tools along with open source tool Spinnaker for deployment. 

[https://www.youtube.com/watch?v=DQIu373gSKU](https://www.youtube.com/watch?v=DQIu373gSKU)


## ArgoCD

Argo CD is a declarative, GitOps continuous delivery tool for Kubernetes.


[https://www.youtube.com/watch?v=35Qimb_AZ8U](https://www.youtube.com/watch?v=35Qimb_AZ8U)







## Bamboo

Atlassian CICD tool.

https://www.atlassian.com/software/bamboo

## Travis

Travis CI enables your team to test and ship your apps.

https://travis-ci.org/

## Tekton

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


### Chaos Monkey

Chaos Monkey is responsible for randomly terminating instances in production to ensure that engineers implement their services to be resilient to instance failures.

[https://netflix.github.io/chaosmonkey/](https://netflix.github.io/chaosmonkey/)


## Building Containers without docker

https://blog.alexellis.io/building-containers-without-docker/

## Ops terminology

https://thenewstack.io/dataops-and-the-problem-with-ops-terminology/

## Qwiklabs

[DevOps Essentials](https://www.qwiklabs.com/quests/96?catalog_rank=%7B%22rank%22%3A3%2C%22num_filters%22%3A1%2C%22has_search%22%3Atrue%7D&search_id=7467726)


https://www.qwiklabs.com/quests/141
