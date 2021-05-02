
## What is a container?

A [container](https://www.freecodecamp.org/news/demystifying-containers-101-a-deep-dive-into-container-technology-for-beginners-d7b60d8511c1/)  is a standard unit of software that packages up code and all its dependencies so the application runs quickly and reliably from one computing environment to another. A Docker container image is a lightweight, standalone, executable package of software that includes everything needed to run an application: code, runtime, system tools, system libraries and settings.  

A [container](https://appfleet.com/blog/what-is-a-container-a-kernel-introduction/) is  attached to different [namespaces](https://opensource.com/article/19/10/namespaces-and-containers-linux).

[Namespaces](https://opensource.com/article/19/10/namespaces-and-containers-linux), along with other technologies like [cgroups](https://en.wikipedia.org/wiki/Cgroups) and [more](https://blog.scottlowe.org/2013/09/04/introducing-linux-network-namespaces/), form the foundation of containerization.

[https://www.docker.com/resources/what-container](https://www.docker.com/resources/what-container)

<img src="https://eglerean.github.io/reproducible-research/img/docker_architecture.svg" width="800">

### Container [Images](https://phoenixnap.com/kb/docker-image-vs-container)

A [container image](https://cloud.google.com/container-registry/docs/image-formats) is a ready-to-run software package, containing everything needed to run an application: the code and any runtime it requires, application and system libraries, and default values for any essential settings.

<img src="https://vitalflux.com/wp-content/uploads/2017/10/Screen-Shot-2017-10-07-at-9.26.42-PM.png" width="800">

By design, a container is immutable: you cannot change the code of a container that is already running. If you have a containerized application and want to make changes, you need to build a new image that includes the change, then recreate the container to start from the updated image.

Container images use [Union Filesystems](https://en.wikipedia.org/wiki/UnionFS). In Linux, docker originally use AUFS but they use OverlayFS now.  The details of union filesystem use in docker container images can be found at https://martinheinz.dev/blog/44.


## Container runtimes

The container runtime is the software that is responsible for running containers.

[Kubernetes](https://github.com/bobbae/gcp/wiki/Kubernetes-Engine-and-Containers) supports several container runtimes: Docker, [containerd](https://containerd.io/), [CRI-O](https://cri-o.io), and any implementation of the Kubernetes CRI (Container Runtime Interface).

## Containers vs. VMs

[Virtual machines](VM) and containers differ in several ways, but the primary difference is that containers provide a way to virtualize an OS so that multiple workloads can run on a single OS instance. With VMs, the hardware is being virtualized to run multiple OS instances. Containers’ speed, agility, and portability make them yet another tool to help streamline software development.



<img src="https://storage.googleapis.com/xebia-blog/1/2016/11/Container-vs-VMs.jpg" width="700">

https://www.weave.works/blog/a-practical-guide-to-choosing-between-docker-containers-and-vms

### Comparison of containerizing vs using VMs

[https://www.youtube.com/watch?v=TvnZTi_gaNc](https://www.youtube.com/watch?v=TvnZTi_gaNc)


## Three ways to run containers in GCP

Find out the top three ways you can run your containers on Google Cloud! Google Kubernetes Engine for a container orchestration solution, Cloud Run for a fully serverless approach and Compute Engine to simply use Virtual Machines.

[https://www.youtube.com/watch?v=jh0fPT-AWwM](https://www.youtube.com/watch?v=jh0fPT-AWwM)
