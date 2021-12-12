[Cloud Build ](https://cloud.google.com/build/docs/overview) is a service that executes your builds on Google Cloud Platform's infrastructure.

## Cloud Code

Using [Cloud Code](https://cloud.google.com/code)  with Kubernetes.

[https://www.youtube.com/watch?v=KNd0mTxcQ_M](https://www.youtube.com/watch?v=KNd0mTxcQ_M)


## Cloud Build

[Cloud Build](https://cloud.google.com/build/docs)  is a service that executes your builds on Google Cloud Platform infrastructure. Cloud Build can import source code from Google Cloud Storage, Cloud Source Repositories, GitHub, or Bitbucket, execute a build to your specifications, and produce artifacts such as Docker containers or Java archives.

<!--
<img src="https://i.redd.it/uscxzz8hwmc41.png" width="500">
-->

### Overview

https://cloud.google.com/build/docs/overview

[https://www.youtube.com/watch?v=w7dMHiEyGAs](https://www.youtube.com/watch?v=w7dMHiEyGAs)

Cloud Build executes your build as a series of build steps, where each build step is run in a Docker container. A build step can do anything that can be done from a container irrespective of the environment. To perform your tasks, you can either [use the supported build steps](https://cloud.google.com/cloud-build/docs/configuring-builds/build-test-deploy-artifacts) provided by Cloud Build or [write your own build steps](https://cloud.google.com/cloud-build/docs/create-custom-build-steps).

[https://cloud.google.com/cloud-build/docs](https://cloud.google.com/cloud-build/docs)

### Starting a build from command line and API

https://cloud.google.com/build/docs/running-builds/start-build-command-line-api



### Creating and managing build triggers

https://cloud.google.com/build/docs/automating-builds/create-manage-triggers#gcloud_2



### Configuring the order of build steps

https://cloud.google.com/build/docs/configuring-builds/configure-build-step-order


### Speeding up builds

https://cloud.google.com/build/docs/speeding-up-builds

### Audit logging

https://cloud.google.com/build/docs/securing-builds/audit-logs
### Deploying to GKE

https://cloud.google.com/build/docs/deploying-builds/deploy-gke

### Git deploy

https://github.com/glasnt/git-deploy


## Container Registry

[Google Container Registry](https://cloud.google.com/container-registry)  is a private container image registry that runs on Google Cloud's reliable, fast, and secure infrastructure. You can access Container Registry through secure HTTPS endpoints, which allow you to push, pull, and manage images from any system, VM instance, or your own hardware. Additionally, you can use the [Docker credential helper](https://cloud.google.com/container-registry/docs/advanced-authentication#docker_credential_helper) command-line tool to configure Docker to authenticate directly with Container Registry.

While Docker provides a central registry for storing public images, you might not want your images to be accessible to the world. To control access to your images, you must store your images in a private registry.

[Container Registry: Qwik Start](https://www.qwiklabs.com/focuses/1768?catalog_rank=%7B%22rank%22%3A7%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&parent=catalog&search_id=7467880)


## Examples

### Cloud Build Notifications in Google Chat


https://devopsquare.com/cloud-build-notifications-in-google-chat-317d277c5d4a


### Cloud Build Email

https://medium.com/datamindedbe/sending-mail-from-google-cloud-build-8b15da779c8f
