
## What is a container?

A [container](https://www.freecodecamp.org/news/demystifying-containers-101-a-deep-dive-into-container-technology-for-beginners-d7b60d8511c1/)  is a standard unit of software that packages up code and all its dependencies so the application runs quickly and reliably from one computing environment to another. A [Docker container](https://www.docker.com/resources/what-container) image is a lightweight, standalone, executable package of software that includes everything needed to run an application: code, runtime, system tools, system libraries and settings.  

An [OS-level virtualization](https://en.wikipedia.org/wiki/OS-level_virtualization), different from [Virtual Machines](VM), is an operating system paradigm in which the kernel allows the existence of multiple isolated user space instances. Such instances, called containers ([LXC](https://linuxcontainers.org/), [Solaris containers](https://www.oracle.com/solaris/technologies/solaris-containers.html), Docker), [Zones](https://www.fujitsu.com/global/products/computing/servers/unix/sparc-enterprise/software/solaris10/container/zone/#:~:text=A%20Solaris%20Zone%20is%20a,where%20Solaris%20OS%20is%20installed.) (Solaris containers), virtual private servers ([OpenVZ](https://openvz.org/)), partitions, virtual environments (VEs), virtual kernels (DragonFly BSD), or [jails](https://en.wikipedia.org/wiki/FreeBSD_jail) (FreeBSD jail or chroot jail), may look like real computers from the point of view of programs running in them. A computer program running on an ordinary operating system can see all resources (connected devices, files and folders, network shares, CPU power, quantifiable hardware capabilities) of that computer. However, programs running inside of a container can only see the container's contents and devices assigned to the container.


A [container](https://appfleet.com/blog/what-is-a-container-a-kernel-introduction/) is  attached to different [namespaces](https://opensource.com/article/19/10/namespaces-and-containers-linux).

[Namespaces](Namespaces), along with other technologies like [cgroups](https://en.wikipedia.org/wiki/Cgroups) and [more](https://blog.scottlowe.org/2013/09/04/introducing-linux-network-namespaces/), form the foundation of containerization.

[https://www.docker.com/resources/what-container](https://www.docker.com/resources/what-container)


### Container Images

A [container image](https://cloud.google.com/container-registry/docs/image-formats) is a ready-to-run software package, containing everything needed to run an application: the code and any runtime it requires, application and system libraries, and default values for any essential settings.


By design, a [container is immutable](https://cloud.google.com/architecture/best-practices-for-operating-containers): you cannot change the code of a container that is already running. If you have a containerized application and want to make changes, you need to build a new image that includes the change, then recreate the container to start from the updated image.

[Container images](https://phoenixnap.com/kb/docker-image-vs-container) use [Union Filesystems](https://en.wikipedia.org/wiki/UnionFS). In Linux, docker originally use AUFS but they use OverlayFS now.  The details of union filesystem use in docker container images can be found at https://martinheinz.dev/blog/44.

## Borg

Google  infrastructure is containerized, using a cluster management system called [Borg](https://research.google.com/pubs/pub43438.html?hl=es) and [Omega](https://queue.acm.org/detail.cfm?id=2898444).

## Container runtimes

The container runtime is the software that is responsible for running containers.

[Kubernetes](https://github.com/bobbae/gcp/wiki/Kubernetes-Engine-and-Containers) supports several container runtimes: Docker, [containerd](https://containerd.io/), [CRI-O](https://cri-o.io), and any implementation of the Kubernetes CRI (Container Runtime Interface).

## Containers vs. VMs

[Virtual machines](VM) and containers differ in several ways, but the primary difference is that containers provide a way to virtualize an OS so that multiple workloads can run on a single OS instance. With VMs, the hardware is being virtualized to run multiple OS instances. Containers’ speed, agility, and portability make them another tool to help streamline software development.




https://www.weave.works/blog/a-practical-guide-to-choosing-between-docker-containers-and-vms

### Comparison of containerizing vs using VMs

[https://www.youtube.com/watch?v=TvnZTi_gaNc](https://www.youtube.com/watch?v=TvnZTi_gaNc)


## Different ways to run containers in GCP



[https://www.youtube.com/watch?v=jh0fPT-AWwM](https://www.youtube.com/watch?v=jh0fPT-AWwM)
