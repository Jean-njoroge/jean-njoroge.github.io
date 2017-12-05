---
layout: post
title: "Significance of Exploratory Data Analysis (EDA)"
date: 2017-11-13
tags:
- machine learning
- Data science
- exploratory data analysis
- univariate analysis
- bivariant analysis
---
Data science is ubiquitous to advanced statistical and machine learning techniques. As long as there is data to analyze, the need to explore is obvious.Yet, an important key component to any data science task frequently undervalued is the exploratory data analysis (EDA). 


At a high level, EDA is the practice of describing the data by means of statistical and visualization techniques to bring important aspects of that data into focus for further analysis. This involves looking at your data set from many angles, describing it, and summarizing it without making any assumptions about its contents. This is a significant step to take before diving into machine learning or statistical modeling, to make sure the data are really what they are claimed to be and that there are no obvious problems. EDA should be part of the way data science operates in your organization.

The phrase exploratory data analysis was coined by John W. Tukey in 1977.  What, is interesting, is that even though he coined the phrase, it is difficult, if not impossible, to find a precise definition of EDA in Tukey’s writings, partly because he preferred working with vague concepts, things that could be made precise in several ways. As such there are various descriptions of EDA in his work, for example.

> *“If we need a short suggestion of what exploratory data analysis is, I would suggest that: 1. it is an attitude, AND 2. a flexibility, AND 3. some graph paper (or transparencies, or both).” (Jones, 1986, Vol. IV, p. 815).*

![EDA methods](/images/edaprocess.png)

![EDA-Process:source Wikipedia](https://github.com/Jean-njoroge/jean-njoroge.github.io/tree/master/)


A good data exploration is a preamble to the formal analysis. It allows the data scientist to: 
1. Verify expected relationships actually exist in the data, thus formulating and validating planned techniques of analysis. 
2. To find some unexpected structure in the data that must be taken into account, thereby suggesting some changes in the planned analysis. 
3. Deliver data-driven insights to business stakeholders by confirming they are asking the right questions and not biasing the investigation with their assumptions.
4. Provide the context around the problem to make sure the potential value of the data scientist’s output can be maximized.


## EDA Methods
EDA is generally cross-classified in two ways. First, each method is either non-graphical or graphical. And second, each method is either univariate or multivariate (usually just bivariate). Non-graphical methods generally involve calculation of summary statistics, while graphical methods obviously summarize the data in a diagrammatic or pictorial way. 

![EDA methods ](/images/edamethods.png)
![EDA methods](https://github.com/Jean-njoroge/jean-njoroge.github.io/tree/master/)

In addition to the above methods, other exploratory data analysis methods include: 

* **Dimensionality reduction:** reduces the number of variables to a few interpretable linear combinations of the data making it easier to understand the fields in the data that account for the most variance between observations and allow for the processing of a reduced volume of data.
* **Cluster analysis:** organizes observed data into similar observations in the dataset into differentiated clusters (groups, which allows for easy identification of patterns of behavior.

## Code
To view an example of EDA , see code for the dataset on Breast Cancer from UCI repository here for an example of EDA [ipython notebook ](https://github.com/Jean-njoroge/Breast-cancer-risk-prediction/blob/master/NB2_ExploratoryDataAnalysis.ipynb)



## Conclusion
In this post, I look at a high level of what EDA entails, describe ways in which EDA is essential in both exploratory and predictive modeling. 



