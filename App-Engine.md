
[App Engine](https://cloud.google.com/appengine)  is a fully managed, serverless [PaaS](PaaS) for developing and hosting web applications at scale. You can choose from several popular languages, libraries, and frameworks to develop your apps, then let [App Engine](https://en.wikipedia.org/wiki/Google_App_Engine) take care of provisioning servers and scaling your app instances based on demand.


## App Engine's environments

The [Standard Environment](https://cloud.google.com/appengine/docs/about-the-standard-environment) and the [Flexible environment](https://cloud.google.com/appengine/docs/flexible/)  support a host of programming languages, including Java, Python, PHP, Node.js, Go, etc. 





## App Engine Standard

[App Engine](https://www.youtube.com/watch?v=2PRciDpqpko) standard environment is based on container instances running on Google's infrastructure. Containers are preconfigured with one of several available runtimes (Java 8, Python 3.7, Go and PHP). Each runtime also includes libraries that support [App Engine Standard APIs](https://cloud.google.com/appengine/docs/about-the-standard-environment#index_of_features).  





### Language Support


#### Go

[https://cloud.google.com/appengine/docs/go](https://cloud.google.com/appengine/docs/go)

Here are some useful URL pointers regarding Go.

[https://github.com/avelino/awesome-go](https://github.com/avelino/awesome-go)

A Go language tutorial video.

[https://www.youtube.com/watch?v=YS4e4q9oBaU&list=PLk_epN-7EGrjdhjn5gCMJ1aLIhRTHDJcu&index=11&t=0s](https://www.youtube.com/watch?v=YS4e4q9oBaU&list=PLk_epN-7EGrjdhjn5gCMJ1aLIhRTHDJcu&index=11&t=0s)


#### Python

[https://cloud.google.com/appengine/docs/python](https://cloud.google.com/appengine/docs/python)

A Python tutorial video.

[https://www.youtube.com/watch?v=rfscVS0vtbw](https://www.youtube.com/watch?v=rfscVS0vtbw)


#### Node.js

https://cloud.google.com/appengine/docs/nodejs

A video tutorial on how to create a web application using node.js and express framework.

[https://www.youtube.com/watch?v=G8uL0lFFoN0](https://www.youtube.com/watch?v=G8uL0lFFoN0)


#### Languages updates

https://cloud.google.com/blog/topics/developers-practitioners/new-java-ruby-python-php-runtimes

## App Engine Flexible

Based on [Google Compute Engine](https://cloud.google.com/compute), the [App Engine flexible](https://cloud.google.com/appengine/docs/flexible/) environment automatically scales your app up and down while also balancing the load. Because of sandbox restrictions, most App Engine standard applications tend to be stateless web applications that respond to HTTP requests quickly.

In contrast, the flexible environment runs your application in Docker containers on [Google Compute Engine virtual machines (VMs)](https://cloud.google.com/compute/docs/instances), which have fewer restrictions. For example, you can use any programming language of your choice, write to disk, use any library you'd like, and even run multiple processes. The flexible environment also allows you to choose any Compute Engine machine type for your instances so that your application has access to more memory and CPU.

[https://cloud.google.com/appengine/docs/flexible/go/flexible-for-standard-users](https://cloud.google.com/appengine/docs/flexible/go/flexible-for-standard-users)


## Choosing an App Engine environment

https://cloud.google.com/appengine/docs/the-appengine-environments

## App Engine and GKE

### Running App Engine Apps on GKE


https://cloud.google.com/appengine/docs/flexible/python/run-flex-app-on-kubernetes

### Moving from App Engine to GKE

https://ipinfo.io/blog/app-engine-to-google-kubernetes-engine/



### App Engine Auto scaling

https://levelup.gitconnected.com/understanding-and-optimization-of-google-app-engines-automatic-scaling-95674910da3b


## Other PaaS

https://github.com/bobbae/gcp/wiki/PaaS#paas-alternatives

- https://github.com/mitja/awesome-paas

- Compare to AWS Elastic Beanstalk 
https://medium.com/@at_ishikawa/comparisons-for-elastic-beanstalk-app-engine-and-heroku-2129d9c827bc

- https://foghornconsulting.com/2017/05/12/battle-of-the-paas-aws-vs-gcp/


## Examples

https://cloud.google.com/appengine/docs/standard/python/samples

https://github.com/GoogleCloudPlatform/golang-samples/tree/main/appengine_flexible

### First steps

https://medium.com/@david.alvares.62/your-first-steps-with-app-engine-63c7eefbe609

### App Engine and Cloud SQL based registration app

https://medium.com/@christcallista16/getting-started-with-gcp-building-a-registration-application-using-app-engine-and-cloud-sql-8f8731ce5d4b

## Tutorials

https://cloud.google.com/appengine/docs/standard/python/tutorials


https://cloud.google.com/go/getting-started

https://cloud.google.com/go/getting-started/authenticate-users-with-iap

https://www.qwiklabs.com/focuses/2754?parent=catalog


## Qwiklabs


[App Engine: Qwik Start - Python](https://www.qwiklabs.com/focuses/1014?catalog_rank=%7B%22rank%22%3A19%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&parent=catalog&search_id=7467964)

[App Engine: Qwik Start - Go](https://www.qwiklabs.com/focuses/2754?catalog_rank=%7B%22rank%22%3A14%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&parent=catalog&search_id=7467964)

[App Engine: Qwik Start - Java](https://www.qwiklabs.com/focuses/951?parent=catalog)


[Baseline: Deploy & Develop](https://www.qwiklabs.com/quests/37?catalog_rank=%7B%22rank%22%3A4%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&search_id=7467936)


[Deploying Applications](https://www.qwiklabs.com/quests/26?catalog_rank=%7B%22rank%22%3A3%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&search_id=7467936)


[Deploying a Python Flask Web Application to App Engine Flexible](https://www.qwiklabs.com/focuses/3339?catalog_rank=%7B%22rank%22%3A24%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&parent=catalog&search_id=7467972)


[Deploy Node.js Express Application in App Engine](https://www.qwiklabs.com/focuses/3340?catalog_rank=%7B%22rank%22%3A21%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&parent=catalog&search_id=7467972)
