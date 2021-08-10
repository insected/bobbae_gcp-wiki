[Machine learning](https://en.wikipedia.org/wiki/Machine_learning) (ML) is the study of computer algorithms that improve automatically through experience and by the use of data.

[Machine learning](https://developers.google.com/machine-learning/glossary) is an [awesome](https://github.com/ujjwalkarn/Machine-Learning-Tutorials)  application of [artificial intelligence](AI) (AI) that provides systems the ability to automatically learn and improve from experience without being explicitly programmed. 

[Machine learning](https://github.com/josephmisiti/awesome-machine-learning/blob/master/books.md)  focuses on the development of computer programs that can access data and use it to learn for themselves.

What is [Machine Learning](https://www.mygreatlearning.com/blog/machine-learning-tutorial/)?

[https://www.youtube.com/watch?v=HcqpanDadyQ](https://www.youtube.com/watch?v=HcqpanDadyQ)

Google Machine Learning Platform Overview.

[https://www.youtube.com/watch?v=QR_LQQ-vvko](https://www.youtube.com/watch?v=QR_LQQ-vvko)

<img src="https://miro.medium.com/max/1575/1*i5HvoYNEBohHxS1MoQoQcQ.png" width="700">

## Machine Learning Crash Course

First read this [comicbook](https://cloud.google.com/products/ai/ml-comic-1).


Then head over to this [tutorial](https://developers.google.com/machine-learning/crash-course/).

And look at these videos: https://www.youtube.com/playlist?list=PLblh5JKOoLUICTaGLRoHQDuF_7q2GfuJF

Then read

http://ema.cri-info.cm/wp-content/uploads/2019/07/2019BurkovTheHundred-pageMachineLearning.pdf

and

https://duchesnay.github.io/pystatsml/index.html

## Machine Learning & Artificial Intelligence 



A Data Scientist models and analyzes key data and continually improves the way the business utilizes data. Data Scientists aim to make accurate predictions about the future using in-depth data modeling and deep learning.

https://cloud.google.com/training/machinelearning-ai

## Machine learning Workflows

[AI Platform](AI-Platform) enables many parts of the machine learning (ML) [workflow](Workflows). This document provides an introductory description of the overall ML process and explains where each AI Platform service fits into the process.

https://cloud.google.com/ai-platform/docs/ml-solutions-overview

## 7 steps of Machine Learning

Gather data, prepare data, choose the model, train the model, evaluate, tune parameters, review prediction or inference.

https://towardsdatascience.com/the-7-steps-of-machine-learning-2877d7e5548e

Steps:

[https://www.youtube.com/watch?v=nKW8Ndu7Mjw](https://www.youtube.com/watch?v=nKW8Ndu7Mjw)

## Dataset Search engine

https://datasetsearch.research.google.com/

## Supervised vs. Unsupervised learning

A supervised machine learning algorithm (as opposed to an unsupervised machine learning algorithm) is one that relies on labeled input data to learn a function that produces an appropriate output when given new unlabeled data.

Imagine a computer is a child, we are its supervisor (e.g. parent, guardian, or teacher), and we want the child (computer) to learn what a pig looks like. We will show the child several different pictures, some of which are pigs and the rest could be pictures of anything (cats, dogs, etc).

When we see a pig, we shout “pig!” When it’s not a pig, we shout “no, not pig!” After doing this several times with the child, we show them a picture and ask “pig?” and they will correctly (most of the time) say “pig!” or “no, not pig!” depending on what the picture is. That is supervised machine learning.

https://towardsdatascience.com/supervised-vs-unsupervised-learning-14f68e32ea8d

The most common tasks within unsupervised learning are clustering, representation learning, and density estimation. In all of these cases, we wish to learn the inherent structure of our data without using explicitly-provided labels. Some common algorithms include k-means clustering, principal component analysis, and autoencoders. Since no labels are provided, there is no specific way to compare model performance in most unsupervised learning methods.

Two common use-cases for unsupervised learning are exploratory analysis and dimensionality reduction.

Unsupervised learning is very useful in exploratory analysis because it can automatically identify structure in data. For example, if an analyst were trying to segment consumers, unsupervised clustering methods would be a great starting point for their analysis. In situations where it is either impossible or impractical for a human to propose trends in the data, unsupervised learning can provide initial insights that can then be used to test individual hypotheses.

Dimensionality reduction, which refers to the methods used to represent data using less columns or features, can be accomplished through unsupervised methods. In representation learning, we wish to learn relationships between individual features, allowing us to represent our data using the latent features that interrelate our initial features. This sparse latent structure is often represented using far fewer features than we started with, so it can make further data processing much less intensive, and can eliminate redundant features.


[[https://miro.medium.com/max/1030/1*zWBYt9DQQEf_XxXWLA2tzQ.jpeg]]


## Tensorflow


Created by the Google Brain team, 
[TensorFlow](Tensorflow) is an open source library for numerical computation and large-scale machine learning.


## Tensorflow Example: Plain and Simple estimators


TensorFlow has a pretty large API surface, but the part we are going to focus on is high-level APIs, called Estimators.

https://towardsdatascience.com/plain-and-simple-estimators-d8d3f4c185c1

The Estimators API gives us a nice workflow of getting our raw data, passing it through an input function, setting up our feature columns and model structure, running our training, and running our evaluation.

[https://www.youtube.com/watch?v=G7oolm0jU8I](https://www.youtube.com/watch?v=G7oolm0jU8I)

## Feature Engineering

Feature engineering is the process of transforming raw data into features that better represent the underlying problem to the predictive models, resulting in improved model accuracy on unseen data.

https://machinelearningmastery.com/discover-feature-engineering-how-to-engineer-features-and-how-to-get-good-at-it/

### One-Hot Encoding

Some learning algorithms only work with numerical feature vectors. When some feature in your dataset is categorical, like “colors” or “days of the week,” you can transform such a categorical feature into several binary ones.

If your example has a categorical feature “colors” and this feature has three possible values: “red,” “yellow,” “green,” you can transform this feature into a vector of three numerical values. By doing so, you increase the dimensionality of your feature vectors. You should not transform red into 1, yellow into 2, and green into 3 to avoid increasing the dimensionality because that would imply that there’s an order among the values in this category and this specific order is important for the decision making. If the order of a feature’s values is not important, using ordered numbers as values is likely to confuse the learning algorithm, because the algorithm will try to find a regularity where there’s no one, which may potentially lead to overfitting.

### Binning

Binning (also called bucketing) is the process of converting a continuous feature into multiple binary features called bins or buckets, typically based on value range. For example, instead of representing age as a single real-valued feature, the analyst could chop ranges of age into discrete bins: all ages between 0 and 5 years-old could be put into one bin, 6 to 10 years-old could be in the second bin, 11 to 15 years-old could be in the third bin, and so on.

### Normalization

Normalization is the process of converting an actual range of values which a numerical
feature can take, into a standard range of values, typically in the interval [≠1, 1] or [0, 1].
For example, suppose the natural range of a particular feature is 350 to 1450. By subtracting 350 from every value of the feature, and dividing the result by 1100, one can normalize those values into the range [0, 1].




By [normalizing](https://www.jeremyjordan.me/batch-normalization/) all of our inputs to a standard scale, we're allowing the network to more quickly learn the optimal parameters for each input node.


### Standardization

Standardization (or z-score normalization) is the procedure during which the feature values are rescaled so that they have the properties of a standard normal distribution with μ = 0 and ‡ = 1, where μ is the mean (the average value of the feature, averaged over all examples in the dataset) and ‡ is the standard deviation from the mean.


### Dealing with Missing Features

In some cases, the data comes to the analyst in the form of a dataset with features already defined. In some examples, values of some features can be missing. That often happens when the dataset was handcrafted, and the person working on it forgot to fill some values or didn’t get them measured at all.


### Data Imputation Techniques

One technique consists in replacing the missing value of a feature by an average value of this
feature in the dataset.

Another technique is to replace the missing value by the same value outside the normal range of values. 

For example, if the normal range is [0, 1], then you can set the missing value equal to 2 or ≠1. The idea is that the learning algorithm will learn what is it better to do when the feature has a value significantly different from other values. Alternatively, you can replace the missing value by a value in the middle of the range. For example, if the range for a feature is [≠1, 1], you can set the missing value to be equal to 0. Here, the idea is that if we use the value in the middle of the range to replace missing features, such value will not significantly affect the prediction.



## Training Datasets

Once you have got your annotated dataset, the first thing you do is you shue the examples and split the dataset into three subsets: training, validation, and test.

The training set is usually the biggest one, and you use it to build the model. 

The validation and test sets are roughly the same sizes, much smaller than the size of the training set. The learning algorithm cannot use examples from these two subsets to build a model. That is why those two sets are often called hold-out sets.

There’s no optimal proportion to split the dataset into these three subsets. In the past, the rule of thumb was to use 70% of the dataset for training, 15% for validation and 15% for testing. However, in the age of big data, datasets often have millions of examples. In such cases, it could be reasonable to keep 95% for training and 2.5%/2.5% for validation/testing.

You may wonder, what is the reason to have three sets and not one. The answer is simple: when we build a model, what we do not want is for the model to only do well at predicting labels of examples the learning algorithms has already seen. A trivial algorithm that simply memorizes all training examples and then uses the memory to “predict” their labels will make no mistakes when asked to predict the labels of the training examples, but such an algorithm would be useless in practice. What we really want is that our model predicts well examples that the learning algorithm didn’t see. So we want good performance on a hold-out set.


## Underfitting and Overfitting

If the model makes many mistakes on the training data, we say that the model has a high bias or that the model underfits. So, underfitting is the inability of the model to predict well the labels of the data it was trained on. There could be several reasons for underfitting, the most important of which are:

- your model is too simple for the data (for example a linear model can often underfit)
- the features you engineered are not informative enough

Overfitting is another problem a model can exhibit. The model that overfits predicts very well the training data but poorly the data from at least one of the two hold-out sets. I already gave an illustration of overfitting in Chapter 3. Several reasons can lead to overfitting, the most important of which are:

- your model is too complex for the data (for example a very tall decision tree or a very deep or wide neural network often overfit)
- you have too many features but a small number of training examples


Many of the modern advancements in neural networks have been a result of stacking many hidden layers.

This deep stacking allows us to learn more complex relationships in the data. However, because we're increasing the complexity of the model, we're also more prone to [potentially overfitting](https://www.jeremyjordan.me/deep-neural-networks-preventing-overfitting/) our data. 



## Regularization

Even the simplest model, such as linear, can overfit the data. That usually happens when the data is high-dimensional, but the number of training examples is relatively low. In fact, when feature vectors are very high-dimensional, the linear learning algorithm can build a model that assigns non-zero values to most dimensions w(j) in the parameter vector w, trying to find very complex relationships between all available features to predict labels of training examples perfectly.

Such a complex model will most likely predict poorly the labels of the hold-out examples. This is because by trying to perfectly predict labels of all training examples, the model will also learn the idiosyncrasies of the training set: the noise in the values of features of the training examples, the sampling imperfection due to the small dataset size, and other artifacts extrinsic to the decision problem in hand but present in the training set.

Regularization is an umbrella-term that encompasses methods that force the learning algorithm to build a less complex model. In practice, that often leads to slightly higher bias but significantly reduces the variance. This problem is known in the literature as the bias-variance tradeoff.

The two most widely used types of regularization are called L1 regularization and L2 regularization. The idea is quite simple. To create a regularized model, we modify the objective function by adding a penalizing term whose value is higher when the model is more complex.

In practice, L1 regularization produces a sparse model, a model that has most of its parameters (in case of linear models, most of w(j)) equal to zero. So L1 makes feature selection by deciding which features are essential for prediction and which are not. That can be useful in case you want to increase model explainability. 

However, if your only goal is to maximize the performance of the model on the hold-out data, then L2 usually gives better results. L2 also has the advantage of being differentiable, so gradient descent can be used for optimizing the objective function.

L1 and L2 regularization methods are also combined in what is called elastic net regularization with L1 and L2 regularizations being special cases. You can find in the literature the name ridge regularization for L2 and lasso for L1.



## Evaluation of Models


Once you have a model built using the training set, how can you say how good the model is? You use test set to assess the model. The test set contains the examples that the learning algorithm has never seen before. If our model performs well on predicting the labels of the examples from the test set, we say that our model generalizes well.


### Accuracy

Accuracy is necessarily relevant or good way of evaluating a model. Accuracy is given by the number of correctly classified examples divided by the total number of classified examples.

Accuracy may be useful when errors in predicting all classes are equally important.  In case of spam/not spam this may not be the case. You would tolerate false positives less than false negatives.  A false positive may mean you don't get an important email.  False negative is no big deal, even though it is annoying to get a spam.

Accuracy can be not useful when all classes not not equally important. Predicting click stream can be biased because of very few real positive clicks per rendered pages. In other words, almost no clicks can be the norm. In that case, a model that is 99.999% accurate can be created by simply returning "no click" as answer every time.

Accuracy is a useful metric when errors in predicting all classes are equally important. In case of the spam/not spam, this may not be the case. For example, you would tolerate false positives less than false negatives. A false positive in spam detection is the situation in which your friend sends you an email, but the model labels it as spam and doesn’t show you. On the other hand, the false negative is less of a problem: if your model doesn’t detect a small percentage of spam messages, it’s not a big deal.

### Confusion Matrix

Confusion Matrix is a table that summarizes how successful the classification model is at predicting examples belonging to various classes.

https://en.wikipedia.org/wiki/Confusion_matrix

Confusion Matrices can be used to calculate two important performance metrics: precision and recall.

### Precision & Recall

The two most frequently used metrics to assess the model are precision and recall.  Precision is the ratio of correct positive predictions to overall number of positive predictions.   Recall is the ratio of positive predictions to the overall number of positive examples in the test set.  

https://wikipedia.org/wiki/Precision_and_recall

https://towardsdatascience.com/beyond-accuracy-precision-and-recall-3da06bea9f6c

https://developers.google.com/machine-learning/crash-course/classification/precision-and-recall

### F-measure

F-measure is the harmonic mean of Precision and Recall and gives a better measure of the incorrectly classified cases than the Accuracy Metric.

https://machinelearningmastery.com/precision-recall-and-f-measure-for-imbalanced-classification/

### ROC and AUC

Receiver Operating Characteristic curve and Area Under the Curve use a combination of the true positive rate and false positive rate to build up a summary picture of the model performance.

https://en.wikipedia.org/wiki/Receiver_operating_characteristic

## Classification

[Classification](https://machinelearningmastery.com/types-of-classification-in-machine-learning/) is a task that requires the use of machine learning algorithms that learn how to assign a class label to examples from the problem domain. An easy to understand example is classifying emails as “spam” or “not spam.”

Classification algorithms are used when you have a dataset of observations where we'd like to use the features associated with an observation to predict its class.

### Basic Bayes Theorem

[Bayes' theorem](https://www.analyticsvidhya.com/blog/2016/06/bayesian-statistics-beginners-simple-english/), named after 18th-century British mathematician Thomas Bayes, is a mathematical formula for determining conditional probability. Conditional probability is the likelihood of an outcome occurring, based on a previous outcome occurring.

[https://www.youtube.com/watch?v=HZGCoVF3YvM](https://www.youtube.com/watch?v=HZGCoVF3YvM)

We can use probability to make predictions in machine learning. Perhaps the most widely used example is called the Naive Bayes algorithm. Not only is it straightforward to understand, but it also achieves surprisingly good results on a wide range of problems.

[https://machinelearningmastery.com/naive-bayes-classifier-scratch-python/](https://machinelearningmastery.com/naive-bayes-classifier-scratch-python/)

Naive [Bayes classification](https://www.jeremyjordan.me/naive-bayes-classification/) methods are quite simple (in terms of model complexity) and commonly used for tasks such as document classification and spam filtering. This algorithm works well for datasets with a large amount of features (ex. a body of text where every word is treated as a feature) but it is naive in the sense that it treats every feature as independent of one another. This is clearly not the case for language, where word order matters when trying to discern meaning from a statement. Nonetheless, these methods have been used quite successfully for various text classification tasks.

### Regression & Classification

[Regression](https://machinelearningmastery.com/neural-network-models-for-combined-classification-and-regression/) and [classification](https://www.youtube.com/watch?v=TJveOYsK6MY) lead to ways of splitting data.

Classification is a problem of automatically assigning a label to an unlabeled example. Spam detection is a famous example of classification.

In machine learning, the classification problem is solved by a classification learning algorithm that takes a collection of labeled examples as inputs and produces a model that can take an unlabeled example as input and either directly output a label or output a number that can be used by the data analyst to deduce the label easily. An example of such a number is a probability.

In a classification problem, a label is a member of a finite set of classes. If the size of the set of classes is two (“sick”/“healthy”, “spam”/“not_spam”), we talk about binary classification (also called binomial).

Multiclass classification (also called multinomial) is a classification problem with three or more classes.

While some learning algorithms naturally allow for more than two classes, others are by nature binary classification algorithms. There are strategies allowing to turn a binary classification learning algorithm into a multiclass one. 

Regression is a problem of predicting a real-valued label (often called a target) given an unlabeled example. Estimating house price valuation based on house features, such as area, the number of bedrooms, location and so on is a famous example of regression.

The regression problem is solved by a regression learning algorithm that takes a collection of labeled examples as inputs and produces a model that can take an unlabeled example as input and output a target.


### Logistic Regression


The goal of [logistic regression](https://www.jeremyjordan.me/logistic-regression/), as with any classifier, is to figure out some way to split the data to allow for an accurate prediction of a given observation's class using the information present in the features. (For instance, if we were examining the Iris flower dataset, our classifier would figure out some method to split the data based on the following: sepal length, sepal width, petal length, petal width.) In the case of a generic two-dimensional example, the split might look something like this.

https://www.youtube.com/watch?v=yIYKR4sgzI8

### Decision Trees

[Decision trees](https://www.jeremyjordan.me/decision-trees/) are one of the oldest and most widely-used machine learning models, due to the fact that they work well with noisy or missing data, can easily be ensembled to form more robust predictors, and are incredibly fast at runtime. Moreover, you can directly visual your model's learned logic, which means that it's an incredibly popular model for domains where model interpretability is important.


### K-nearest neighbors

The [k-nearest neighbors]( https://towardsdatascience.com/machine-learning-basics-with-the-k-nearest-neighbors-algorithm-6a6e71d01761 ) (KNN) algorithm is a simple, easy-to-implement supervised machine learning algorithm that can be used to solve both classification and regression problems. 

Many machine learning techniques involve building a model that is capable of representing the data and then finding the optimal parameters for the model to minimize error. [K-nearest neighbors](https://www.jeremyjordan.me/k-nearest-neighbors/), however, is an example of instance-based learning where we instead simply store the training data and use it to make new predictions.

https://towardsdatascience.com/machine-learning-basics-with-the-k-nearest-neighbors-algorithm-6a6e71d01761


### SVM

[Support vector machines](https://www.jeremyjordan.me/support-vector-machines/) classifier works well in complicated feature domains, albeit requiring clear separation between classes. 

SVM  is a supervised machine learning model that uses classification algorithms for two-group classification problems. After giving an SVM model sets of labeled training data for each category, they're able to categorize new text.

Compared to newer algorithms like neural networks, they have two main advantages: higher speed and better performance with a limited number of samples (in the thousands). This makes the algorithm very suitable for text classification problems, where it’s common to have access to a dataset of at most a couple of thousands of tagged samples.

https://monkeylearn.com/blog/introduction-to-support-vector-machines-svm/

SVMs don't work well with noisy data, and the algorithm scales roughly cubic O(n3) to input depending on your implementation. For example, sklearn's SVM fit time complexity is more than quadratic, so it won't be able to train quickly on large datasets (>10,000 examples).

### Random forests

Decision trees are desirable in that they scale well to larger datasets, they are robust against irrelevant features, and it is very easy to visualize the rationalization between a decision tree's predictions. Further, decision trees have low bias as there is minimal implicitly defined structure in the model (as opposed to linear regression, for example, which makes the assumption of linear relationships). Unfortunately, decision trees are prone to high variance and will overfit noisy data.

[Random forests](https://www.jeremyjordan.me/random-forests/) inherit the benefits of a decision tree model whilst improving upon the performance by reducing the variance. In building a random forest, we train a collection of decision trees on random subsets of the training data. Further, on each sampling from the population, we also sample a subset of features from the overall feature space. This adds randomness (with the intent to reduce variance in the end model) to the splitting process by limiting the features available for to split on for each individual base model.

### Boosted trees

[Boosting](https://www.jeremyjordan.me/boosted-trees/) is an iterative ensembling process where models are trained in a sequential order. These models are known as "weak learners" as they are simple prediction rules which only perform slightly better than a random guess (ie. slightly better than 50% accuracy). The general concept behind boosting is to focus on the "hard" examples, or the examples that the model fails to predict correctly with confidence. These examples are given more emphasis by skewing the distribution of observations so that these examples are more likely to appear in a sample. As such, the next weak learner will focus more on getting these hard examples correct. Because your learner is always doing better than random, you'll always get some degree of information from each sequential training round. When all of the simple prediction rules are combined into one overarching model, a powerful predictor emerges.


### Content Classification

Content Classification analyzes a document and returns a list of content categories that apply to the text found in the document. 

[https://cloud.google.com/natural-language/docs/classifying-text](https://cloud.google.com/natural-language/docs/classifying-text)

Using [AutoML](AutoML) to classify text.

[https://www.youtube.com/watch?v=ieaqfU1BwJ8](https://www.youtube.com/watch?v=ieaqfU1BwJ8)


### Classification, redaction, and de-identification

The [Cloud Data Loss Prevention](https://cloud.google.com/dlp)  (DLP) helps you understand, manage, and protect sensitive data. With the Cloud DLP, you can easily classify and redact sensitive data contained in text-based content and images, including content stored in Google Cloud storage repositories.

[https://cloud.google.com/dlp/docs/classification-redaction](https://cloud.google.com/dlp/docs/classification-redaction)

## Regression

Regression algorithms are used when you have a dataset of observations where you'd like to use the features to predict a continuous output.

Example: Predict the price of a house using the following features: sq ft, number of rooms, zip code, age of house, school district.


### Linear Regression


[Linear regression](https://www.jeremyjordan.me/linear-regression/) is used to predict an outcome given some input value(s). While machine learning classifiers use features to predict a discrete label for a given instance or example, machine learning regressors have the ability use features to predict a continuous outcome for a given instance or example. For example, a classifier might draw a decision boundary that can tell you whether or not a house is likely to sell at a given price (when provided with features of the house) but a regressor can use those same features to predict the market value of the house. Nonetheless, regression is still a supervised learning technique and you'll still need to train your model on a set of examples with known outcomes.

https://www.youtube.com/watch?v=nk2CQITm_eo



### Polynomial regression

[Polynomial regression](https://www.jeremyjordan.me/polynomial-regression/) is very similar to linear regression, with a slight deviation in how we treat our feature-space.

## Clustering

Clustering is a popular technique to find groups or segments in your data that are similar. This is an unsupervised learning algorithm in the sense that you don't train the algorithm and give it examples for what you'd like it to do, you just let the clustering algorithm explore the data and provide you with new insights.


### K-means clustering 

[K-means clustering](https://www.jeremyjordan.me/grouping-data-points-with-k-means-clustering/) is a simple method for partitioning n data points in k groups, or clusters.

https://www.youtube.com/watch?v=4b5d3muPQmA



## Dimensionality Reduction

When we're building machine learning models, sometimes we deal with datasets with well over 1,000 or even 10,000 dimensions. While this allows us to account for many features, these features are often redundant. Ideally, due to the curse of dimensionality, we'd like to limit our data to capture the true signal in the data and ignore the noise. 

Dimensionality reduction is one technique to reduce the dimension of our feature-space while maintaining the maximum amount of information. 

Dimensionality reduction is also very convenient for visualizing higher-dimensional data sets in two or three dimensions. 

### Principal Components Analysis

[Principal components analysis](https://www.jeremyjordan.me/principal-components-analysis/) (PCA) is the most popular dimensionality reduction technique to date. It allows us to take an n-dimensional feature-space and reduce it to a k-dimensional feature-space while maintaining as much information from the original dataset as possible in the reduced dataset. Specifically, PCA will create a new feature-space that aims to capture as much variance as possible in the original dataset; I'll elaborate on this later in this post.

### Autoencoders

[Autoencoders](https://www.jeremyjordan.me/autoencoders/) are an unsupervised learning technique in which we leverage neural networks for the task of representation learning.

## Neural Networks

Neural networks are one of the most popular approaches to machine learning today, achieving impressive performance on a large variety of tasks. Often referred to as the "universal function approximator", this approach is very flexible to learning a variety of tasks.

### Neural Networks Representation

Neural networks are a [biologically-inspired algorithm](https://www.jeremyjordan.me/intro-to-neural-networks/) that attempt to mimic the functions of neurons in the brain. Each neuron acts as a computational unit, accepting input from the dendrites and outputting signal through the axon terminals. Actions are triggered when a specific combination of neurons are activated.

### Activation functions

[Activation functions](https://www.jeremyjordan.me/neural-networks-activation-functions/) are used to determine the firing of neurons in a neural network. Given a linear combination of inputs and weights from the previous layer, the activation function controls how we'll pass that information on to the next layer.

### Backpropagation


[Backpropagation](https://www.jeremyjordan.me/neural-networks-training/) computes the gradient of the loss function with respect to the weights of the network for a single input–output example, and does so efficiently, unlike a naive direct computation of the gradient with respect to each weight individually. This efficiency makes it feasible to use gradient methods for training multilayer networks, updating weights to minimize loss; gradient descent, or variants such as stochastic gradient descent, are commonly used.



### Gradient descent 

[Gradient descent](https://www.jeremyjordan.me/gradient-descent/) is an optimization technique commonly used in training machine learning algorithms. Often when we're building a machine learning model, we'll develop a cost function which is capable of measuring how well our model is doing. This function will penalize any error our model makes (by assigning a cost) with respect to the current parameter values. Thus, by minimizing the cost function we can find the optimal parameters that yield the best model performance.

https://www.youtube.com/watch?v=sDv4f4s2SB8

### Hyperparameter Tuning

You will probably tune hyperparameters by experimentally finding the best combination of values, one per hyperparamter.

https://en.wikipedia.org/wiki/Hyperparameter_optimization

### Learning Rate

One of the key hyperparameters to set in order to train a neural network is the [learning rate](https://www.jeremyjordan.me/nn-learning-rate/) for gradient descent. As a reminder, this parameter scales the magnitude of our weight updates in order to minimize the network's loss function.

If your learning rate is set too low, training will progress very slowly as you are making very tiny updates to the weights in your network. However, if your learning rate is set too high, it can cause undesirable divergent behavior in your loss function. 


### Convolutional Neural Networks

[CNN](https://www.jeremyjordan.me/convolutional-neural-networks/) are used heavily in image recognition applications of machine learning. Convolutional neural networks provide an advantage over feed-forward networks because they are capable of considering locality of features.

A convolutional neural network (CNN) is a special kind of FFNN that significantly reduces the number of parameters in a deep neural network with many units without losing too much in the quality of the model. CNNs have found applications in image and text processing where they beat many previously established benchmarks.

Because CNNs were invented with image processing in mind, I explain them on the image classification example.


### Recurrent Neural Networks

[Recurrent neural networks](https://www.jeremyjordan.me/introduction-to-recurrent-neural-networks/) are good  for learning from sequential data.

Recurrent neural networks (RNNs) are used to label, classify, or generate sequences. A sequence is a matrix, each row of which is a feature vector and the order of rows matters. Labeling a sequence means predicting a class to each feature vector in a sequence. Classifying a sequence means predicting a class for the entire sequence. Generating a sequence means to output another sequence (of a possibly dierent length) somehow relevant to the input sequence.

RNNs are often used in text processing because sentences and texts are naturally sequences of either words/punctuation marks or sequences of characters. For the same reason, recurrent neural networks are also used in speech processing.


## Reinforcement Learning

[Reinforcement learning](https://www.jeremyjordan.me/overview-of-reinforcement-learning/) is an approach to machine learning where agents are rewarded to accomplish some task. "Good" behavior is reinforced via a reward, so this approach can more realistically be considered a method of reward maximization. 


Reinforcement learning is a method of learning where we teach the computer to perform some task by providing it with feedback as it performs actions. This is different from supervised learning in that we don't explicitly provide correct and incorrect examples of how the task should be completed, we simply tell the computer when it is doing a good job along the way. Reinforcement learning is also distinct from unsupervised learning because we are providing the computer with some level of feedback, even if we aren't providing explicit examples.

Reinforcement learning is a subfield of machine learning where the machine “lives” in an environment and is capable of perceiving the state of that environment as a vector of features. The machine can execute actions in every state. Different actions bring different rewards and could also move the machine to another state of the environment. The goal of a reinforcement learning algorithm is to learn a policy. A policy is a function f (similar to the model in supervised learning) that takes the feature vector of a state as input and outputs an optimal action to execute in that state. The action is optimal if it maximizes the expected average reward.


### Markov Decision Process

The [Markov Decision Process](https://www.jeremyjordan.me/markov-decision-process/) is a method for planning in a stochastic environment. Whereas we cannot control or optimize the randomness that occurs, we can optimize our actions within a random environment. Planning for stochastic environments is much more difficult than planning for a deterministic environment; given the randomness present, there's a degree of uncertainty surrounding the results of our actions.


### Monte Carlo learning

The [Monte Carlo](https://www.jeremyjordan.me/rl-learning-implementations/) approach approximates the value of a state-action pair by calculating the mean return from a collection of episodes.


## Model based vs. Instance based learning

Most supervised learning algorithms are model-based, e.g. SVM. Model-based learning algorithms use the training data to create a model that has parameters learned from the training data.  After the model was built, the training data can be discarded.

Instance-based learning algorithms use the whole dataset as the model. One instance-based algorithm frequently used in practice is k-Nearest Neighbors (kNN). In classification, to predict a label for an input example the kNN algorithm looks at the close neighborhood of the input example in the space of feature vectors and outputs the label that it saw the most often in this close neighborhood.


## Shallow vs. Deep learning

A shallow learning algorithm learns the parameters of the model directly from the features of the training examples. Most supervised learning algorithms are shallow. The exceptions are neural network learning algorithms, specifically those that build neural networks with more than one layer between input and output. Such neural networks are called deep neural networks. In deep neural network learning (or, simply, deep learning), contrary to shallow learning, most model parameters are learned not directly from the features of the training examples, but from the outputs of the preceding layers.

## Characteristics of a machine learning model

https://subscription.packtpub.com/book/data/9781838820299/1/ch01lvl1sec03/characteristics-of-a-machine-learning-model

https://www.malicksarr.com/type-of-machine-learning-algorithms-the-complete-overview/

https://serokell.io/blog/machine-learning-algorithm-classification-overview

https://towardsdatascience.com/a-tour-of-machine-learning-algorithms-466b8bf75c0a


## Natural Language Processing

### TF-IDF Vectorization


[Term frequency-inverse document frequency](https://www.jeremyjordan.me/identifying-related-bodies-of-text-using-tf-idf-vectorization/) (TF-IDF) vectorization is a mouthful to say, but it's also a simple and convenient way to characterize bodies of text. Due to its simplicity, this method scales better than some other topic modeling techniques (latent dirichlet allocation, probabilistic latent semantic indexing) when dealing with large datasets.


#### Build Text Classification Model using  TF-IDF and NLTK

https://www.datacamp.com/community/tutorials/text-analytics-beginners-nltk

#### NLTK

https://www.nltk.org/book/


### BERT 

Bidirectional Encoder Representations from Transformers is described in this [paper](https://arxiv.org/pdf/1810.04805.pdf).

https://towardsdatascience.com/bert-explained-state-of-the-art-language-model-for-nlp-f8b21a9b6270

### ELMo

ELMo is a deep contextualized word representation that models both (1) complex characteristics of word use (e.g., syntax and semantics), and (2) how these uses vary across linguistic contexts (i.e., to model polysemy).


https://allennlp.org/elmo

### Transfer Learning

The process of training a model on a large-scale dataset and then using that pre-trained model to process learning for another target task. 

Transfer Learning became popular in the field of NLP thanks to the state-of-the-art performance of different algorithms like ULMFiT, Skip-Gram, Elmo, BERT etc.

https://towardsdatascience.com/transfer-learning-using-elmo-embedding-c4a7e415103c

### Attention

https://jalammar.github.io/visualizing-neural-machine-translation-mechanics-of-seq2seq-models-with-attention/



### Transformers

https://jalammar.github.io/illustrated-transformer/



### BERT and ELMo


http://jalammar.github.io/illustrated-bert/

### trends

https://www.elderresearch.com/blog/trends-in-natural-language-processing/

## GCP ML Solutions

### AutoML

[AutoML](AutoML) makes the power of machine learning available to you even if you have limited knowledge of machine learning. You can use AutoML to build on Google's machine learning capabilities to create your own custom machine learning models that are tailored to your business needs, and then integrate those models into your applications and web sites.


[https://cloud.google.com/automl/docs](https://cloud.google.com/automl/docs)



### AI Platform and Machine Learning

[AI Platform](AI-Platform) enables many parts of the machine learning (ML) workflow. 

### ML Solutions Overview 


[https://cloud.google.com/ai-platform/docs/ml-solutions-overview](https://cloud.google.com/ai-platform/docs/ml-solutions-overview)


### Choosing Machine Learning Options

Decision pyramid to choose the right ML option.

[https://www.youtube.com/watch?v=pm_-pVPvZ-4](https://www.youtube.com/watch?v=pm_-pVPvZ-4)


### CloudML Engine

[https://www.youtube.com/watch?v=m0rqccviLNM](https://www.youtube.com/watch?v=m0rqccviLNM)


### Cloud AutoML to custom model

[https://www.youtube.com/watch?v=OHIEZ-Scek8](https://www.youtube.com/watch?v=OHIEZ-Scek8)



### AutoML NL for custom text classification

[https://www.youtube.com/watch?v=ieaqfU1BwJ8](https://www.youtube.com/watch?v=ieaqfU1BwJ8)


### Custom Sentiment Analysis with AutoML Natural Language

https://www.youtube.com/watch?v=CReeC8YuEd8

### Vision AI

Cloud Vision includes several options that you can use to integrate machine learning vision models into your applications and web sites.

[https://cloud.google.com/vision/overview/docs](https://cloud.google.com/vision/overview/docs)

[https://www.youtube.com/watch?v=kgxfdTh9lz0](https://www.youtube.com/watch?v=kgxfdTh9lz0)

[https://www.youtube.com/watch?v=BN8aO0LULyw](https://www.youtube.com/watch?v=BN8aO0LULyw)

A favorite Qwiklab. Awwvision.

[https://www.qwiklabs.com/focuses/1241?parent=catalog](https://www.qwiklabs.com/focuses/1241?parent=catalog)


### Video AI

Video Intelligence includes several options that you can use to integrate machine learning video intelligence models into your applications and web sites.

[https://cloud.google.com/video-intelligence/overview/docs](https://cloud.google.com/video-intelligence/overview/docs)

[https://www.youtube.com/watch?v=h1zU0Qor9J8](https://www.youtube.com/watch?v=h1zU0Qor9J8)


### Cloud Natural Language API

The [Cloud Natural Language API](https://cloud.google.com/natural-language) provides natural language understanding technologies to developers, including sentiment analysis, entity analysis, entity sentiment analysis, content classification, and syntax analysis. This API is part of the larger Cloud Machine Learning API family.

[https://cloud.google.com/natural-language/docs](https://cloud.google.com/natural-language/docs)

#### Example of using Classification of Bag of Words via Keras

[https://www.youtube.com/watch?v=UFtXy0KRxVI](https://www.youtube.com/watch?v=UFtXy0KRxVI)

#### Gain Insights from Text with Cloud Natural Language API

Qwiklabs GSP097  https://www.qwiklabs.com/focuses/582?parent=catalog

#### Entity Analysis

[https://www.youtube.com/watch?v=3iOtK0sRNMI](https://www.youtube.com/watch?v=3iOtK0sRNMI)


#### RNN & Natural Language generation

[https://www.youtube.com/watch?v=MNvT5JekDpg](https://www.youtube.com/watch?v=MNvT5JekDpg)


### Cloud Translation

Cloud Translation can dynamically translate text between thousands of language pairs. Translation lets websites and programs programmatically integrate with the translation service.

[https://cloud.google.com/translate/docs](https://cloud.google.com/translate/docs)

#### AutoML Translation vs Translation API

The Translation API covers a huge number of language pairs and does a great job with general-purpose text. Where AutoML Translation really shines is for the "last mile" between generic translation tasks and specific, niche vocabularies. Our custom models start from the generic Translation API model, but add a layer that specifically helps the model get the right translation for domain-specific content that matters to you.

https://cloud.google.com/translate/automl/docs/beginners-guide

#### Using Python and Translation API

[https://www.youtube.com/watch?v=YapTts_An9A](https://www.youtube.com/watch?v=YapTts_An9A)


### Text-to-Speech

Text-to-Speech converts text or Speech Synthesis Markup Language (SSML) input into audio data of natural human speech.

[https://cloud.google.com/text-to-speech/docs](https://cloud.google.com/text-to-speech/docs)

#### Cloud Text-to-Speech API using C#

[https://www.youtube.com/watch?v=OK1ZmlaFIV8](https://www.youtube.com/watch?v=OK1ZmlaFIV8)


### Speech-to-Text

Text-to-Speech converts text or Speech Synthesis Markup Language (SSML) input into audio data of natural human speech.

[https://cloud.google.com/speech-to-text/docs](https://cloud.google.com/speech-to-text/docs)

#### Convert speech to text using Node.js

[https://www.youtube.com/watch?v=naZ8oEKuR44](https://www.youtube.com/watch?v=naZ8oEKuR44)

## Difference between AutoML and Cloud Natural language API

Google [AutoML Natural Language](https://cloud.google.com/natural-language/automl/docs) is much more powerful than the [Natural Language API](https://cloud.google.com/natural-language) because it allows the user to train models that are customized for their specific dataset and domain.

It is as easy to use and doesn’t require machine learning knowledge. The two downsides are the higher costs and the necessity of providing a high-quality dataset that needs to train models that perform well.

The AutoML beta supports only three NLP tasks for now (classification, sentiment analysis, entity extraction) and supports only English language documents. 


### Natural Language API 

The [Google Natural Language API](https://cloud.google.com/natural-language) is an easy to use interface to a set of powerful NLP models which have been pre-trained by Google to perform various tasks. As these models have been trained on enormously large document corpuses, their performance is usually quite good as long as they are used on datasets that do not make use of a very idiosyncratic language.

The biggest advantage of using these pre-trained models via the API is, that no training dataset is needed. The API allows the user to immediately start making predictions, which can be very valuable in situations where little labeled data is available.



The Natural Language API comprises five different services:

* Syntax Analysis
* Sentiment Analysis
* Entity Analysis
* Entity Sentiment Analysis
* Text Classification

The major advantage of the Google [Natural Language API](https://cloud.google.com/natural-language) is its ease of use. No machine learning skills are required and almost no coding skills. On the Google Cloud website, you can find code snippets for calling the API for a lot of languages.



The Google [Natural Language API](https://cloud.google.com/natural-language) is a very convenient option for quick, out-of-the-box solutions. Very little technical knowledge and no understanding of the underlying machine learning models is required.

The main disadvantage is its inflexibility and the lack of access to the models. The models cannot be tuned to a specific task or dataset.

In a real-world environment, most tasks will probably require a more tailored solution than the standardized Natural Language API functions can provide.

### AutoML Natural Language

If the [Natural Language API](https://cloud.google.com/natural-language) is not flexible enough for your business purposes, then [AutoML Natural Language](https://cloud.google.com/natural-language/automl/docs) might be the right service. AutoML is a new Google Cloud Service (still in beta) that enables the user to create customized machine learning models. In contrast to the Natural Language API, the AutoML models will be trained on the user’s data and therefore fit a specific task.

Custom machine learning models for classifying content are useful when the predefined categories that are available from the Natural Language API are too generic or not applicable to your specific use case or knowledge domain.

The AutoML service requires a bit more effort for the user, mainly because you have to provide a dataset to train the model. However, the training and evaluation of the models in completely automated and no machine learning knowledge is required. The whole process can be done without writing any code by using the Google Cloud console. Of course, if you want to automate these steps, there is support for all common programming languages.

The training process is quite slow, probably because the underlying models are very big. Training a small test classification task with 15,000 samples and 10 categories and the training can take several hours. A real-world example with a much bigger dataset can take several days.

Fine-tuning big models like [BERT](https://arxiv.org/abs/1810.04805) is a computationally expensive process, especially when a lot of cross-validation is performed.

That means while using AutoML might be very convenient, for performance critical tasks it makes sense to invest the time and develop the model yourself.


## AI Hub

[AI Hub](AI-Hub) is a platform that lets us centralize our code and knowledge in a way that can step up the pace of deployment and learnings globally.

## AI Platform

[AI Platform](AI-Platform) is a development platform to build AI applications that run on GCP and on-premises. 

## ML Frameworks

### Tensorflow 

[Tensorflow](Tensorflow) is an open source, powerful, portable machine learning library developed by Google that can work with very large datasets.


### Scikit Learn


[Scikit Learn](Scikit-Learn)  provides a range of supervised and unsupervised learning algorithms via a consistent interface.


### Keras

[Keras](Keras) is a neural network library. It wraps the efficient numerical computation libraries Theano and TensorFlow and allows you to define and train neural network models.

### Pytorch

[PyTorch](PyTorch)    is an [awesome](https://github.com/bharathgs/Awesome-pytorch-list) source machine learning library based on the Torch library, used for applications such as computer vision and natural language processing, primarily developed by Facebook's AI Research lab.


https://www.guru99.com/pytorch-tutorial.html




### Kubeflow

[Kubeflow](Kubeflow) Pipelines is a platform for building, deploying, and managing multi-step ML workflows based on Docker containers. Kubeflow offers several components that you can use to build your ML training, hyperparameter tuning, and serving workloads across multiple platforms.

### MLOps



[MLOps](MLOps) is the process of taking an experimental Machine Learning model into a production web system. The word is a compound of “Machine Learning” and the continuous development practice of DevOps in the software field. Machine Learning models are tested and developed in isolated experimental systems.

## Metascience and p-value

https://en.wikipedia.org/wiki/P-value

# Links

- [StatQuest videos](https://www.youtube.com/channel/UCtYLUTtgS3k1Fg4y5tAhLbw)
- [Google AI Fun Projects](https://www.youtube.com/watch?v=_IeS1m8r6SY&list=PLIivdWyY5sqLsaG5hNms0D9aZRBE7DHBb&index=1)
- [AI Tutorial](https://www.guru99.com/artificial-intelligence-tutorial.html)
- [AI Platform Training and Prediction sample code repo](https://github.com/GoogleCloudPlatform/cloudml-samples)
- [Guide to bring code to ML GCP](https://github.com/GoogleCloudPlatform/ml-on-gcp)
- [Labs and demos for courses for GCP ML and Bigdata Training](https://github.com/GoogleCloudPlatform/training-data-analyst)
- [Official repo for Google AI Platform](https://github.com/GoogleCloudPlatform/ai-platform-samples)
- [Building Machine Learning and Deep Learning Models on GCP](https://github.com/Apress/building-ml-and-dl-models-on-gcp)
- [Hands-On Machine Learning on GCP](https://github.com/PacktPublishing/Hands-On-Machine-Learning-on-Google-Cloud-Platform)
- [Machine Learning Mastery](https://machinelearningmastery.com/start-here/)
- [Awesome Machine Learning](https://github.com/josephmisiti/awesome-machine-learning)
- [Machine Learning Tutorial](https://www.javatpoint.com/machine-learning)

# Qwiklabs

- https://google.qwiklabs.com/quests/82

