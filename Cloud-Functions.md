
[Google Cloud Functions](https://cloud.google.com/functions/docs/concepts/overview) is a [lightweight compute solution](https://www.youtube.com/watch?v=vM-2O-uKBNQ) for developers to create single-purpose, stand-alone functions that respond to Cloud events without the need to manage a server or runtime environment.


https://cloud.google.com/functions/docs/quickstart

### Cloud Functions vs Cloud Run

https://towardsdatascience.com/understand-and-compare-cloud-functions-vs-cloud-run-5afc2beb2fb

https://medium.com/google-cloud/why-i-definitively-switched-from-cloud-functions-to-cloud-run-635d03f1eb4d

### Cloud Functions second generation

https://cloud.google.com/functions/docs/2nd-gen/getting-started

https://cloud.google.com/blog/products/serverless/introducing-the-next-generation-of-cloud-functions

https://medium.com/geekculture/2nd-generation-google-cloud-function-a069a131e313

https://cloud.google.com/blog/products/serverless/cloud-functions-2nd-generation-now-generally-available

### Execution environment

https://cloud.google.com/functions/docs/concepts/exec

#### Stateless

https://cloud.google.com/functions/docs/concepts/exec#stateless_functions

### Minimum instances


You can avoid cold starts for your application and reduce application latency by setting a minimum number of instances.

https://cloud.google.com/run/docs/configuring/min-instances

### Using maximum instances

You can control the scaling behavior of your function by setting a maximum number of Cloud Functions instances.

https://cloud.google.com/functions/docs/configuring/max-instances

### Region Performances

https://medium.com/google-cloud/cloud-run-and-cloud-functions-does-the-region-change-the-performances-b967e5cee0cc

### Functions Framework

https://github.com/GoogleCloudPlatform/functions-framework-python

### Cloud Functions for .NET

[https://cloud.google.com/blog/products/application-development/introducing-net-google-cloud-functions](https://cloud.google.com/blog/products/application-development/introducing-net-google-cloud-functions)

### Anti patterns


#### Idempotency

https://cloud.google.com/blog/topics/developers-practitioners/avoiding-gcf-anti-patterns-part-1-how-write-event-driven-cloud-functions-properly-coding-idempotency-mind

#### Reuse

https://cloud.google.com/blog/topics/developers-practitioners/avoiding-gcf-anti-patterns-part-2-how-reuse-cloud-function-instances-future-invocations

### Cloud Functions URL permission error and IAM

https://lukestoolkit.blogspot.com/2020/06/google-cloud-functions-error-forbidden.html


## Tutorial

https://medium.com/geekculture/google-cloud-functions-a-brief-tutorial-de07d8945b01


### Event driven applications using Cloud Functions

https://medium.com/brainjar/how-to-build-an-event-driven-application-on-google-cloud-using-cloud-functions-64fa241b556e


### Deploying Cloud Functions on a Chromebook

https://medium.com/google-cloud/who-said-you-cant-code-on-a-chromebook-local-development-with-cloud-functions-4e68dca1240b

### API Gateway with Cloud Functions

https://medium.com/@sdptd20/exploring-google-cloud-api-gateway-with-google-cloud-functions-ff56c1c96cc9

### Monitoring High usage BigQuery jobs

https://engineering.premise.com/tutorial-detection-of-high-usage-bigquery-jobs-on-google-cloud-platform-gcp-aadb591eefe5


### OCR tutorial with Cloud Functions

https://cloud.google.com/functions/docs/tutorials/ocr

### Going beyond Cloud Functions limits using BigQuery

https://medium.com/google-cloud/google-cloud-function-beyond-the-limits-ea1f16c577b

### Working around the 9 minute limit of Cloud Functions


https://medium.com/@hayovanloon/working-around-the-9-minute-limit-of-google-cloud-functions-78ff19bd869c

### Using Cloud Functions to implement a Slack Slash command

https://cloud.google.com/functions/docs/tutorials/slack

### Blurring images using ImageMagick 

https://cloud.google.com/functions/docs/tutorials/imagemagick

### Cloud Functions caching with node-cache

https://medium.com/@kangthecreator/google-cloud-functions-caching-with-node-cache-6647c76c9adc

### OAuth2 authentication for Cloud Functions

https://dev.to/rampi/oauth2-authentication-for-a-google-cloud-functions-56g

###

### Serverless performance monitoring

https://cloud.google.com/architecture/serverless-web-performance-monitoring-using-cloud-functions

### Streaming data from Cloud storage to BigQuery

https://cloud.google.com/architecture/streaming-data-from-cloud-storage-into-bigquery-using-cloud-functions

### Connecting to Cloud Memorystore Redis instance

https://cloud.google.com/memorystore/docs/redis/connect-redis-instance-functions

### Testing Cloud Functions using Cloud Build and Terraform

https://cloud.google.com/architecture/system-testing-cloud-functions-using-cloud-build-and-terraform

### Handling Promises

https://cloud.google.com/blog/topics/developers-practitioners/avoiding-gcf-anti-patterns-part-4-how-handle-promises-correctly-your-nodejs-cloud-function

### Static outbound IP for Cloud Functions using Terraform

https://shashwotrisal.medium.com/how-to-create-a-static-outbound-ip-for-google-cloud-functions-using-terraform-a8e9b30074b6