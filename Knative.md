Kubernetes-based platform to deploy and manage modern [serverless](Serverless) workloads.

https://knative.dev/docs/

## Quickstart


https://cloud.google.com/anthos/run/docs/quickstarts/prebuilt-deploy-gke

## Features


[Knative](https://knative.dev/) extends [Kubernetes](Kubernetes-Engine-and-Containers) to provide a set of middleware components that are essential to build modern, source-centric, and container-based applications that can run anywhere: on premises, in the cloud, or even in a third-party data center. Each of the components under the Knative project attempt to identify common patterns and codify the best practices that are shared by successful, real-world, Kubernetes-based frameworks and applications. Knative components focus on solving mundane but difficult tasks such as:

*   [Deploying a container](https://knative.dev/docs/serving/getting-started-knative-app)
*   [Routing and managing traffic with blue/green deployment](https://knative.dev/docs/serving/samples/blue-green-deployment)
*   [Scaling automatically and sizing workloads based on demand](https://knative.dev/docs/serving/autoscaling)
*   [Binding running services to eventing ecosystems](https://knative.dev/docs/eventing/getting-started)

Developers on Knative can use familiar idioms, languages, and frameworks to deploy functions, applications, or containers workloads.

## Serving and Eventing

Knative consists of the Serving and Eventing components:


*   [Eventing](https://knative.dev/docs/eventing) - Management and delivery of events
*   [Serving](https://knative.dev/docs/serving) - Request-driven compute that can scale to zero



## Run managed serverless containers with Knative

[https://www.youtube.com/watch?v=wPLjUF1hFCw](https://www.youtube.com/watch?v=wPLjUF1hFCw)

## Knative installation

Knative installation is done on top of Kubernetes and uses optional extensions such as [Ambassador](https://www.getambassador.io/), [Contour](https://projectcontour.io/), [Kong](https://konghq.com/kong/) and [Gloo](https://docs.solo.io/gloo-edge/latest/).

## Knative based Cloud Run

[https://cloud.google.com/blog/products/serverless/knative-based-cloud-run-services-are-ga](https://cloud.google.com/blog/products/serverless/knative-based-cloud-run-services-are-ga)

Cloud Run is the service name fully compliant with Knative and it exists in 2 flavors: Managed and on GKE.

https://medium.com/google-cloud/knative-and-cloud-run-portability-in-action-1a655c914318


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
 
## Knative and Cloud Run portability

https://medium.com/google-cloud/knative-and-cloud-run-portability-in-action-1a655c914318

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



