---
title       : Executive Machine Learning
subtitle    : How I Learned to Stop Worrying and Love the Buzzwords
author      : Drew Lanenga
job         : Data Scientist, Lytics
framework   : shower        # {io2012, html5slides, shower, dzslides, ...}
highlighter : highlight.js  # {highlight.js, prettify, highlight}
hitheme     : tomorrow      # 
widgets     : []            # {mathjax, quiz, bootstrap}
mode        : selfcontained # {standalone, draft}

--- #Cover .cover bg:"#7acddf"

## Executive Machine Learning

---

## Executive Machine Learning

1.  What machine learning is
2.  What "predictive analytics" are
3.  Executive glossary to lookup key buzzwords

--- .shout

## Machine Learning


---

## Machine Learning


**muh·ʃeen  lear·niŋ**: Any process that uses data to get better/more accurate.

Machine learning is what allows *predictive analytics* to be *predictive*.

---

## Model Building

1. Extract the data and transform it into a useful structure
2. Split data into two groups: *training* and *validation*
    - **Training**: Build the best model you can with part of the data
    - **Validation**: See if the training model performs on the rest of the data
       - If it *performs well*: you're done
       - If it *doesn't perform well*: repeat step 2

You **can't use any machine learning model until it has been trained**, and your model is **no good until it has been validated**.

--- .shout

## Predictive Analytics

---

## Predictive Analytics

Predictive analytics make *predictions* typically in the following categories:

- Predict a value
- Predict clusters
- Make a recommendation

---

## Predicting Values

- Predict a **Number** - typically called **regression**
    - 
- Predict a **Label** - typically called **classification**
    - 

--- .shout

## Appendix

---

## Glossary: General

- **Machine Learning**: Processes that get smarter (more accurate/predictive) with more data
- **Correlation**: Information about one thing implicitly gives you information about another
- **Overfitting**: Building models that don't generalize.  Typically, data is beaten into submission and more anomilies are modeled than actual relationships.

---

## Glossary: Data

- **Cardinality**: Number of unique levels of a variable
- **Ontology**: Domain-specificy knowledge hierarchy.
    - i.e. flip-flop `->` sandal `->` footwear; jacket `->` outerwear
- **Structured Data**: Data that you can put into a spreadsheet
- **Unstructured Data**: Typically a bunch of text; any information inside one point could be very different from any other point

---

## Glossary: Regression

- **Regression**: Using related data to predict a number
- **Regression Tree**: A form of regression built by segmenting the data to create a set of decision rules, called a tree, about a dataset.  A number is output.
- **Logistic Regression**: Specific type of regression used to predict the probability that an event will occur

---

## Glossary: Classification

- **Classification Tree**: Similar to a regression tree, but the output is a category/label/tag.
- **Support Vector Machine**: Another model for classification tasks
- **Naive Bayes Classifier**: Uses Bayes' Theorem to make classifications.  Performs well when you have a LOT of possible fields

---

## Glossary: Clustering

- **k-means**: Create a pre-determined number of clusters (*k*) from data

---

## Glossary: Anomaly Detection

- **Anomaly Detection**: Use
- **Outlier**: A record that is, by one or more data points, very different from other records.

---

## Glossary: Advanced

- **Bootstrap**: Taking smaller samples of a larger dataset multiple times, and running the analysis on the smaller sets.  When the output is aggregated across samples, this is sometimes used as a sort of pesudo-divide and conquer approach to analyze larger data sets.
- **Bagging**: Bootstrap aggregating, averaging the results of a bootstrap.
- **Random Forest**: Essentially a bagging with regression/classification trees.
- **Neural Network**: Sophisticated approach to modeling non-linear relationships.  Very accurate, but a complete black box -- you can't tell how it built the model, but it works.



"iOS 8 is the biggest iOS release ever"
"so you can do more than ever"
"The all-new Photos app makes it simpler than ever..."
"Our smartest keyboard ever"
"It's also easier than ever to share family photos"
"Spotlight.  Brighter than ever."
