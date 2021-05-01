
## Serverless 


### Introduction

Google Cloud’s serverless platform lets you write code your way without worrying about the underlying infrastructure. Deploy functions or apps as source code or as containers. Build full stack serverless applications with Google Cloud’s storage, databases, machine learning, and more. Easily extend applications with event-driven computing from Google or third-party service integrations. You can even choose to move your serverless workloads to on-premises environments or to the cloud.

[https://www.youtube.com/watch?v=PBw9vD_BO5A](https://www.youtube.com/watch?v=PBw9vD_BO5A)


### Cloud Run

Cloud Run is a managed compute platform that enables you to run stateless containers that can be invoked via web requests or Pub/Sub events. 

[http://cloud.run](http://cloud.run/)

Cloud Run is serverless: it abstracts away all infrastructure management, so you can focus on what matters most — building great applications. It is built from [Knative](https://cloud.google.com/knative/), letting you choose to run your containers either fully managed with Cloud Run, in your Google Kubernetes Engine cluster, or in workloads on-premises with Cloud Run for Anthos.

[https://cloud.google.com/run/docs](https://cloud.google.com/run/docs)


#### Quickstart: Build and Deploy

This interactive tutorial can be opened in Cloud Shell editor (theia) and followed step by step.

[https://cloud.google.com/run/docs/quickstarts/build-and-deploy](https://cloud.google.com/run/docs/quickstarts/build-and-deploy)


#### Use Cases

[https://cloud.google.com/run/#section-6](https://cloud.google.com/run/#section-6)

Learn how to deploy serverless containers in 3 environments using Cloud Run and Knative.

[https://www.youtube.com/watch?v=nhwYc4StHIc](https://www.youtube.com/watch?v=nhwYc4StHIc)

A video on migrating kubernetes apps to serverless with Cloud Run on Anthos.

[https://www.youtube.com/watch?v=0T5UliS9j8A](https://www.youtube.com/watch?v=0T5UliS9j8A)


### App Engine

App Engine is a fully managed, serverless platform for developing and hosting web applications at scale. You can choose from several popular languages, libraries, and frameworks to develop your apps, then let App Engine take care of provisioning servers and scaling your app instances based on demand.

[https://cloud.google.com/appengine/docs](https://cloud.google.com/appengine/docs)

Google App Engine makes it easy to focus on your code, while letting us manage your infrastructure.

[https://www.youtube.com/watch?v=2PRciDpqpko](https://www.youtube.com/watch?v=2PRciDpqpko)


### Cloud Functions

[Google Cloud Functions](https://cloud.google.com/functions/docs/concepts/overview) is a lightweight compute solution for developers to create single-purpose, stand-alone functions that respond to Cloud events without the need to manage a server or runtime environment.

[https://cloud.google.com/functions/docs](https://cloud.google.com/functions/docs)

A video tutorial of Cloud Functions that  will show you how to deploy a Cloud Function from a Google Cloud project.  You will learn how to test your function and see your log entries. 

[https://www.youtube.com/watch?v=vM-2O-uKBNQ](https://www.youtube.com/watch?v=vM-2O-uKBNQ)


#### Cloud Functions for .NET

[https://cloud.google.com/blog/products/application-development/introducing-net-google-cloud-functions](https://cloud.google.com/blog/products/application-development/introducing-net-google-cloud-functions)


### Knative

Knative (pronounced kay-nay-tiv) extends [Kubernetes](https://kubernetes.io/docs/concepts/overview/what-is-kubernetes/) to provide a set of middleware components that are essential to build modern, source-centric, and container-based applications that can run anywhere: on premises, in the cloud, or even in a third-party data center. Each of the components under the Knative project attempt to identify common patterns and codify the best practices that are shared by successful, real-world, Kubernetes-based frameworks and applications. Knative components focus on solving mundane but difficult tasks such as:



*   [Deploying a container](https://knative.dev/docs/serving/getting-started-knative-app)
*   [Routing and managing traffic with blue/green deployment](https://knative.dev/docs/serving/samples/blue-green-deployment)
*   [Scaling automatically and sizing workloads based on demand](https://knative.dev/docs/serving/autoscaling)
*   [Binding running services to eventing ecosystems](https://knative.dev/docs/eventing/getting-started)

Developers on Knative can use familiar idioms, languages, and frameworks to deploy functions, applications, or containers workloads.

Knative consists of the Serving and Eventing components:



*   [Eventing](https://knative.dev/docs/eventing) - Management and delivery of events
*   [Serving](https://knative.dev/docs/serving) - Request-driven compute that can scale to zero

[https://knative.dev/](https://knative.dev/)

Run managed serverless containers with Knative.

[https://www.youtube.com/watch?v=wPLjUF1hFCw](https://www.youtube.com/watch?v=wPLjUF1hFCw)

Knative installation is done on top of Kubernetes and uses optional extensions such as [Ambassador](https://www.getambassador.io/), [Contour](https://projectcontour.io/), [Kong](https://konghq.com/kong/) and [Gloo](https://docs.solo.io/gloo-edge/latest/).

#### Cloud Run

[https://cloud.google.com/blog/products/serverless/knative-based-cloud-run-services-are-ga](https://cloud.google.com/blog/products/serverless/knative-based-cloud-run-services-are-ga)


### Workflows

You can use Workflows to create serverless workflows that link a series of serverless tasks together in an order you define. Combine the power of Google Cloud's APIs, serverless products like Cloud Functions and Cloud Run, and calls to external APIs to create flexible serverless applications. Workflows require no infrastructure management and scales seamlessly with demand, including scaling down to zero.

[https://cloud.google.com/workflows/docs](https://cloud.google.com/workflows/docs)

Build serverless workflows orchestrating various products and API calls within Google Cloud and beyond. 

[https://www.youtube.com/watch?v=Uz8G8fTwwXs](https://www.youtube.com/watch?v=Uz8G8fTwwXs)


### Serverless Predictions at Scale

Cloud Machine Learning Engine Prediction Service can serve TensorFlow models and scale.

[https://www.youtube.com/watch?v=_JCMN8-yhBM](https://www.youtube.com/watch?v=_JCMN8-yhBM)


### Qwiklabs


#### Deploy on Cloud Run

This is a Qwiklab to show you how to deploy a website using Cloud Run.

[Deploy Your Website on Cloud Run](https://www.qwiklabs.com/focuses/10445?parent=catalog)


#### Web Applications on Cloud Run

It is a part of the larger “Quest”.

[Websites and Web Applications](https://www.qwiklabs.com/quests/39?catalog_rank=%7B%22rank%22%3A5%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&search_id=7467936)


#### Monitoring Cloud Functions

You can [view your Cloud Functions](https://cloud.google.com/functions) with their execution times,execution counts, and memory usage in the Cloud Console using [Cloud Monitoring](https://cloud.google.com/monitoring), where you can set up custom alerting on these metrics.

[Monitoring and Logging for Cloud Functions](https://www.qwiklabs.com/focuses/1833?catalog_rank=%7B%22rank%22%3A16%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&parent=catalog&search_id=7468061)


#### Logging in Google Cloud

Learn how to monitor, troubleshoot, and improve your infrastructure and application performance. Guided by the principles of Site Reliability Engineering (SRE), this course features a combination of lectures, demos, hands-on labs, and real-world case studies. In this course, you'll gain experience with full-stack monitoring, real-time log management and analysis, debugging code in production, and profiling CPU and memory usage.

[Logging, Monitoring and Observability in Google Cloud](https://www.qwiklabs.com/courses/1514?catalog_rank=%7B%22rank%22%3A17%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&search_id=7468061)


#### Stackdriver Cloud Functions

In this lab you will learn how to use Cloud Functions to perform lightweight processing of Stackdriver Logging messages.

[Responding to Stackdriver Messages with Cloud Functions](https://www.qwiklabs.com/focuses/8500?catalog_rank=%7B%22rank%22%3A22%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&parent=catalog&search_id=7468090)
