[AutoML](https://en.wikipedia.org/wiki/Automated_machine_learning) is a general term describing automated AI driven methods to enhance [ML](Machine-Learning) application and processes.  AutoML is also name used by multiple projects and companies in different contexts and cloud based services.

Google Cloud [AutoML](https://cloud.google.com/automl)  helps you easily build high quality custom machine learning models with limited machine learning expertise needed.

https://cloud.google.com/automl


## AI Platform with AutoML

[AI Platform](https://cloud.google.com/ai-platform/docs/technical-overview)brings AutoML and AI Platform (Classic) together into a unified API, client library, and user interface. With AI Platform, both AutoML training and custom training are available options. 

https://cloud.google.com/vertex-ai/docs

## AutoML Vision

Derive insights from your images in the cloud or at the edge with [AutoML Vision](https://cloud.google.com/vision/automl/docs) or use pre-trained Vision API models to detect emotion, understand text, and more.


https://cloud.google.com/vision/automl/docs

[AutoML Vision](https://cloud.google.com/vision/automl/docs) enables you to train machine learning models to classify your images according to your own defined labels.

- Train models from labeled images and evaluate their performance.
- Leverage a human labeling service for datasets with unlabeled images.
- Register trained models for serving through the AutoML API.

[AutoML Vision Edge](https://firebase.google.com/docs/ml/automl-image-labeling) now allows you to export your custom trained models.

- AutoML Vision Edge allows you to train and deploy low-latency, high accuracy models optimized for edge devices.
- With Tensorflow Lite, Core ML, and container export formats, AutoML Vision Edge supports a variety of devices.
- Hardware architectures supported: Edge TPUs, ARM and NVIDIA.
- To build an application on iOS or Android devices you can use AutoML Vision Edge in ML Kit. This solution is available via Firebase and offers an end-to-end development flow for creating and deploying custom models to mobile devices using ML Kit client libraries.

https://cloud.google.com/vision/automl/docs#videos

## AutoML Video intelligence

Video Intelligence includes several options that you can use to integrate machine learning video intelligence models into your applications and web sites. For example, video classification and object tracking.

https://cloud.google.com/video-intelligence/automl/docs

## AutoML Natural Language

[AutoML Natural Language](https://cloud.google.com/vision/automl/docs) enables you to build and deploy custom machine learning models that analyze documents, categorizing them, identify entities within them, or assessing attitudes within them. Learn more about the AutoML Natural Language features and capabilities.

https://cloud.google.com/natural-language/automl/docs

## AutoML Translation

[AutoML Translation](https://cloud.google.com/translate/automl/docs)  lets you to create your own, custom translation models so that translation queries return results specific to your domain.

https://cloud.google.com/translate/automl/docs

[Cloud Translation - Advanced](https://cloud.google.com/translate/docs/intro-to-v3) is part of the [Cloud Translation service](https://cloud.google.com/translate) that provides support for glossaries, batch requests, and AutoML models.


## AutoML Tables

[AutoML Tables](https://cloud.google.com/automl-tables/docs) helps to  build and deploy  machine learning models on structured data at speed and scale.

AutoML Tables helps you create clean, effective training data by providing information about missing data, correlation, cardinality, and distribution for each of your features. And because there's no charge for importing your data and viewing information about it, you don't incur charges from AutoML Tables until you start training your model.

https://cloud.google.com/automl-tables/docs




### AutoML Tables Beginner's Guide

https://cloud.google.com/automl-tables/docs/beginners-guide

https://cloud.google.com/automl-tables/docs/samples


### AutoML Tables Quickstart

https://cloud.google.com/automl-tables/docs/quickstart


### AutoML Feature Engineering

When you kick off training, AutoML Tables automatically performs common feature engineering tasks for you, including:

- Normalize and bucketize numeric features.
- Create one-hot encoding and embeddings for categorical features.
- Perform basic processing for text features.
- Extract date- and time-related features from Timestamp columns.

There is a list of common requirements for training data that AutoML Tables automatically does for you. You do not need to include these calculations in your training data. In fact, if you perform these transformations yourself and include them in your training data, you might decrease the quality of the resulting model.

https://cloud.google.com/automl-tables/docs/data-best-practices#tables-does

### Model training

When you kick off training for your model, [AutoML Tables](https://cloud.google.com/automl-tables/docs) takes your dataset and starts training for multiple model architectures at the same time. This approach enables AutoML Tables to determine the best model architecture for your data quickly, without having to serially iterate over the many possible model architectures.  Using your training and validation sets, AutoML determine the best model architecture for your data. 

### Using AutoML Tables from BigQuery

You can use [AutoML Tables](https://cloud.google.com/automl-tables/docs) directly from [BigQuery](BigQuery) SQL.

https://towardsdatascience.com/the-best-of-both-worlds-calling-auto-ml-from-bigquery-9dfd433a45d6

#### Choosing between AutoML Tables and BigQueryML


You might want to use [BigQuery ML](BigQuery-ML) if you are more focused on rapid experimentation or iteration with what data to include in the model and want to use simpler model types for this purpose (such as logistic regression).

You might want to work directly in the AutoML Tables interface if you have already finalized the data, and you:

- Are optimizing for maximizing model quality (accuracy, low RMSE, and so on) without needing to manually do feature engineering, model selection, ensembling, and so on.

- Are willing to wait longer to attain that model quality. AutoML Tables takes at least an hour to train a model, because it experiments with many modeling options. BigQuery ML potentially returns models in minutes because it sticks with the model architectures and parameter values and ranges you set.

- Have a wide variety of feature inputs (beyond numbers and classes) that would benefit from the additional automated feature engineering that AutoML Tables provides.

### Transparency and Logging

You can view the structure of your AutoML Tables model using [Cloud Logging](Logging). In Logging, you can see the final model hyperparameters as well as the hyperparameters and objective values used during model validation.





### Using Cloud Logging to view AutoML Tables model

Using [Cloud Logging](Logging), you can see the final model hyperparameters as well as the hyperparameters and object values used during model training and tuning.

Activity logs are structured as described in the LogEntry type documentation.


https://cloud.google.com/automl-tables/docs/logging

AutoML Tables model logs have, among other fields:

- automl_tables as the value of the log_type field
- jsonPayload that contains the specific details of the log entry
- timestamp that describes when the model was created

#### Payload contents

The contents of a log entry are provided in JSON object format and are stored in the jsonPayload field.

- modelStructure
- trainingObjectivePoint	

### List of Hyperparameters

The [hyperparameter](https://cloud.google.com/ai-platform/training/docs/hyperparameter-tuning-overview) data provided in the logs differ for each type of model. The following sections describe the hyperparameters for each model type.

https://cloud.google.com/automl-tables/docs/logging#hps

### Working with long-running operations


When you make an API call that takes a long time to complete, the initial call returns right away, even though the operation is still running. There are some helper methods you can use to determine the status of a long-running operation.

[AutoML Tables sends project owners an email](https://cloud.google.com/automl-tables/docs/long-operations) when long-running operations are complete.



https://cloud.google.com/automl-tables/docs/long-operations

### Explainability

https://cloud.google.com/automl-tables/docs/features#ai-explanations

#### Test data export

https://cloud.google.com/automl-tables/docs/features#export


### AutoML Tables example

Music recommendations

https://github.com/GoogleCloudPlatform/ai-platform-samples/blob/master/notebooks/samples/tables/music_recommendation/music_recommendation.ipynb

### When to use AutoML vs others

Use [BigQuery ML](bigquery-ml) for easy, low-cost machine learning and quick experimentation to see if ML is viable on your data. Sometimes, the accuracy you get with BQML is sufficient, and you will simply stop here.

Once you identify a viable ML problem using BQML, use Auto ML for code-free, state-of-the-art models. Text classification, for example, is a very specialized field with high-dimensional inputs. So, you can do better with a customized solution (i.e., Auto ML Natural Language) than with a structured data approach that just uses bag-of-words.

Hand-roll your own custom models only for problems where you have lots of data and enough time/effort to devote. Use AutoML as a benchmark. If, you can not beat Auto ML after some reasonable effort, stop wasting time. Just go with Auto ML.

https://towardsdatascience.com/choosing-between-tensorflow-keras-bigquery-ml-and-automl-natural-language-for-text-classification-6b1c9fc21013


## Links
- [AutoML Cloud Natural language Classification Tutorial](https://cloud.google.com/natural-language/automl/docs/tutorial#python)
- [AutoML Cloud Natural Language Samples](https://cloud.google.com/natural-language/automl/docs/samples)
- [AutoML Tables Quickstart](https://cloud.google.com/automl-tables/docs/quickstart)
- [AutoML Tables notebooks](https://cloud.google.com/automl-tables/docs/notebooks)
- [AutoML Cloud Translation API tutorial](https://cloud.google.com/translate/automl/docs/tutorial)
- [AutoML Cloud Video Intelligence API Quickstarts](https://cloud.google.com/video-intelligence/automl/docs/quickstart)
- [AutoML Vision](https://cloud.google.com/vision/automl/docs)
- [Cloud Vision API](https://cloud.google.com/vision/docs)
- [Cloud Natural language](https://cloud.google.com/natural-language/docs)
- [Cloud Translation](https://cloud.google.com/translate/docs)
- [Cloud Text-to-Speech](https://cloud.google.com/text-to-speech/docs)
- [Cloud Speech-to-Text](https://cloud.google.com/speech-to-text/docs)
- [Dialogflow](https://cloud.google.com/dialogflow/docs)
- [Cloud Inference API](https://cloud.google.com/inference/docs)