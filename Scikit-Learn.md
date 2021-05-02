# Introduction

Scikit-learn provides a range of supervised and unsupervised learning algorithms via a consistent interface.

It is built on Numpy, Scipy, and Matplotlib libraries.


https://scikit-learn.org/stable/


# Videos

[https://www.youtube.com/watch?v=rvVkVsG49uU](https://www.youtube.com/watch?v=rvVkVsG49uU)

[https://www.youtube.com/watch?v=MaKLWy5zXe8](https://www.youtube.com/watch?v=MaKLWy5zXe8)


# Pre-Processing



https://scikit-learn.org/stable/modules/preprocessing.html#preprocessing



## StandardScaler

Sklearn provides several built-in machine learning models, called estimators, with these estimators Standardization of datasets is a common requirement. For instance, if all the individual features do not more or less look like a standard normally distributed data the model may not perform as expected. To overcome this scikit-learn offers StandardScaler.

## Scling to a range

Sk-learn provides another option, to scale down a feature to a particular minimum and maximum value using MinMaxScaler.

## Normalizer

Each sample with at least one non zero component is rescaled independently of other samples so that its norm equals one i.e scaling real-valued metric attributes into the range 0 and 1.

## Encoding categorical data

Many a times data is not in the continuous numerical form, such data is said to be categorical for instance, [‘Good’,’Bad’], [‘Male’,’Female’] such features can be encoded as numeric value for instance, [1,0],[1,0].

To convert categorical data into numerical one can use something known as one-hot or dumming, OneHotEncoder transforms each categorical feature with n_categories possible values into n_categories binary features, with one of them being 1, and all others 0.

# Splitting up Training and Testing data

Once data pre-processing is done, we’ll move ahead to splitting the training and testing data for our model. With Sklearn the data randomly splits up into Training and Testing sets as per the given size.

# Classification

## Phases

The classification has two phases, a learning phase, and the evaluation phase. In the learning phase, the classifier trains its model on a given dataset and in the evaluation phase, it tests the classifier performance. Performance is evaluated on the basis of various parameters such as accuracy, error, precision, and recall.

[https://www.datacamp.com/community/tutorials/naive-bayes-scikit-learn](https://www.datacamp.com/community/tutorials/naive-bayes-scikit-learn)

##  SVM Classification

Identifying which category an object belongs to.

https://scikit-learn.org/stable/modules/svm.html#svm-classification

# Regression

Predicting a continuous-valued attribute associated with an object.

https://scikit-learn.org/stable/modules/svm.html#svm-regression

## Linear Regression

Linear regression attempts to model the relationship between two variables by fitting a linear equation to observed data. It basically performs the task to predict a dependent variable value (y) based on a given independent variable (x). So, this regression technique finds out a linear relationship between x (input) and y(output). 

https://towardsdatascience.com/how-does-linear-regression-actually-work-3297021970dd

## Logistic Regression

Logistic regression measures the relationship between the categorical dependent variable and one or more independent variables by estimating probabilities.

https://towardsdatascience.com/an-introduction-to-logistic-regression-8136ad65da2e

## SVM

Support vector machines (SVMs) are a set of supervised learning methods used for classification, regression. With this algorithm, we plot each data item as a point in n-dimensional space with the value of each feature being the value of a particular coordinate. Then, we perform classification by finding the hyper-plane that differentiates the two classes. Follow this blog for an in-depth understanding of SVM.


https://towardsdatascience.com/https-medium-com-pupalerushikesh-svm-f4b42800e989

## Decision Trees (DTs)

Decision Trees (DTs) are supervised learning methods used for classification and regression. The goal is to create a model that predicts the value of a target variable by learning simple decision rules inferred from the data features.

https://towardsdatascience.com/decision-trees-in-machine-learning-641b9c4e8052

## Random Forest

Random forests are an ensemble learning method for classification, regression and other, tasks that operate by constructing a multitude of decision trees at training time and outputting the class that is the mode of the classes (classification) or mean prediction (regression) of the individual trees.

https://towardsdatascience.com/random-forest-3a55c3aca46d



# Clustering

Cluster analysis of unlabeled data can be performed with the module sklearn.cluster.

Each clustering algorithm comes in two variants: a class, that implements the fit method to learn the clusters on train data, and a function, that, given train data, returns an array of integer labels corresponding to the different clusters. For the class, the labels over the training data can be found in the labels_ attribute.

https://scikit-learn.org/stable/modules/clustering.html


## KMeans

The KMeans algorithm clusters data by trying to separate samples in n groups of equal variance, minimizing a criterion known as the inertia or within-cluster sum-of-squares (see below). This algorithm requires the number of clusters to be specified. It scales well to large number of samples and has been used across a large range of application areas in many different fields.

https://scikit-learn.org/stable/modules/clustering.html#k-means


## Affinity Propagation

AffinityPropagation creates clusters by sending messages between pairs of samples until convergence. A dataset is then described using a small number of exemplars, which are identified as those most representative of other samples. The messages sent between pairs represent the suitability for one sample to be the exemplar of the other, which is updated in response to the values from other pairs. This updating happens iteratively until convergence, at which point the final exemplars are chosen, and hence the final clustering is given.


https://scikit-learn.org/stable/modules/clustering.html#affinity-propagation