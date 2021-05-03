
### Cloud Code

Using [Cloud Code](https://cloud.google.com/code)  with Kubernetes.

[https://www.youtube.com/watch?v=KNd0mTxcQ_M](https://www.youtube.com/watch?v=KNd0mTxcQ_M)


### Cloud Build

[Cloud Build](https://cloud.google.com/build/docs)  is a service that executes your builds on Google Cloud Platform infrastructure. Cloud Build can import source code from Google Cloud Storage, Cloud Source Repositories, GitHub, or Bitbucket, execute a build to your specifications, and produce artifacts such as Docker containers or Java archives.

<img src="https://i.redd.it/uscxzz8hwmc41.png" width="500">

A video about Cloud Build with Containers.

[https://www.youtube.com/watch?v=w7dMHiEyGAs](https://www.youtube.com/watch?v=w7dMHiEyGAs)

Cloud Build executes your build as a series of build steps, where each build step is run in a Docker container. A build step can do anything that can be done from a container irrespective of the environment. To perform your tasks, you can either [use the supported build steps](https://cloud.google.com/cloud-build/docs/configuring-builds/build-test-deploy-artifacts) provided by Cloud Build or [write your own build steps](https://cloud.google.com/cloud-build/docs/create-custom-build-steps).

[https://cloud.google.com/cloud-build/docs](https://cloud.google.com/cloud-build/docs)


### Container Registry

Google Container Registry is a private container image registry that runs on Google Cloud's reliable, fast, and secure infrastructure. You can access Container Registry through secure HTTPS endpoints, which allow you to push, pull, and manage images from any system, VM instance, or your own hardware. Additionally, you can use the [Docker credential helper](https://cloud.google.com/container-registry/docs/advanced-authentication#docker_credential_helper) command-line tool to configure Docker to authenticate directly with Container Registry.

While Docker provides a central registry for storing public images, you might not want your images to be accessible to the world. To control access to your images, you must store your images in a private registry.

[Container Registry: Qwik Start](https://www.qwiklabs.com/focuses/1768?catalog_rank=%7B%22rank%22%3A7%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&parent=catalog&search_id=7467880)
