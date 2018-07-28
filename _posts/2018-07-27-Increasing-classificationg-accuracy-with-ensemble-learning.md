---
layout: post
title: "Increasing Classification Accuracy with Ensemble Learners"
date: 2018-07-27
tags:
- machine learning
- Data science
- ensemble learning
- bagging
- boosting
- stacking
---
Ensemble learning is a machine learning concept that combines multiple learning algorithms. Each of which solves the same original task, to obtain a better combined model, with more accurate and reliable estimates or decisions than can be obtained from using a single model. Given a complex classification problem as is often in many industrial challenges -- from investment timing to drug discovery, and fraud detection to recommendation systems, different approaches are applied to the classification problem. However, while in search for a viable solution, various algorithms are applied, sometimes none of them are better than the rest. In such instances, one can elect to keep them all and then select the final classifier, by combining the individual classifiers. 

### How then is the combination achieved? 

As a quick answer, I can take the average, or I can apply the different ways of making the most out of my sub-classifiers.  This is the idea behind ensemble learning. Divide the decision amongst several classifiers to arrive to a more accurate or representative decision - divide-and-conquer technique of the machine learning world.

> **Ensemble machine learning methods use multiple learning algorithms to obtain better predictive performance than could be obtained from any of the constituent learning algorithms,**

Ensembles techniques are based on algorithms, some of which are simple and less computational intensive, while others are quite complex and more computation intensive. In any production environment, both accuracy and computation time are important. Thus, in most instances, data scientist need to make compromise between accuracy and time. This compromise is achieved by combining many weak learners to gain a confidence index out of them, which is essential in implementing such a system for real-time application with very high accuracy. The figure below shows the basic architecture of and framework:


![Ensemble learning architeceture](/images/ensemble-learning.png)
![general process of machine learning in materials science ](/images/ml-process.png)
### Why use ensemble methods?
Under what circumstances does one need to use ensemble methods? You may ask! Although one would argue that there are various reasons of why, more or less thinking outside the box, here I outline some of the general reasons to use ensemble learning, some of which are:
 * **Large dataset**: It is challenging to train a large data set using a single model, in such instances a data scientist will create a small subset of data to train different models, and eventually choose the average of all as the final prediction.
 * **Small data set**:  Similarly, a dataset is too small to train a single model in such instances a data scientist will use bootstrap methods to create random subsamples of data to train the models.
 * **Complex (nonlinear) data**:  real-world datasets are nonlinear, where a single model cannot define the class boundary clearly. This is known as under-fitting of the model. In such cases, a data scientist uses more than one model to train different subsets of the data and average out the result at the end to predict distinct boundaries.
* **Minimize error**: main cause of error in machine learning, are due to noise, bias and variance. Ensemble methods helps to minimize these errors. The methods are designed to improve the stability and accuracy of machine learning algorithms. Combination of multiple classifiers decrease variance, especially in the case of unstable classifier and may produce a more reliable classifier than a single classifier. 
o	Let’s recap on the different types of errors
    * Bias error quantifies how much on an average are the predicted values different from the actual value. A high bias error means we have an under-performing model which keeps on missing important trends.
    * Variance quantifies how are the prediction made on same observation different from each other. A high variance model will over-fit on your training population and perform badly on any observation beyond training. Thus, failing to generalize model on any unseen data. Following diagram will give you more clarity (Assume that red spot is the real value and blue dots are predictions):

### Ensemble Approaches {Next Post]
In next post, I want to explore some examples for increasing classification accuracy using ensemble learning approaches, bagging, boosting and stacking, which all leverage a crowd of experts. The objective is to improve accuracy by decreasing variance (bagging), bias(boosting), or improve predictions(stacking).

