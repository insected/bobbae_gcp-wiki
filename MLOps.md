# MLOps

Machine learning (ML) workflows include steps to prepare and analyze data, train and evaluate models, deploy trained models to production, track ML artifacts and understand their dependencies, etc. Managing these steps in an ad-hoc manner can be difficult and time-consuming.

MLOps is the practice of applying DevOps practices to help automate, manage, and audit ML workflows. AI Platform Pipelines helps you implement MLOps by providing a platform where you can orchestrate the steps in your workflow as a pipeline. ML pipelines are portable and reproducible definitions of ML workflows.

https://cloud.google.com/solutions/machine-learning/setting-up-an-mlops-environment


## AI  Platform  Pipelines 

https://cloud.google.com/ai-platform/pipelines/docs


## ML CICD

Automating continuous integration (CI), continuous delivery (CD), and continuous training (CT) for machine learning (ML) systems.

https://cloud.google.com/solutions/machine-learning/mlops-continuous-delivery-and-automation-pipelines-in-machine-learning

## TFX

TFX is an open source project that you can use to define your ML workflow as a pipeline. Currently, TFX components can only train TensorFlow based models. TFX provides components that you can use to ingest and transform data, train and evaluate a model, deploy a trained model for inference, etc. By using the TFX SDK, you can compose a pipeline for your ML process from TFX components.

https://cloud.google.com/ai-platform/pipelines/docs/create-pipeline

## DataOps vs MLOps

* DataOps is an automated, process-oriented methodology, used by analytic and data teams, to improve the quality and reduce the cycle time of data analytics.

* MLOps is a practice for collaboration and communication between data scientists and operations professionals to help manage the production of ML lifecycle. MLOps looks to increase automation and improve the quality of production ML while also focusing on business and regulatory requirements.

## DevOps vs MLOps

DevOps  is the combination of cultural philosophies, practices, and tools that increases an organization's ability to deliver applications and services at high velocity: evolving and improving products at a faster pace than organizations using traditional software development and infrastructure management processes.

https://github.com/bobbae/gcp/wiki/DevOps

Comparison with MLOps:

https://towardsdatascience.com/mlops-with-a-feature-store-816cfa5966e9

## GitOps

GitOps is a way of implementing Continuous Deployment for cloud native applications. It focuses on a developer-centric experience when operating infrastructure, by using tools developers are already familiar with, including Git and Continuous Deployment tools.

The core idea of GitOps is having a Git repository that always contains declarative descriptions of the infrastructure currently desired in the production environment and an automated process to make the production environment match the described state in the repository. If you want to deploy a new application or update an existing one, you only need to update the repository - the automated process handles everything else. It’s like having cruise control for managing your applications in production.

https://www.gitops.tech/