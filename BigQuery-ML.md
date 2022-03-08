

[BigQuery ML](https://cloud.google.com/bigquery-ml/docs/) enables users to create and execute machine learning models in [BigQuery](BigQuery) by using SQL queries.



https://towardsdatascience.com/creating-a-machine-learning-model-with-sql-81d843a5307c


## BigQuery ML Algorithms supported

### Linear regression

https://cloud.google.com/bigquery-ml/docs/linear-regression-tutorial

To forecast numerical values with a linear model

https://machinelearningmastery.com/linear-regression-for-machine-learning/


### Binary logistic regression

https://cloud.google.com/bigquery-ml/docs/logistic-regression-prediction

For classification use cases when the choice is between only two different options (Yes or No, 1 or 0, True or False)

https://towardsdatascience.com/implementing-binary-logistic-regression-in-r-7d802a9d98fe

https://towardsdatascience.com/super-fast-machine-learning-to-production-with-bigquery-ml-53c43b3825a3


### K-means clustering

https://cloud.google.com/bigquery-ml/docs/kmeans-tutorial

k-means clustering is a method of vector quantization, originally from signal processing, that aims to partition n observations into k clusters in which each observation belongs to the cluster with the nearest mean (cluster centers or cluster centroid).

https://en.wikipedia.org/wiki/K-means_clustering


### Multiclass logistic regression

For classification scenarios when the choice is between multiple options

https://gluon.mxnet.io/chapter02_supervised-learning/softmax-regression-scratch.html

### Matrix factorization

https://cloud.google.com/bigquery-ml/docs/bigqueryml-mf-explicit-tutorial


For developing recommendation engines based on past information

https://developers.google.com/machine-learning/recommendation/collaborative/matrix


### Time series and ARIMA


https://en.wikipedia.org/wiki/Autoregressive_integrated_moving_average


https://cloud.google.com/bigquery-ml/docs/arima-single-time-series-forecasting-tutorial

To forecast business KPIs leveraging time series data from the past

https://otexts.com/fpp2/arima.html


### Boosted tree

https://xgboost.readthedocs.io/en/latest/tutorials/model.html


For classification and regression use cases with XGBoost


https://github.com/PacktPublishing/Machine-Learning-with-BigQuery-ML/blob/master/Chapter10/classifying_trees_xgboost.sql

### AutoML Tables

To leverage AutoML capabilities from the BigQuery SQL interface

https://cloud.google.com/automl-tables/docs


### Deep Neural Network (DNN)

For developing TensorFlow models for classification or regression scenarios, avoiding any lines of code

https://machinelearningmastery.com/what-is-deep-learning/


https://github.com/PacktPublishing/Machine-Learning-with-BigQuery-ML/blob/master/Chapter11/nyc_bike_sharing_dnn.sql

### Explainable AI and BigQuery ML

https://medium.com/codex/using-explainable-ai-in-bigquery-ml-1ec9ac0a7228


###  BigQuery ML  Tutorials

https://cloud.google.com/bigquery-ml/docs/tutorials



### Using AutoML Tables with BigQuery ML

[AutoML](AutoML) Tables let you build and deploy machine learning models using structured data and explain prediction results.
It can be used along with BigQuery ML. This makes it easy to train Tables models on BigQuery data using SQL from BigQuery UI and evaluate and use the models for prediction directly via SQL.

https://amygdala.github.io/gcp_blog/ml/automl/bigquery/2020/07/14/bqml_tables.html

To train an AutoML Tables model inside of BigQuery, use the BigQuery ML CREATE MODEL statement with one of the AutoML Tables model types.

https://cloud.google.com/bigquery-ml/docs/reference/standard-sql/bigqueryml-syntax-create-automl


### Unsupervised anomaly detection for time series and non-time series data

https://cloud.google.com/blog/products/data-analytics/bigquery-ml-unsupervised-anomaly-detection


### Explaining BigQuery ML Model

https://towardsdatascience.com/explaining-a-bigquery-ml-model-5cf8d9636ec9


### BigQuery ML Book

https://github.com/PacktPublishing/Machine-Learning-with-BigQuery-ML

### Videos

https://www.youtube.com/playlist?list=PLeLcvrwLe187Kk5QIqt7Kb8qdQSQd9AcY

### Cheatsheet

https://medium.com/fifty-five-data-science/bigquery-machine-learning-cheat-sheet-7c053b21a657


### Recommender

https://medium.com/g-company/build-a-recommender-with-bigquery-ml-15e67a457548

### BigQuery ML Models deployment with Vertex AI and Kubeflow

https://medium.com/@corba77/bigquery-ml-models-deployment-with-vertex-ai-and-kubeflow-2cff8586277f

### Predicting taxi fares

https://medium.com/@jakob.salomonsson/predicting-the-fare-on-a-billion-taxi-trips-with-bigquery-108135c8697d

## Qwiklabs


### Applying BQML's Classification, Regression, and Demand Forecasting for Retail Applications

https://google.qwiklabs.com/quests/162


### Predict Visitor Purchases with a Classification Model in BQML

GSP229

https://google.qwiklabs.com/focuses/1794?parent=catalog