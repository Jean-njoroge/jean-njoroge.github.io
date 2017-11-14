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

![EDA-Process ](/images/edaprocess.png)
![EDA Process](https://github.com/Jean-njoroge/jean-njoroge.github.io/tree/master/)

### What is Exploratory Data Analysis (EDA)?
As long as there is data to analyze, the need to explore is obvious.  The phrase EDA, was coined/defined by John W. Tukey in 1977. Indeed, he reenergized descriptive statistics through EDA and changed the language and paradigm of statistics in doing so. What, I find intriguing is that it is hard, if not impossible, to find a precise definition of EDA in Tukey’s writings. Which, is not a surprise, because he preferred working with vague concepts, things that could be made precise in several ways. He introduced EDA, but describing its characteristics and creating novel tools.  You will find various descriptions of EDA in his work, for example.

> *“If we need a short suggestion of what exploratory data analysis is, I would suggest that: 1. it is an attitude, AND 2. a flexibility, AND 3. some graph paper (or transparencies, or both).” (Jones, 1986, Vol. IV, p. 815).*

At a high level, EDA is the practice of describing the data by means of statistical and visualization techniques to bring important aspects of that data into focus for further analysis. This involves looking at your data set from many angles, describing it, and summarizing it without making any assumptions about its contents. 

### EDA Methods
EDA is generally cross-classified in two ways. First, each method is either non-graphical or graphical. And second, each method is either univariate or multivariate (usually just bivariate). Non-graphical methods generally involve calculation of summary statistics, while graphical methods obviously summarize the data in a diagrammatic or pictorial way. 

![EDA methods ](/images/eda_methods.png)
![EDA methods](https://github.com/Jean-njoroge/jean-njoroge.github.io/tree/master/)

* Univariate methods (graphical and non-graphical) look at one variable (data column) at a time, 
* multivariate methods look at two or more variables at a time to explore relationships. Usually our multivariate EDA will be bivariate (looking at exactly two variables), but occasionally it will involve three or more variables. 
* Dimensionality reduction to understand the fields in the data that account for the most variance between observations and allow for the processing of a reduced volume of data
* Cluster analysis is an exploratory data analysis tool for organizing observed data or cases into similar observations in the dataset into differentiated groupings, which by collapsing the data into a few small data points, patterns of behavior can be more easily identified (see figure 4)



Validating assumptions and identifying patterns

One of the main purposes of EDA is to look at the data before assuming anything about it. This is important, first, so that the data scientist can validate any assumptions that might have been made in framing the problem or that are necessary for using certain algorithms. Second, assumption-free exploration of the data can aid in the recognition of patterns and potential causes for observed behavior that could help answer the question at hand or inform modeling choices.

Often there are two types of assumptions that can affect the validity of analysis: technical and business. The proper use of certain analytical models and algorithms relies on specific technical assumptions being correct, such as no collinearity between variables, variance in the data being independent of the data’s value, and whether data is missing or corrupted in some way. During EDA, various technical assumptions are assessed to help select the best model for the data and task at hand. Without such an assessment, a model could be used for which assumptions are violated, making the model no longer applicable to the data in question and potentially resulting in poor predictions and incorrect conclusions that could have negative effects for an organization. Furthermore, EDA helps during the feature engineering stage by suggesting relationships that might be more efficiently encoded when incorporated into a model.

The second type of assumption, the business assumption, is a bit more elusive. With proper knowledge of a model, the data scientist knows each type of assumption that must be valid for its use and can go about systematically checking them. Business assumptions, on the other hand, can be completely unrecognized and deeply entangled with the problem and how it is framed. Once, we were working with a client who was trying to understand how users interacted with their app and what interactions signaled likely churn. Deeply embedded in their framing of the problem was their assumption that their user base was composed of, say, experienced chefs looking to take their cooking to the next level with complex recipes. In fact, the user base was composed mostly of inexperienced users trying to find recipes for quick, easy-to-make meals. When we showed the client the assumption that they had been building their app upon was misinformed, they had to pivot and embark on understanding a whole new set of questions to inform future app development.

While validating these technical and business assumptions, the data scientist will be systematically assessing the contents of each data field and its interactions with other variables, especially the key metric representing behavior that the business wants to understand or predict (e.g. user lifetime, spend). Humans are natural pattern recognizers. By exhaustively visualizing the data in different ways and positioning those visualizations strategically together, data scientists can take advantage of their pattern recognition skills to identify potential causes for behavior, identify potentially problematic or spurious data points, and develop hypotheses to test that will inform their analysis and model development strategy.

Building an intuition for the data

There is also a less concrete reason for why EDA is a necessary step to take before more advanced modeling: data scientists need to become acquainted with the data first hand and develop an intuition for what is within it. This intuition is especially important for being able to quickly identify when things go wrong. If, during EDA, I plot user lifetime versus age and see that younger users tend to stay with a product longer, then, I would expect whatever model I build to have a term that would result in increased lifetime when age is decreased. If I train a model that shows different behavior, I would quickly realize that I should investigate what is happening and make sure I didn’t make any mistakes. Without EDA, glaring problems with the data or mistakes in the implementation of a model can go unnoticed for too long and can potentially result in decisions being made on wrong information.

Validating that the data is what you think it is

In the days of Tukey-style EDA, the analyst was typically well aware of how the data they were analyzing was generated. However, now as organizations generate vast numbers of datasets internally as well as acquire third-party data, the analyst is typically far removed from the data generation process. If the data is not what you think it is, then your results could be poorly affected, or worse, misinterpreted and acted on.

One example of a way data generation can be misinterpreted and cause problems is when data is provided at the user level but is actually generated at a higher level of granularity (such as for the company, location, age group the observation is a part of). This situation results in data being the same for otherwise disparate users within a group.

Let’s look at Company A’s situation. Company A is trying to predict which of its users would subscribe to a new product offering in order to target them. They are having a hard time developing a model—every attempt results in poor predictions. Then someone thinks to perform extensive EDA, a task that they at first thought was unnecessary for achieving their desired results. The results show them that the subscribers being predicted for were part of larger corporate accounts who controlled what products their employees subscribed to. This control meant that users could look exactly the same in the data in every way but have different target outcomes, meaning that the individual-level data had little ability to inform predictions. Not only did EDA in this case expose technical problems with the approach taken so far but it also showed that the wrong question was being asked. If the subscriber’s’ behavior was controlled by its organization, there was no business use to targeting subscribers. The company needed to target and thus predict new product subscriptions for corporate accounts.

Other examples that we have seen where data generation process has been wrongfully assumed:

Data is generated the same across versions of a product or across platforms.
Data is timestamped according to X time zone or the same across time zones.
Data is recorded for all activity but is only recorded when a user is signed in.
Identifiers for users remain constant over time or identifiers are unique.
