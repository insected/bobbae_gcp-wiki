

[BigQuery ML](https://cloud.google.com/bigquery-ml/docs/) enables users to create and execute machine learning models in [BigQuery](BigQuery) by using SQL queries.

https://towardsdatascience.com/explaining-a-bigquery-ml-model-5cf8d9636ec9

## BigQuery ML Algorithms supported

### Linear regression

To forecast numerical values with a linear model

### Binary logistic regression

For classification use cases when the choice is between only two different options (Yes or No, 1 or 0, True or False)

### Multiclass logistic regression

For classification scenarios when the choice is between multiple options

### Matrix factorization

For developing recommendation engines based on past information


### Time series

To forecast business KPIs leveraging timeseries data from the past



### Boosted tree

For classification and regression use cases with XGBoost

### AutoML table

To leverage AutoML capabilities from the BigQuery SQL interface

### Deep Neural Network (DNN)

For developing TensorFlow models for classification or regression scenarios, avoiding any lines of code


##  BigQuery ML  Tutorials

https://cloud.google.com/bigquery-ml/docs/tutorials

### Using AutoML Tables with BigQuery ML

[AutoML](AutoML) Tables let you build and deploy machine learning models using structured data and explain prediction results.
It can be used along with BigQuery ML. This makes it easy to train Tables models on BigQuery data using SQL from BigQuery UI and evaluate and use the models for prediction directly via SQL.

https://amygdala.github.io/gcp_blog/ml/automl/bigquery/2020/07/14/bqml_tables.html

To train an AutoML Tables model inside of BigQuery, use the BigQuery ML CREATE MODEL statement with one of the AutoML Tables model types.

https://cloud.google.com/bigquery-ml/docs/reference/standard-sql/bigqueryml-syntax-create-automl


### Unsupervised anomaly detection for time series and non-time series data

https://cloud.google.com/blog/products/data-analytics/bigquery-ml-unsupervised-anomaly-detection
