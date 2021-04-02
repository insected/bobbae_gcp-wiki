- [DevOps](#devops)
  * [Introduction](#introduction)
  * [Jenkins & GKE](#jenkins---gke)
  * [Spinnaker](#spinnaker)
  * [Jib](#jib)
  * [Kubernetes CI/CD](#kubernetes-ci-cd)
    + [Security](#security)
      - [StackRox](#stackrox)
      - [Binary Authorization Attestations with Voucher](#binary-authorization-attestations-with-voucher)
  * [GitOps](#gitops)
    + [Tutorial](#tutorial)
    + [Gitlab Gitops with Anthos](#gitlab-gitops-with-anthos)
  * [ArgoCD](#argocd)
  * [Chaos Monkey](#chaos-monkey)

<small><i><a href='http://ecotrust-canada.github.io/markdown-toc/'>Table of contents generated with markdown-toc</a></i></small>

## DevOps


### Introduction

[DevOps](https://cloud.google.com/devops/) is an organizational and cultural movement that aims to increase software delivery velocity, improve service reliability, and build shared ownership among software stakeholders. In this quest you will learn how to use Google Cloud to improve the speed, stability, availability, and security of your software delivery capability. [DevOps Research and Assessment](https://devops-research.com/) has joined Google Cloud. How does your team measure up? [Take this five multiple-choice question quiz](https://beta.devops-research.com/quickcheck.html) and find out! 

[DevOps Essentials](https://www.qwiklabs.com/quests/96?catalog_rank=%7B%22rank%22%3A3%2C%22num_filters%22%3A1%2C%22has_search%22%3Atrue%7D&search_id=7467726)


### Jenkins & GKE

Jenkins is one of the most popular CI systems in the world. It’s flexibility and ecosystem allow it to be used for almost any task.

[https://www.youtube.com/watch?v=IDoRWieTcMc](https://www.youtube.com/watch?v=IDoRWieTcMc)


### Spinnaker

Build a container based CI/CD pipeline leveraging Google Cloud Platform  tools along with open source tool Spinnaker for deployment. 

[https://www.youtube.com/watch?v=DQIu373gSKU](https://www.youtube.com/watch?v=DQIu373gSKU)


### Jib

Build optimized containers for your Java applications.

[https://www.youtube.com/watch?v=p36tv1YWIfU](https://www.youtube.com/watch?v=p36tv1YWIfU)


### Kubernetes CI/CD

This session demonstrates how using the best tools in the Kubernetes ecosystem, such as Jenkins X, Tekton, Docker, Helm, Skaffold, ChartMuseum, Knative, Prow and others can help you create a fully automated setup. 

[https://www.youtube.com/watch?v=jXPn36d5Tog](https://www.youtube.com/watch?v=jXPn36d5Tog)

Kubernetes had become the orchestrator of choice to deploy applications — but what about a developer’s day to day job? Building Kubernetes applications can require spending a lot of time on building containers, deploying them, and waiting to see changes. Developing applications on Kubernetes doesn’t have to be difficult, and this talk will show you how to leverage local development tools like Skaffold and Google Cloud Build to develop at 10x velocity. We’ll cover how Skaffold intelligently rebuilds and redeploys your application on every code change, all from the comfort of your favorite IDE. We’ll then go over how to use Skaffold and Google Cloud Build to easily deploy a robust CI/CD pipeline from GitHub to GKE, simplifying your local development experience from start to finish.

[https://www.youtube.com/watch?v=TYx0BTyFtmc](https://www.youtube.com/watch?v=TYx0BTyFtmc)


#### Security


##### StackRox

[https://www.stackrox.com/post/2020/11/stackrox-integrates-with-google-artifact-registry/](https://www.stackrox.com/post/2020/11/stackrox-integrates-with-google-artifact-registry/)


##### Binary Authorization Attestations with Voucher

[https://cloud.google.com/binary-authorization/docs/creating-attestations-voucher](https://cloud.google.com/binary-authorization/docs/creating-attestations-voucher)


### GitOps 

GitOps is a way to do application delivery. It works by using [Git](https://git-scm.com/) as a single source of truth for [declarative infrastructure and applications](https://en.wikipedia.org/wiki/Infrastructure_as_code), together with tools ensuring the _actual state_ of infrastructure and applications converges towards the _desired state_ declared in Git. With Git at the center of your delivery pipelines, developers can make pull requests to accelerate and simplify application deployments and operations tasks to your infrastructure or container-orchestration system (e.g. [Kubernetes](https://kubernetes.io/)).

[https://github.com/weaveworks/awesome-gitops](https://github.com/weaveworks/awesome-gitops)


#### Tutorial

This tutorial explains how to manage infrastructure as code with [Terraform](https://cloud.google.com/docs/terraform) and [Cloud Build](https://cloud.google.com/cloud-build) using the popular [GitOps](https://thenewstack.io/what-is-gitops-and-why-it-might-be-the-next-big-thing-for-devops/) methodology. The term GitOps was [first coined by Weaveworks](https://www.weave.works/blog/gitops-operations-by-pull-request), and its key concept is using a Git repository to store the environment state that you want. Terraform is a [HashiCorp](https://www.hashicorp.com/) open source tool that enables you to predictably create, change, and improve your cloud infrastructure by using code. In this tutorial, you use [Cloud Build](https://cloud.google.com/cloud-build), a Google Cloud continuous integration service, to automatically apply Terraform manifests to your environment.

[https://cloud.google.com/solutions/managing-infrastructure-as-code](https://cloud.google.com/solutions/managing-infrastructure-as-code)


#### Gitlab Gitops with Anthos

[https://www.youtube.com/watch?v=npc08ggdTOw](https://www.youtube.com/watch?v=npc08ggdTOw)


### ArgoCD

[https://www.youtube.com/watch?v=35Qimb_AZ8U](https://www.youtube.com/watch?v=35Qimb_AZ8U)


### Chaos Monkey

[https://netflix.github.io/chaosmonkey/](https://netflix.github.io/chaosmonkey/)


