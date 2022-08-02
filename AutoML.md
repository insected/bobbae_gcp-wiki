[AutoML](https://en.wikipedia.org/wiki/Automated_machine_learning) is a general term describing automated AI driven methods to enhance [ML](Machine-Learning) application and processes.  AutoML is also name used by multiple projects and companies in different contexts and cloud based services.

Google Cloud [AutoML](https://cloud.google.com/automl)  helps you  build   custom machine learning models with limited machine learning expertise needed.

https://cloud.google.com/automl



## AI Platform with AutoML

[AI Platform](https://cloud.google.com/ai-platform/docs/technical-overview) brings AutoML and AI Platform (Classic) together into a unified API, client library, and user interface.  

https://cloud.google.com/vertex-ai/docs

## AutoML Vision

Derive insights from your images in the cloud or at the edge with [AutoML Vision](https://cloud.google.com/vision/automl/docs) or use pre-trained Vision API models to detect emotion, understand text, and more.


https://cloud.google.com/vision/automl/docs

[AutoML Vision](https://cloud.google.com/vision/automl/docs) enables you to train machine learning models to classify your images according to your own defined labels.

[AutoML Vision Edge](https://firebase.google.com/docs/ml/automl-image-labeling) allows you to export your custom trained models.

https://cloud.google.com/vision/automl/docs#videos

## AutoML Video intelligence

[Video Intelligence](  https://cloud.google.com/video-intelligence/automl/docs ) includes several options that you can use to integrate machine learning video intelligence models into your applications.



## AutoML Natural Language

[AutoML Natural Language](https://cloud.google.com/natural-language/automl/docs) enables you to build and deploy custom machine learning models that analyze documents, categorizing them, identify entities within them, or assessing attitudes within them. 



## AutoML Translation

[AutoML Translation](https://cloud.google.com/translate/automl/docs)  lets you to create your own translation models so that translation queries return results specific to your domain.


[Cloud Translation - Advanced](https://cloud.google.com/translate/docs/intro-to-v3) is part of the [Cloud Translation service](https://cloud.google.com/translate) that provides support for glossaries, batch requests, and AutoML models.


## AutoML Tables

[AutoML Tables](https://cloud.google.com/automl-tables/docs) helps to  build and deploy  machine learning models on structured data at speed and scale.

AutoML Tables help you create clean, effective training data by providing information about missing data, correlation, cardinality, and distribution for each of your features. 

### How-to guides

https://cloud.google.com/automl-tables/docs/how-to

### AutoML Tables Beginner's Guide

https://cloud.google.com/automl-tables/docs/beginners-guide


#### AutoML Tables samples

https://cloud.google.com/automl-tables/docs/samples


### AutoML Tables Quickstart

https://cloud.google.com/automl-tables/docs/quickstart


### AutoML Feature Engineering

When you kick off training, AutoML Tables automatically [performs common feature engineering](  https://cloud.google.com/automl-tables/docs/data-best-practices#tables-does  ) tasks for you, including:

- [Normalize and bucketize](  https://developers.google.com/machine-learning/data-prep/transform/bucketing ) numeric features.
- Create [one-hot encoding](https://en.m.wikipedia.org/wiki/One-hot) and embeddings for categorical features.
- Perform basic processing for text features.
- Extract date- and time-related features from Timestamp columns.

#### Data Prepping

https://developers.google.com/machine-learning/data-prep

### Model training

When you kick off training for your model, [AutoML Tables](https://cloud.google.com/automl-tables/docs) takes your dataset and starts training for multiple model architectures at the same time. This approach enables AutoML Tables to determine the best model architecture for your data quickly, without having to serially iterate over the many possible model architectures.  

### Using AutoML Tables from BigQuery

You can use [AutoML Tables](https://cloud.google.com/automl-tables/docs) directly from [BigQuery](BigQuery) SQL.

https://towardsdatascience.com/the-best-of-both-worlds-calling-auto-ml-from-bigquery-9dfd433a45d6

#### Choosing between AutoML Tables and BigQueryML


You might want to use [BigQuery ML](BigQuery-ML) if you are more focused on rapid experimentation or iteration with what data to include in the model and want to use simpler model types for this purpose, such as logistic regression.

You might want to work directly in the AutoML Tables interface if you have already finalized the data, and you are optimizing for maximizing model quality.


### Transparency and Logging

You can view the structure of your AutoML Tables model using [Cloud Logging](Logging). 


### Using Cloud Logging to view AutoML Tables model

Using [Cloud Logging](Logging), you can see the final model hyperparameters as well as the hyperparameters and object values used during model training and tuning.

AutoML Tables model logs have, among other fields:

- automl_tables as the value of the log_type field
- jsonPayload that contains the specific details of the log entry
- timestamp that describes when the model was created

#### Payload contents

The contents of a log entry are provided in JSON object format and are stored in the jsonPayload field.

- modelStructure
- trainingObjectivePoint	

### List of Hyperparameters

The [hyperparameter](https://cloud.google.com/ai-platform/training/docs/hyperparameter-tuning-overview) data provided in the logs differ for each type of model. 

https://cloud.google.com/automl-tables/docs/logging#hps

### Working with long-running operations


When you make an API call that takes a long time to complete, the initial call returns right away, even though the operation is still running. 

[AutoML Tables sends project owners an email](https://cloud.google.com/automl-tables/docs/long-operations) when long-running operations are complete.

### Explainability

https://cloud.google.com/automl-tables/docs/features#ai-explanations

#### Test data export

https://cloud.google.com/automl-tables/docs/features#export

### When to use AutoML vs others

Use [BigQuery ML](bigquery-ml) for easy, low-cost machine learning and quick viable ML problem using BQML, use Auto ML for code-free, state-of-the-art models. 

https://towardsdatascience.com/choosing-between-tensorflow-keras-bigquery-ml-and-automl-natural-language-for-text-classification-6b1c9fc21013


### Measuring and Improving Speech-to-Text Accuracy

https://medium.com/@nishitkamdar/measuring-and-improving-speech-to-text-accuracy-google-cloud-platform-eba62c50b8ac

## Pycaret

https://towardsdatascience.com/build-pycaret-deploy-gcp-521415a6c330


## Examples
### Classify images of clouds using AutoML
https://www.cloudskillsboost.google/focuses/8406?parent=catalog


### AutoML Tables notebooks

https://cloud.google.com/automl-tables/docs/notebooks

### Music recommendations

https://github.com/GoogleCloudPlatform/ai-platform-samples/blob/master/notebooks/samples/tables/music_recommendation/music_recommendation.ipynb

### Handwritten recipes using AutoML and Vision API 

https://cloud.google.com/blog/products/ai-machine-learning/chefkoch-digitizes-handwritten-recipes-with-automl-and-vision-api

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