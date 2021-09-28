[GitOps](https://www.gitops.tech/) is a way of implementing Continuous Deployment for cloud native applications. It focuses on a developer-centric experience when operating infrastructure, by using tools developers are already familiar with, including Git and Continuous Deployment tools.

The core idea of [GitOps](https://www.weave.works/technologies/gitops/) is having a Git repository that always contains declarative descriptions of the infrastructure currently desired in the production environment and an automated process to make the production environment match the described state in the repository. If you want to deploy a new application or update an existing one, you only need to update the repository - the automated process handles everything else. It’s like having cruise control for managing your applications in production.


GitOps is a way to do application delivery. It works by using [Git](https://git-scm.com/) as a single source of truth for [declarative infrastructure and applications](https://en.wikipedia.org/wiki/Infrastructure_as_code), together with tools ensuring the _actual state_ of infrastructure and applications converges towards the _desired state_ declared in Git. With Git at the center of your delivery pipelines, developers can make pull requests to accelerate and simplify application deployments and operations tasks to your infrastructure or container-orchestration system (e.g. [Kubernetes](Kubernetes)).

The term GitOps was [first coined by Weaveworks](https://www.weave.works/blog/gitops-operations-by-pull-request), and its key concept is using a Git repository to store the environment state that you want. 

[https://github.com/weaveworks/awesome-gitops](https://github.com/weaveworks/awesome-gitops)


## GitOps style continuous delivery with Cloud Build

https://cloud.google.com/kubernetes-engine/docs/tutorials/gitops-cloud-build

## GitOps, GKE, Cloud Build

https://medium.com/google-cloud/how-to-apply-gitops-cd-with-gke-and-cloud-build-in-5-minutes-58455a2bf063

## KubeStack

Terraform [GitOps Framework](https://www.kubestack.com/).

## Argo CD
https://github.com/argoproj/argo-cd

### Argo and GitOps

https://www.cncf.io/blog/2020/12/17/solving-configuration-drift-using-gitops-with-argo-cd/


### Argo CD Terraform module

https://www.kubestack.com/catalog/argo-cd

## Terraform GitOps via Cloud Build

This tutorial explains how to manage infrastructure as code with [Terraform](https://cloud.google.com/docs/terraform) and [Cloud Build](https://cloud.google.com/cloud-build) using the popular [GitOps](https://thenewstack.io/what-is-gitops-and-why-it-might-be-the-next-big-thing-for-devops/) methodology. 

The tutorial uses [Cloud Build](https://cloud.google.com/cloud-build) to automatically apply Terraform manifests to your environment.

https://cloud.google.com/architecture/managing-infrastructure-as-code

## Building docker images with github actions

https://medium.com/@flowsquad/building-docker-images-with-github-actions-and-google-cloud-b8894e0edff0


## Gitlab GitOps with Anthos

[https://www.youtube.com/watch?v=npc08ggdTOw](https://www.youtube.com/watch?v=npc08ggdTOw)

## List of GitOps resources

https://github.com/weaveworks/awesome-gitops