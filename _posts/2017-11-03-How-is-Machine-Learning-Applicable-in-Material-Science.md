---
layout: post
title: "How is Machine Learning Applicable in Material Science?"
date: 2017-11-03
tags:
- machine learning
- material science
- algorithms 
---

A few weeks ago, a colleague asked me - “How Machine Learning is Applicable Material Science?”. It got me interested, because these are two topics, I understand very well. We both studied Computational Material Science (Material Informatics), utilized python and other tools to build models, evaluated terabytes of data from simulations, used statistical mechanics and numerical methods to extract useful insights on the structure-property relationships of material. Indeed, machine learning methods sound familiar to a computational material scientist, but it is an elusive familiarity.  In this blog, I will examine areas in which machine learning and material science intertwine.
> *Our everyday existence is influenced by materials, from Silicon chips storage of data in billionths of a second, to new alloys for automobile engines, to solar panels for renewable energy. Indeed, advances in materials shape our day-to-day lives and drive economic growth. Simply put materials make things happen.*

Propelled by [Materials Genome Initiative](https://www.mgi.gov/),algorithmic developments; and unquestionable successes of data-driven efforts in other domains, informatics strategies are beginning to take shape within materials science. Using material properties data and advanced computer models, engineers can realistically simulate the behavior of new materials in specific applications and avoid lengthy cycles of build and test.  These simulations cover a wide range of operating environments and length and time scales. The new field, called computational materials science, is one of the fastest growing areas within the field of chemistry and materials science.

### Machine learning in Material Science
Machine learning automates analytical model building, using algorithms that iteratively learn from data, allowing computers to find hidden insights without being explicitly programmed. Much has been written about machine learning and how our daily activities; web searches, credit scoring, fraud detection, and text analysis amongst others influenced by this field.

 In material science, machine learning is critical in areas such as new materials discovery and material property prediction. For example, in an experiment on predicting the glass transition temperature Tg it is difficult to find a formula that can accurately describe the relationship between Tg and the four relevant factors of rigidness, chain mobility, average molecular polarizability and net charge; however, a machine learning method can be used to model the relationships between conditional factors and decision attributes based on a given sample. This is where machine learning plays a role and where the “core” algorithms lie. The knowledge obtained through machine learning is stored in a format that is readily usable and, in turn, can be used for materials discovery and design. 

### Basic Steps of Machine learning in Material Science
Basic steps of machine learning in material science, involves three steps, sample generation, module building and model evaluations

![general process of machine learning in materials science ](/images/ml-process.png)
![General process of machine learning in materials science](https://github.com/Jean-njoroge/jean-njoroge.github.io/tree/master/)

* **Sample construction:** raw data is collected from computational simulations and experimental measurements. Mostly, data is incomplete, noisy and inconsistent, hence, data cleaning should be performed when constructing a sample from raw data. 
* **Model building**: input data is linked to output data using a set of nonlinear or linear functions. in materials science, complex relationships usually exist between the conditional factors and the target attributes, which traditional methods have difficulty handling. 
* **Model evaluations**: A data-driven model should achieve good performance not only on existing data but also on unseen data. Generally, we can evaluate the generalization errors of models by means of calculation-based tests and use the results to select the best one. 

### Machine learning and material property predication
Regardless of problem under study, a criterion for machine learning is existence of past data, either clean, curated and reliable data corresponding to the problem under study should already be available, or an effort is in place for the creation of the data.

In material science, a machine learning framework for predicting material properties, includes a dataset with attributes relating to a variety of materials that fall within a  chemical class of interest, and a relevant measured or computed property of those materials i.e., the material, is referred to as “input”, and the property of interest, is referred to as the “target” or “output.”   learning problem is then defined as follows: 
Given a {materials → property} dataset, what is the best estimate of the property for a new material not in the original dataset?

An approach to understanding this problem, is to first represent numerically the various input cases (or materials) in the dataset. Each input case would have been reduced to a string of numbers, it is important to emphasize this step, because this is where one requires significant expertise and knowledge of the materials class and the application (‘domain expertise”).

![GitHub Logo](/images/property-prediction.png)
![Property predicition application of machine learning in materials science.](https://github.com/Jean-njoroge/jean-njoroge.github.io/tree/master/)

The second step establishes a mapping between the features and the target property, and is entirely numerical in nature, largely devoid of the need for domain knowledge. Both the fingerprinting and mapping/learning steps are schematically.
Several algorithms, ranging from simple (e.g., linear regression) to highly sophisticated (kernel ridge 4 regression, decision trees, deep neural networks), are available to establish this mapping and the creation of surrogate prediction models. While some algorithms provide actual functional forms that relate input to output (e.g., regression), others do not (e.g., decision trees). 

In this discussion, the assumption is that the target property is a continuous quantity (e.g., bulk modulus, band gap, melting temperature, etc.). Problems can also involve discrete targets (e.g., crystal structure, specific structural motifs, etc.), which are referred to as classification problems.  Throughout the machine learning process, it is essential to adhere to rigorous statistical practices. Central to this is the notion of cross-validation and testing on unseen data, which attempt to ensure that a learning model developed based on the original dataset can truly handle a new case without falling prey to the perils of “overfitting”.

### Conclusions

The materials science community is just beginning to explore and utilize the plethora of available information theoretic algorithms to mine and learn from data. Machine learning should be viewed as the sum total of the organized creation of the initial dataset, the fingerprinting and learning steps, and a necessary subsequent step (discussed at the end of this article) of progressive and targeted new data infusion, ultimately leading to an expert recommendation system that can continuously and adaptively improve.

### References:

*	Yu et.al. Material discovery and design using machine learning. J. Materiomics 3 (2017) 159- 177
*	Ramprasad et.al., Machine Learning and Materials Informatics: Recent Applications and Prospects

