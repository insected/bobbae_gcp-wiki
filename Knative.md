Kubernetes-based platform to deploy and manage modern serverless workloads.

https://knative.dev/docs/


Knative components build on top of Kubernetes, abstracting away the complex details and enabling developers to focus on what matters. 

Knative offers features like scale-to-zero, autoscaling, in-cluster builds, and eventing framework for cloud-native applications on Kubernetes.

Built by codifying the best practices shared by successful real-world implementations, Knative solves the "boring but difficult" parts of deploying and managing cloud native services so you don't have to.


## Components



### Build

- Configurable and flexible approach to building source code into containers

- Pluggable approach leveraging Dockerfiles or built templates

- No cross-compiling or need for local build tools

- Support for cached artifacts for faster builds

- Allow your organization to utilize spare capacity for better resource usage

### Serving

- Higher level abstraction, easy to reason about the object model

- Seamless autoscaling based on HTTP requests

- Gradual rollouts for new revisions

- Integrates networking and service mesh automatically

- Pluggable: connect your own logging and monitoring platform

### Eventing

- Universal subscription, delivery, and management of events

- Build loosely coupled, event-driven systems with high-level objects

- Declarative binding between event producers and event consuming services

- Scalable from just a few events to live streams

- Custom event pipelines to connect with your own existing systems
 
## Samples

### Getting Started
https://knative.dev/docs/serving/getting-started-knative-app/

### Blue Green
https://knative.dev/docs/serving/samples/blue-green-deployment/

### Auto Scale

https://knative.dev/docs/serving/autoscaling/

### Eventing

https://knative.dev/docs/eventing/getting-started/

### Code Samples

https://knative.dev/docs/samples/