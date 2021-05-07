




<img src="https://cloudx-bricks-prod-bucket.storage.googleapis.com/70eb42ad287e1b01bdc5edbbe73ce52ab972d14bcced1359c6172dbdb8627d31.svg" width="800">



[App Engine](https://cloud.google.com/appengine)  is a fully managed, serverless platform for developing and hosting web applications at scale. You can choose from several popular languages, libraries, and frameworks to develop your apps, then let App Engine take care of provisioning servers and scaling your app instances based on demand.



[Google App Engine](https://www.youtube.com/watch?v=Xuf3J6SKVV0&list=PLIivdWyY5sqIQ4_5PwyyXZVdsXr3wYhip&index=4&t=1s) makes it easy to focus on your code, not infrastructure.



## App Engine's environments

The [Standard Environment](https://cloud.google.com/appengine/docs/about-the-standard-environment) and the [Flexible environment](https://cloud.google.com/appengine/docs/flexible/) , support a host of programming languages, including Java, Python, PHP, Node.js, Go, etc.. The two environments give users maximum flexibility in how their application behaves since each environment has certain strengths. Read [The App Engine Environments](https://cloud.google.com/appengine/docs/the-appengine-environments) for more information.

[https://cloud.google.com/appengine/docs/standard/python3](https://cloud.google.com/appengine/docs/standard/python3)

[App Engine](https://www.youtube.com/watch?v=2PRciDpqpko) allows developers to focus on doing what they do best, writing code. The App Engine standard environment is based on container instances running on Google's infrastructure. Containers are preconfigured with one of several available runtimes (Java 8, Python 3.7, Go and PHP). Each runtime also includes libraries that support [App Engine Standard APIs](https://cloud.google.com/appengine/docs/about-the-standard-environment#index_of_features).  

## Locations

https://cloud.google.com/about/locations#region

## Comparison to other PaaS

* Compare to AWS Elastic Beanstalk 
https://medium.com/@at_ishikawa/comparisons-for-elastic-beanstalk-app-engine-and-heroku-2129d9c827bc


## AppEngine Standard

The App Engine standard environment makes it easy to build and deploy an application that runs reliably even under heavy load and with large amounts of data. It includes the following features:



*   Persistent storage with queries, sorting, and transactions.
*   Automatic scaling and load balancing.
*   Asynchronous task queues for performing work outside the scope of a request.
*   Scheduled tasks for triggering events at specified times or regular intervals.
*   Integration with other [Google cloud services and APIs](https://cloud.google.com/products/).

Applications run in a secure, sandboxed environment, allowing the App Engine standard environment to distribute requests across multiple servers, and scaling servers to meet traffic demands. Your application runs within its own secure, reliable environment that is independent of the hardware, operating system, or physical location of the server.



## Language Support


### Go

[https://cloud.google.com/appengine/docs/go](https://cloud.google.com/appengine/docs/go)

Here are some useful URL pointers regarding Go.

[https://github.com/avelino/awesome-go](https://github.com/avelino/awesome-go)

A Go language tutorial video.

[https://www.youtube.com/watch?v=YS4e4q9oBaU&list=PLk_epN-7EGrjdhjn5gCMJ1aLIhRTHDJcu&index=11&t=0s](https://www.youtube.com/watch?v=YS4e4q9oBaU&list=PLk_epN-7EGrjdhjn5gCMJ1aLIhRTHDJcu&index=11&t=0s)


### Python

[https://cloud.google.com/appengine/docs/python](https://cloud.google.com/appengine/docs/python)

A Python tutorial video.

[https://www.youtube.com/watch?v=rfscVS0vtbw](https://www.youtube.com/watch?v=rfscVS0vtbw)


### Node.js

A video tutorial on how to create a web application using node.js and express framework.

[https://www.youtube.com/watch?v=G8uL0lFFoN0](https://www.youtube.com/watch?v=G8uL0lFFoN0)


## App Engine Flexible

Based on [Google Compute Engine](https://cloud.google.com/compute), the App Engine flexible environment automatically scales your app up and down while also balancing the load. In the standard environment, your application runs on a lightweight instance inside of a sandbox. This sandbox restricts what your application can do. For example, the sandbox only allows your app to use a limited set of binary libraries, and your app cannot write to disk. The standard environment also limits the CPU and memory options available to your application. Because of these restrictions, most App Engine standard applications tend to be stateless web applications that respond to HTTP requests quickly.

In contrast, the flexible environment runs your application in Docker containers on [Google Compute Engine virtual machines (VMs)](https://cloud.google.com/compute/docs/instances), which have fewer restrictions. For example, you can use any programming language of your choice, write to disk, use any library you'd like, and even run multiple processes. The flexible environment also allows you to choose any Compute Engine machine type for your instances so that your application has access to more memory and CPU.

[https://cloud.google.com/appengine/docs/flexible/go/flexible-for-standard-users](https://cloud.google.com/appengine/docs/flexible/go/flexible-for-standard-users)


## Qwiklabs


[App Engine: Qwik Start - Python](https://www.qwiklabs.com/focuses/1014?catalog_rank=%7B%22rank%22%3A19%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&parent=catalog&search_id=7467964)

[App Engine: Qwik Start - Go](https://www.qwiklabs.com/focuses/2754?catalog_rank=%7B%22rank%22%3A14%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&parent=catalog&search_id=7467964)

[App Engine: Qwik Start - Java](https://www.qwiklabs.com/focuses/951?parent=catalog)


[Baseline: Deploy & Develop](https://www.qwiklabs.com/quests/37?catalog_rank=%7B%22rank%22%3A4%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&search_id=7467936)


[Deploying Applications](https://www.qwiklabs.com/quests/26?catalog_rank=%7B%22rank%22%3A3%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&search_id=7467936)


[Deploying a Python Flask Web Application to App Engine Flexible](https://www.qwiklabs.com/focuses/3339?catalog_rank=%7B%22rank%22%3A24%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&parent=catalog&search_id=7467972)


[Deploy Node.js Express Application in App Engine](https://www.qwiklabs.com/focuses/3340?catalog_rank=%7B%22rank%22%3A21%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&parent=catalog&search_id=7467972)