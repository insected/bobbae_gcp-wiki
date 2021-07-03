
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

[https://www.youtube.com/watch?v=nKW8Ndu7Mjw](https://www.youtube.com/watch?v=nKW8Ndu7Mjw)



## Plain and Simple estimators

The Estimators API gives us a nice workflow of getting our raw data, passing it through an input function, setting up our feature columns and model structure, running our training, and running our evaluation.

[https://www.youtube.com/watch?v=G7oolm0jU8I](https://www.youtube.com/watch?v=G7oolm0jU8I)


## Precision & Recall

https://en.m.wikipedia.org/wiki/Precision_and_recall

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

### Logistic Regression

The goal of [logistic regression](https://www.jeremyjordan.me/logistic-regression/), as with any classifier, is to figure out some way to split the data to allow for an accurate prediction of a given observation's class using the information present in the features. (For instance, if we were examining the Iris flower dataset, our classifier would figure out some method to split the data based on the following: sepal length, sepal width, petal length, petal width.) In the case of a generic two-dimensional example, the split might look something like this.

https://www.youtube.com/watch?v=yIYKR4sgzI8

### Decision Trees

[Decision trees](https://www.jeremyjordan.me/decision-trees/) are one of the oldest and most widely-used machine learning models, due to the fact that they work well with noisy or missing data, can easily be ensembled to form more robust predictors, and are incredibly fast at runtime. Moreover, you can directly visual your model's learned logic, which means that it's an incredibly popular model for domains where model interpretability is important.


### K-nearest neighbors


Many machine learning techniques involve building a model that is capable of representing the data and then finding the optimal parameters for the model to minimize error. [K-nearest neighbors](https://www.jeremyjordan.me/k-nearest-neighbors/), however, is an example of instance-based learning where we instead simply store the training data and use it to make new predictions.


### SVM

[Support vector machines](https://www.jeremyjordan.me/support-vector-machines/) classifier works well in complicated feature domains, albeit requiring clear separation between classes. SVMs don't work well with noisy data, and the algorithm scales roughly cubic O(n3) to input depending on your implementation (sklearn's SVM fit time complexity is more than quadratic, so it won't be able to train quickly on large datasets (>10,000 examples).

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


https://www.youtube.com/watch?v=PaFPbb66DxQ&list=PLblh5JKOoLUIzaEkCLIUxQFjPIlapw8nU&index=1


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


### Learning Rate

One of the key hyperparameters to set in order to train a neural network is the [learning rate](https://www.jeremyjordan.me/nn-learning-rate/) for gradient descent. As a reminder, this parameter scales the magnitude of our weight updates in order to minimize the network's loss function.

If your learning rate is set too low, training will progress very slowly as you are making very tiny updates to the weights in your network. However, if your learning rate is set too high, it can cause undesirable divergent behavior in your loss function. 

### Overfitting

Many of the modern advancements in neural networks have been a result of stacking many hidden layers.
This deep stacking allows us to learn more complex relationships in the data. However, because we're increasing the complexity of the model, we're also more prone to [potentially overfitting](https://www.jeremyjordan.me/deep-neural-networks-preventing-overfitting/) our data. 


### Normalization

By [normalizing](https://www.jeremyjordan.me/batch-normalization/) all of our inputs to a standard scale, we're allowing the network to more quickly learn the optimal parameters for each input node.


### Convolutional Neural Networks

[Convolutional neural networks](https://www.jeremyjordan.me/convolutional-neural-networks/) are used heavily in image recognition applications of machine learning. Convolutional neural networks provide an advantage over feed-forward networks because they are capable of considering locality of features.

### Recurrent Neural Networks

[Recurrent neural networks](https://www.jeremyjordan.me/introduction-to-recurrent-neural-networks/) are good  for learning from sequential data.


## Reinforcement Learning

[Reinforcement learning](https://www.jeremyjordan.me/overview-of-reinforcement-learning/) is an approach to machine learning where agents are rewarded to accomplish some task. "Good" behavior is reinforced via a reward, so this approach can more realistically be considered a method of reward maximization. 


Reinforcement learning is a method of learning where we teach the computer to perform some task by providing it with feedback as it performs actions. This is different from supervised learning in that we don't explicitly provide correct and incorrect examples of how the task should be completed, we simply tell the computer when it is doing a good job along the way. Reinforcement learning is also distinct from unsupervised learning because we are providing the computer with some level of feedback, even if we aren't providing explicit examples.

### Markov Decision Process

The [Markov Decision Process](https://www.jeremyjordan.me/markov-decision-process/) is a method for planning in a stochastic environment. Whereas we cannot control or optimize the randomness that occurs, we can optimize our actions within a random environment. Planning for stochastic environments is much more difficult than planning for a deterministic environment; given the randomness present, there's a degree of uncertainty surrounding the results of our actions.


### Monte Carlo learning

The [Monte Carlo](https://www.jeremyjordan.me/rl-learning-implementations/) approach approximates the value of a state-action pair by calculating the mean return from a collection of episodes.


## Natural Language Processing

### TF-IDF Vectorization


[Term frequency-inverse document frequency](https://www.jeremyjordan.me/identifying-related-bodies-of-text-using-tf-idf-vectorization/) (TF-IDF) vectorization is a mouthful to say, but it's also a simple and convenient way to characterize bodies of text. Due to its simplicity, this method scales better than some other topic modeling techniques (latent dirichlet allocation, probabilistic latent semantic indexing) when dealing with large datasets.


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

The Cloud Natural Language API provides natural language understanding technologies to developers, including sentiment analysis, entity analysis, entity sentiment analysis, content classification, and syntax analysis. This API is part of the larger Cloud Machine Learning API family.

[https://cloud.google.com/natural-language/docs](https://cloud.google.com/natural-language/docs)

[https://www.youtube.com/watch?v=UFtXy0KRxVI](https://www.youtube.com/watch?v=UFtXy0KRxVI)

[https://www.youtube.com/watch?v=3iOtK0sRNMI](https://www.youtube.com/watch?v=3iOtK0sRNMI)

[https://www.youtube.com/watch?v=MNvT5JekDpg](https://www.youtube.com/watch?v=MNvT5JekDpg)


### Cloud Translation

Cloud Translation can dynamically translate text between thousands of language pairs. Translation lets websites and programs programmatically integrate with the translation service.

[https://cloud.google.com/translate/docs](https://cloud.google.com/translate/docs)

[https://www.youtube.com/watch?v=YapTts_An9A](https://www.youtube.com/watch?v=YapTts_An9A)


### Text-to-Speech

Text-to-Speech converts text or Speech Synthesis Markup Language (SSML) input into audio data of natural human speech.

[https://cloud.google.com/text-to-speech/docs](https://cloud.google.com/text-to-speech/docs)

[https://www.youtube.com/watch?v=OK1ZmlaFIV8](https://www.youtube.com/watch?v=OK1ZmlaFIV8)


### Speech-to-Text

Text-to-Speech converts text or Speech Synthesis Markup Language (SSML) input into audio data of natural human speech.

[https://cloud.google.com/speech-to-text/docs](https://cloud.google.com/speech-to-text/docs)

[https://www.youtube.com/watch?v=naZ8oEKuR44](https://www.youtube.com/watch?v=naZ8oEKuR44)





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

[PyTorch](https://pytorch.org/)    is an [awesome](https://github.com/bharathgs/Awesome-pytorch-list) source machine learning library based on the Torch library, used for applications such as computer vision and natural language processing, primarily developed by Facebook's AI Research lab.


https://www.guru99.com/pytorch-tutorial.html




### Kubeflow

[Kubeflow](Kubeflow) Pipelines is a platform for building, deploying, and managing multi-step ML workflows based on Docker containers. Kubeflow offers several components that you can use to build your ML training, hyperparameter tuning, and serving workloads across multiple platforms.

### MLOps



[MLOps](MLOps) is the process of taking an experimental Machine Learning model into a production web system. The word is a compound of “Machine Learning” and the continuous development practice of DevOps in the software field. Machine Learning models are tested and developed in isolated experimental systems.



# Links

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