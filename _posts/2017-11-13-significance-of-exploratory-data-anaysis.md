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


At a high level, EDA is the practice of describing the data by means of statistical and visualization techniques to bring important aspects of that data into focus for further analysis. This involves looking at your data set from many angles, describing it, and summarizing it without making any assumptions about its contents. This is a significant step to take before diving into machine learning or statistical modeling, to make sure the data are really what they are claimed to be and that there are no obvious problems. 

![EDA methods]images/edaprocess.png
![EDA-Process:source Wikipedia](https://github.com/Jean-njoroge/jean-njoroge.github.io/tree/master/)

A good data exploration is a preamble to the formal analysis in various ways:
1. By verifying that the expected relationships actually exist in the data, thereby validating the planned techniques of analysis. 
2. By finding some unexpected structure in the data that must be taken into account, thereby suggesting some changes in the planned analysis. 
3. Benefits business stakeholders by confirming they are asking the right questions and not biasing the investigation with their assumptions, as well as by providing the context around the problem to make sure the potential value of the data scientist’s output can be maximized.
 
 
 The phrase exploratory data analysis, was coined by John W. Tukey in 1977.  What, is interesting, is that even though he coined the phrase, it is difficult, if not impossible, to find a precise definition of EDA in Tukey’s writings, partly because he preferred working with vague concepts, things that could be made precise in several ways. As such there are various descriptions of EDA in his work, for example.

> *“If we need a short suggestion of what exploratory data analysis is, I would suggest that: 1. it is an attitude, AND 2. a flexibility, AND 3. some graph paper (or transparencies, or both).” (Jones, 1986, Vol. IV, p. 815).*

### EDA Methods
EDA is generally cross-classified in two ways. First, each method is either non-graphical or graphical. And second, each method is either univariate or multivariate (usually just bivariate). Non-graphical methods generally involve calculation of summary statistics, while graphical methods obviously summarize the data in a diagrammatic or pictorial way. 

![EDA methods ](/images/edamethods.png)
![EDA methods](https://github.com/Jean-njoroge/jean-njoroge.github.io/tree/master/)

* Univariate methods (graphical and non-graphical) look at one variable (data column) at a time, 
* multivariate methods look at two or more variables at a time to explore relationships. Usually our multivariate EDA will be bivariate (looking at exactly two variables), but occasionally it will involve three or more variables. 
* Dimensionality reduction to understand the fields in the data that account for the most variance between observations and allow for the processing of a reduced volume of data
* Cluster analysis is an exploratory data analysis tool for organizing observed data or cases into similar observations in the dataset into differentiated groupings, which by collapsing the data into a few small data points, patterns of behavior can be more easily identified (see figure 4)


In this post, I look at a high level of what EDA entails, describe ways in which EDA is essential in both exploratory and predictive modeling. I hope that this post will spark your curiosity as you know why EDA should be part of the way data science operates in your organization.



