[Google Container Registry](https://cloud.google.com/container-registry)  is a private container image registry that runs on Google Cloud infrastructure. You can access Container Registry through secure HTTPS endpoints, which allow you to push, pull, and manage images from any system, VM instance, or your own hardware. Additionally, you can use the [Docker credential helper](https://cloud.google.com/container-registry/docs/advanced-authentication#docker_credential_helper) command-line tool to configure Docker to authenticate directly with Container Registry.

While Docker provides a central registry for storing public images, you might not want your images to be accessible to the world. To control access to your images, you can store your images in a private registry.

https://docs.docker.com/registry/


## QwikStart

https://cloud.google.com/container-registry/docs/quickstart

##  Logging into a private registry from GKE and GCE

https://blog.devgenius.io/google-container-registry-gcr-logging-into-a-private-registry-from-gke-gce-docker-e627643e47c5