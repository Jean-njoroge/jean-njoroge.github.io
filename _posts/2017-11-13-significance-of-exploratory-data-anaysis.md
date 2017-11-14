---
layout: post
title: "Significance of Exploratory Data Analysis"
date: 2017-11-13
tags:
- machine learning
- Data science
- exploratory data analysis
- univariate analysis
- bivariant analysis
---
*“Exploratory data analysis isolates patterns and features of the data and reveals these forcefully to the analyst.” (Hoaglin, Mosteller, & Tukey, 1983, p. 1)*

I am a curious person, perhaps the reason why as part of the data science task, exploration of the data is one of my favorite.  In this post, I look at a high level of what EDA entails, describe ways in which EDA is essential in both exploratory and predictive modeling. As I continue learning and updating my DS skills, I hope that this post will spark your curiosity as you know why EDA should be part of the way data science operates in your organization.

### Introduction

 Data science is ubiquitous to advanced statistical and machine learning techniques. Yet, an important key component to any data science endeavor frequently undervalued or forgotten: exploratory data analysis (EDA). It is a crucial step to take before diving into machine learning or statistical modeling to make sure that the data are really what they are claimed to be and that there are no obvious problems. But good exploration also prepares you for the formal analysis in various ways:

1. By verifying that the expected relationships actually exist in the data, thereby validating the planned techniques of analysis. 
2. By finding some unexpected structure in the data that must be taken into account, thereby suggesting some changes in the planned analysis. 
3. Benefits business stakeholders by confirming they are asking the right questions and not biasing the investigation with their assumptions, as well as by providing the context around the problem to make sure the potential value of the data scientist’s output can be maximized.

### What is Exploratory Data Analysis (EDA)?
As long as there is data to analyze, the need to explore is obvious.  The phrase EDA, was coined/defined by John W. Tukey in 1977. Indeed, he reenergized descriptive statistics through EDA and changed the language and paradigm of statistics in doing so. What, I find intriguing is that it is hard, if not impossible, to find a precise definition of EDA in Tukey’s writings. Which, is not a surprise, because he preferred working with vague concepts, things that could be made precise in several ways. He introduced EDA, but describing its characteristics and creating novel tools.  You will find various descriptions of EDA in his work, for example.

> *“If we need a short suggestion of what exploratory data analysis is, I would suggest that: 1. it is an attitude, AND 2. a flexibility, AND 3. some graph paper (or transparencies, or both).” (Jones, 1986, Vol. IV, p. 815).

At a high level, EDA is the practice of describing the data by means of statistical and visualization techniques to bring important aspects of that data into focus for further analysis. This involves looking at your data set from many angles, describing it, and summarizing it without making any assumptions about its contents. EDA is generally cross-classified in two ways. First, each method is either non-graphical or graphical. And second, each method is either univariate or multivariate (usually just bivariate). Non-graphical methods generally involve calculation of summary statistics, while graphical methods obviously summarize the data in a diagrammatic or pictorial way. 


