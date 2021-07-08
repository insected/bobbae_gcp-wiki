

Machine learning (ML) [workflows](Workflows) include steps to prepare and analyze data, train and evaluate models, deploy trained models to production, track ML artifacts and understand their dependencies, etc. Managing these steps in an ad-hoc manner can be difficult and time-consuming.

[MLOps](https://cloud.google.com/solutions/machine-learning/setting-up-an-mlops-environment) is the practice of applying DevOps practices to help automate, manage, and audit ML workflows. AI Platform Pipelines helps you implement MLOps by providing a platform where you can orchestrate the steps in your workflow as a pipeline. ML pipelines are portable and reproducible definitions of ML workflows.  [Kubeflow](Kubeflow) is a kind of MLOps tool.



## AI  Platform  Pipelines 

[AI Platform Pipelines](https://cloud.google.com/ai-platform/pipelines/docs) makes it easier to get started with MLOps by saving you the difficulty of setting up Kubeflow Pipelines with TensorFlow Extended (TFX). Kubeflow Pipelines is an open source platform for running, monitoring, auditing, and managing ML pipelines on Kubernetes. TFX is an open source project for building ML pipelines that orchestrate end-to-end ML workflows.





## Kubeflow

[Kubeflow](Kubeflow) is the ML toolkit for Kubernetes.

Using the Kubeflow configuration interfaces you can specify the ML tools required for your workflow. Then you can deploy the workflow to various clouds.


## MLflow

[MLflow](https://mlflow.org/) is a MLOps platform that was born from learning the standards of Big Tech with the focus on creating transferable knowledge, ease of use, modularity and compatibility with popular ML libraries and frameworks. It was designed for a 1 or 1000+ person organisation. 


## Neptune

[Neptune](https://neptune.ai/) is a metadata store for MLOps, built for research and production teams that run a lot of experiments. 

It gives you a central place to log, store, display, organize, compare, and query all metadata generated during the machine learning lifecycle

https://neptune.ai/blog/mlflow-vs-kubeflow-vs-neptune-differences


## Pachyderm

[Pachyderm](https://www.pachyderm.com/) is a data science platform that combines Data Lineage with End-to-End Pipelines on Kubernetes, engineered for the enterprise.  [Other similar tools](https://neptune.ai/blog/the-best-pachyderm-alternatives) also exist to control an end-to-end machine learning life cycle.

## DVC

[DVC](https://dvc.org/) is built to make ML models shareable and reproducible. It is designed to handle large files, data sets, machine learning models, and metrics as well as code.

## MLRun

[MLRun](https://github.com/mlrun/mlrun) is an open-source MLOps framework that offers an integrative approach to managing your machine-learning pipelines from early development through model development to full pipeline deployment in production. MLRun offers a convenient abstraction layer to a wide variety of technology stacks while empowering data engineers and data scientists to define the feature and models.


## Vertex Pipelines

https://cloud.google.com/vertex-ai/docs/pipelines/introduction


## ML CICD

[Automating](https://cloud.google.com/solutions/machine-learning/mlops-continuous-delivery-and-automation-pipelines-in-machine-learning) continuous integration (CI), continuous delivery (CD), and continuous training (CT) for machine learning (ML) systems.



## TFX

[TFX](https://www.tensorflow.org/tfx) is an open source project that you can use to define your ML workflow as a pipeline. Currently, TFX components can only train TensorFlow based models. TFX provides components that you can use to ingest and transform data, train and evaluate a model, deploy a trained model for inference, etc. By using the TFX SDK, you can compose a pipeline for your ML process from TFX components.


