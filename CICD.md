
[CI/CD](https://en.wikipedia.org/wiki/CI/CD) bridges the gaps between development and operation activities and teams by enforcing automation in building, testing and deployment of applications. 

[DevOps](DevOps) practices involve continuous development, continuous testing, continuous integration, continuous deployment and continuous monitoring of software applications throughout its development life cycle.

### Cloud Build

[Cloud Build](Cloud-Build) is a service that executes your builds on Google Cloud Platform's infrastructure.

### Cloud Deploy

https://cloud.google.com/blog/products/devops-sre/google-cloud-deploy-now-ga

#### Deploying to GKE

https://davelms.medium.com/automate-gke-deployments-using-cloud-build-and-cloud-deploy-2c15909ddf22

https://blog.searce.com/deploy-applications-to-gke-using-google-cloud-deploy-f1fda8618966

### Selective deployment

https://github.com/GoogleCloudPlatform/professional-services/tree/main/examples/cloudbuild-selective-deployment


### CICD Pipelines with Cloud Build and Artifact Registry

https://dev.to/brianburton/cloud-build-docker-and-artifact-registry-cicd-pipelines-with-private-packages-5ci2

## CICD Tools

[https://www.youtube.com/watch?v=jXPn36d5Tog](https://www.youtube.com/watch?v=jXPn36d5Tog)

Building Kubernetes applications can require spending a lot of time on building containers, deploying them, and waiting to see changes. 

https://www.guru99.com/top-20-continuous-integration-tools.html


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


https://awstip.com/deploying-java-spring-app-to-gke-using-argocd-d84837113ce9

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
) is a toolkit  for converting source code to build artifacts. It is a part of [Moby Project](https://github.com/moby/moby).



### podmon

[Podman](https://podman.io/
) is a daemonless container engine for developing, managing, and running OCI Containers on your Linux System.



### Jib

[Jib](https://cloud.google.com/blog/products/application-development/introducing-jib-build-java-docker-images-better) is a tool to build optimized containers for your Java applications.



[https://www.youtube.com/watch?v=p36tv1YWIfU](https://www.youtube.com/watch?v=p36tv1YWIfU)



### jib and skaffold 

https://medium.com/google-cloud/building-and-deploying-containerized-application-to-kubernetes-using-jib-and-skaffold-80305363a8fd

### ko


[Ko](https://github.com/google/ko
) lets you build and deploy Go applications on Kubernetes.

## Testing

A successful DevOps [testing strategy](https://smartbear.com/blog/devops-testing-strategy-best-practices-tools/
) is one aimed at building, testing and releasing software faster and more frequently. If you're lucky enough to start out in a "greenfield" organization without an established coding culture, it's a good idea to try to create and automate your software delivery pipeline upfront.



### Chaos Monkey

[Chaos Monkey](https://netflix.github.io/chaosmonkey/) is responsible for randomly terminating instances in production to ensure that engineers implement their services to be resilient to instance failures.

### gremlin

https://medium.com/google-cloud/gremlin-chaos-engineering-on-google-cloud-2568f9fc70c9

### Distributed load testing using Google Kubernetes Engine

https://cloud.google.com/architecture/distributed-load-testing-using-gke

## Building Containers without docker

https://blog.alexellis.io/building-containers-without-docker/

## Gitlab and GKE

https://blog.searce.com/gitlab-ci-cd-to-deploy-applications-on-gke-using-shared-runner-47f8c42817ac

## Deploying Cloud Functions with GitLab CI/CD

https://towardsdev.com/deploying-cloud-functions-with-gitlab-ci-cd-960e707d217a

## Cloud Deploy and GKE

https://blog.searce.com/deploy-applications-to-gke-using-google-cloud-deploy-f1fda8618966

## CICD Pipeline as Code using Terraform

https://genekuo.medium.com/setting-up-a-ci-cd-pipeline-on-gcp-with-terraform-539e66797072

## CICD with Cloud Build on Compute Engine
https://blog.searce.com/ci-cd-with-cloud-build-on-compute-engine-451ccb7b8a1
