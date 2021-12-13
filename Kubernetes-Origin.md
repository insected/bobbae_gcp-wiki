Similar systems that may have influenced Kubernetes designs.

### Borg

Borg is Google's main cluster management system that manages long running production services and non-production batch jobs on the same set of machines to maximize cluster utilization. 

Google's Borg system is a cluster manager that runs hundreds of thousands of jobs, from many thousands of different applications, across a number of clusters each with up to tens of thousands of machines. 

It achieves high utilization by combining admission control, efficient task-packing, over-commitment, and machine sharing with process-level performance isolation. It supports high-availability applications with runtime features that minimize fault-recovery time, and scheduling policies that reduce the probability of correlated failures. Borg simplifies life for its users by offering a declarative job specification language, name service integration, real-time job monitoring, and tools to analyze and simulate system behavior.

[https://research.google/pubs/pub43438/](https://research.google/pubs/pub43438/)

### Omega

Omega is a Google's cluster management system based on shared state. Omega is a clean-slate rewrite of Borg using more principled architecture. In Omega, all system state lives in a consistent Paxos-based storage system that is accessed by a multitude of components which act as peers. A new parallel scheduler architecture is built around shared state, using lock-free optimistic concurrency and performance scalability.   Compared to monolithic schedulers or Two-level schedulers like Mesos and Hadoop-on-demand, the Omega addresses the entire cluster state in a scheduler.

https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/41684.pdf

Kubernetes is the latest open-source container manager that draws on lessons from both previous systems.   





https://mwhittaker.github.io/papers/html/burns2016borg.html

All three systems use containers for security and performance isolation. [Container](Containers) technology has evolved greatly since the inception of Borg from chroot to jails to cgroups. 

https://research.google/pubs/pub44843/

### Twine / Tupperware

Facebook's own hyperscale orchestration tool.

https://engineering.fb.com/2019/06/06/data-center-engineering/twine/

### Swarm
Docker Swarm is Docker’s native Container Orchestration Engine. 

https://github.com/docker/classicswarm

### Mesos

Mesos takes more of a distributed approach to managing datacenter and cloud resources. Mesos can have multiple masters which use Zookeeper to keep track of the cluster state amongst the masters and form a high-availability cluster.

http://mesos.apache.org/