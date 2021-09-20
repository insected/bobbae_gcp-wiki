

Google Cloud’s [serverless platform](https://www.youtube.com/watch?v=PBw9vD_BO5A) lets you write code your way without worrying about the underlying infrastructure. Deploy functions or apps as source code or as containers. 

Build full stack serverless applications with Google Cloud’s storage, databases, machine learning, and more. 

Easily extend applications with event-driven computing from Google or third-party service integrations. You can even choose to move your serverless workloads to on-premises environments or to the cloud.

## Choosing Serverless Option

https://medium.com/gdgeurope/choosing-server-less-option-on-gcp-510e49fdb40a


## Cloud Run

[Cloud Run](Cloud-Run) is a managed compute platform that enables you to run stateless containers that can be invoked via web requests or Pub/Sub events. 



## App Engine

[App Engine](App-Engine) is a fully managed, serverless platform for developing and hosting web applications at scale. You can choose from several popular languages, libraries, and frameworks to develop your apps, then let App Engine take care of provisioning servers and scaling your app instances based on demand.




[https://www.youtube.com/watch?v=2PRciDpqpko](https://www.youtube.com/watch?v=2PRciDpqpko)


## Cloud Functions

[Google Cloud Functions](Cloud-Functions) is a [lightweight compute solution](https://www.youtube.com/watch?v=vM-2O-uKBNQ) for developers to create single-purpose, stand-alone functions that respond to Cloud events without the need to manage a server or runtime environment.


## Knative

[Knative](https://knative.dev/) extends [Kubernetes](Kubernetes-Engine-and-Containers) to provide a set of middleware components that are essential to build modern, source-centric, and container-based applications that can run anywhere: on premises, in the cloud, or even in a third-party data center. Each of the components under the Knative project attempt to identify common patterns and codify the best practices that are shared by successful, real-world, Kubernetes-based frameworks and applications. Knative components focus on solving mundane but difficult tasks such as:



*   [Deploying a container](https://knative.dev/docs/serving/getting-started-knative-app)
*   [Routing and managing traffic with blue/green deployment](https://knative.dev/docs/serving/samples/blue-green-deployment)
*   [Scaling automatically and sizing workloads based on demand](https://knative.dev/docs/serving/autoscaling)
*   [Binding running services to eventing ecosystems](https://knative.dev/docs/eventing/getting-started)

Developers on Knative can use familiar idioms, languages, and frameworks to deploy functions, applications, or containers workloads.

Knative consists of the Serving and Eventing components:



*   [Eventing](https://knative.dev/docs/eventing) - Management and delivery of events
*   [Serving](https://knative.dev/docs/serving) - Request-driven compute that can scale to zero



Run managed serverless containers with Knative.

[https://www.youtube.com/watch?v=wPLjUF1hFCw](https://www.youtube.com/watch?v=wPLjUF1hFCw)

Knative installation is done on top of Kubernetes and uses optional extensions such as [Ambassador](https://www.getambassador.io/), [Contour](https://projectcontour.io/), [Kong](https://konghq.com/kong/) and [Gloo](https://docs.solo.io/gloo-edge/latest/).

### Knative based Cloud Run

[https://cloud.google.com/blog/products/serverless/knative-based-cloud-run-services-are-ga](https://cloud.google.com/blog/products/serverless/knative-based-cloud-run-services-are-ga)

Cloud Run is the service name fully compliant with Knative and it exists in 2 flavors: Managed and on GKE.

https://medium.com/google-cloud/knative-and-cloud-run-portability-in-action-1a655c914318

#### Quickstart

https://cloud.google.com/anthos/run/docs/quickstarts/prebuilt-deploy-gke

## Cloud Workflows and serverless tasks

You can use [Cloud Workflows](Workflows) to create serverless workflows that link a series of serverless tasks together in an order you define. Combine the power of Google Cloud's APIs, serverless products like Cloud Functions and Cloud Run, and calls to external APIs to create flexible serverless applications. Workflows require no infrastructure management and scales seamlessly with demand, including scaling down to zero.



Build serverless workflows orchestrating various products and API calls within Google Cloud and beyond. 

[https://www.youtube.com/watch?v=Uz8G8fTwwXs](https://www.youtube.com/watch?v=Uz8G8fTwwXs)


## Serverless Tensorflow Predictions at Scale

Cloud Machine Learning Engine Prediction Service can serve TensorFlow models and scale.

[https://www.youtube.com/watch?v=_JCMN8-yhBM](https://www.youtube.com/watch?v=_JCMN8-yhBM)


## CloudRun Continous Deployment and Domain Mapping

https://faun.pub/cloudrun-continous-deployment-and-domain-mapping-f83c703b88b1


## Qwiklabs



[Deploy Your Website on Cloud Run](https://www.qwiklabs.com/focuses/10445?parent=catalog)



[Websites and Web Applications](https://www.qwiklabs.com/quests/39?catalog_rank=%7B%22rank%22%3A5%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&search_id=7467936)



[Monitoring and Logging for Cloud Functions](https://www.qwiklabs.com/focuses/1833?catalog_rank=%7B%22rank%22%3A16%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&parent=catalog&search_id=7468061)



[Logging, Monitoring and Observability in Google Cloud](https://www.qwiklabs.com/courses/1514?catalog_rank=%7B%22rank%22%3A17%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&search_id=7468061)



[Responding to Stackdriver Messages with Cloud Functions](https://www.qwiklabs.com/focuses/8500?catalog_rank=%7B%22rank%22%3A22%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&parent=catalog&search_id=7468090)
