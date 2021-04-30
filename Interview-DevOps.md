https://www.edureka.co/blog/interview-questions/top-devops-interview-questions-2016/


## jenkins

https://www.guru99.com/jenkins-interview-questions.html

## jenkins , teamcity, bamboo, tavis, circle-ci, codeship 

https://www.altexsoft.com/blog/engineering/comparison-of-most-popular-continuous-integration-tools-jenkins-teamcity-bamboo-travis-ci-and-more/

## building docker images

https://www.taniarascia.com/continuous-integration-pipeline-docker/

Explain what each line does in the following dockerfile

```
# Pull from a base image
FROM node:12-alpine

# Copy the files from the current directory to app/
COPY . app/

# Use app/ as the working directory
WORKDIR app/

# Install dependencies (npm ci is similar to npm i, but for automated builds)
RUN npm ci --only-production

# Build production client side React application
RUN npm run build

# Listen on the specified port
EXPOSE 5000

# Set Node server
ENTRYPOINT npm run start
```
