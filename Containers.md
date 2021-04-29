
## What is a container?

A container is a standard unit of software that packages up code and all its dependencies so the application runs quickly and reliably from one computing environment to another. A Docker container image is a lightweight, standalone, executable package of software that includes everything needed to run an application: code, runtime, system tools, system libraries and settings.

[https://www.docker.com/resources/what-container](https://www.docker.com/resources/what-container)

### Container Images

A container image is a ready-to-run software package, containing everything needed to run an application: the code and any runtime it requires, application and system libraries, and default values for any essential settings.

By design, a container is immutable: you cannot change the code of a container that is already running. If you have a containerized application and want to make changes, you need to build a new image that includes the change, then recreate the container to start from the updated image.

Container images use [Union Filesystems](https://en.wikipedia.org/wiki/UnionFS). In Linux, docker originally use AUFS but they use OverlayFS now.  The details of union filesystem use in docker container images can be found at https://martinheinz.dev/blog/44.


## Container runtimes

The container runtime is the software that is responsible for running containers.

Kubernetes supports several container runtimes: Docker, [containerd](https://containerd.io/), [CRI-O](https://cri-o.io), and any implementation of the Kubernetes CRI (Container Runtime Interface).


## Containers vs. VMs

Virtual machines and containers differ in several ways, but the primary difference is that containers provide a way to virtualize an OS so that multiple workloads can run on a single OS instance. With VMs, the hardware is being virtualized to run multiple OS instances. Containers’ speed, agility, and portability make them yet another tool to help streamline software development.

https://www.weave.works/blog/a-practical-guide-to-choosing-between-docker-containers-and-vms

### Comparison of containerizing vs using VMs

[https://www.youtube.com/watch?v=TvnZTi_gaNc](https://www.youtube.com/watch?v=TvnZTi_gaNc)


## Three ways to run containers in GCP

Find out the top three ways you can run your containers on Google Cloud! Google Kubernetes Engine for a container orchestration solution, Cloud Run for a fully serverless approach and Compute Engine to simply use Virtual Machines.

[https://www.youtube.com/watch?v=jh0fPT-AWwM](https://www.youtube.com/watch?v=jh0fPT-AWwM)
