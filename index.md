---
title       : Executive Machine Learning
subtitle    : Or How I Learned to Stop Worrying and Love the Buzzwords
author      : Drew Lanenga
job         : Data Scientist, Lytics
framework   : shower        # {io2012, html5slides, shower, dzslides, ...}
highlighter : highlight.js  # {highlight.js, prettify, highlight}
hitheme     : tomorrow      # 
widgets     : []            # {mathjax, quiz, bootstrap}
mode        : selfcontained # {standalone, draft}

--- #Cover .cover bg:"#7acddf"

## Executive Machine Learning

<img class="cover-img" alt="background" src="https://cloud.githubusercontent.com/assets/3698679/3165966/5563cf64-eb5b-11e3-9136-638fb04d4c1a.jpg" />

<div class="cover-logo-container">
	<img class="cover-logo" alt="logo" src="http://taction.io/images/p_lytics.png" />
</div>

---

## TL;DR

Machine Learning gets a lot of hype for being very sophisticated.  Most machine learning techniques boil down to two tasks: **prediction** and **recommendation**.


Here, we'll walk through each and provide a supplemental glossary for reference.


--- .shout

## Machine Learning


---

## Machine Learning


**[muh·ʃeen  lear·niŋ]**: Any process that uses data to to build models that get better/more accurate with more data.

>  All models are approximations.  Essentially, all models are wrong, but some are useful.
>  &mdash; **George E. P. Box**

---

## Model Building

1. Extract the data and transform it into a useful structure
2. Split data into two groups: *training* and *validation*
    - **Training**: Build the best model you can with part of the data
    - **Validation**: See how the training model performs on the rest of the data
       - If it *performs well*: you're done
       - If it *doesn't perform well*: repeat step 2

--- .takeaway

## You can't use any machine learning model until it has been trained, and your model is no good until it has been validated.

--- .shout

## Prediction

---

## Predictive Analytics

Predictive analytics use *correlated data* to make *predictions* typically in the following categories:

- Predict a **Number** - typically called **regression**
    - *ex.* Predicting a user's future purchase quantity
- Predict a **Label** - typically called **classification**
    - *ex.* Predicting the contents of an image (house, dog, etc.)

--- .shout

## Recommendation

---

## Object similarity

More generally, recommendation is more a problem of determining *object similarity*.

- Similar users are often grouped together for *clustering* or *cohort analysis* to discover hidden segments in the data.
- Similar users can also help drive recommendation engines by the assumption that similar users consume essentially the same content.


---

## Implementation

**High level**: Use distance metrics and/or *matrix factorization* to identify *latent variables* that explain why the data are they way they are.

Matrix factorization yields similar users and similar items.

Recommendations can then be user level (*who you should follow on Twitter*) or item level (*users who bought X also bought Y*).

---

## Interpretation Examples


| Industry | Latent Variable |
| -------- | --------------- |
| Music    | Genre, epoch    |
| Apparel  | Category (fashion forward, dad pants, grunge, etc.) |

Often, latent variables aren't always semantically meaningful and don't have a strict interpretation


--- .shout

## Appendix

---

## Glossary: General

- **Correlation**: Information about one thing implicitly gives you information about another
- **Overfitting**: Building models that don't generalize.  Typically, data is beaten into submission and more anomilies are modeled than actual relationships.
- **Latent variable**: Hidden (non-observable) variables that explain relationships in what is actually observed.

---

## Glossary: Data

- **Cardinality**: Number of unique levels of a variable.
- **Ontology**: Domain-specificy knowledge hierarchy.
    - i.e. flip-flop `->` sandal `->` footwear; jacket `->` outerwear
- **Structured Data**: Data that you can put into a spreadsheet.
- **Unstructured Data**: Typically a bunch of text; any information inside one point could be very different from any other point.

---

## Glossary: Regression

- **Regression**: Using related data to predict a number.  Typically computationally expensive.
- **Regression Tree**: A form of regression built by segmenting the data to create a set of decision rules, called a tree, about a dataset.
- **Logistic Regression**: Specific type of regression used to predict the probability that an event will occur.
- **Gradient Descent**: A method to estimate regression output.  Less computationally expensive.

---

## Glossary: Classification

- **Classification Tree**: Similar to a regression tree, but the output is a category/label/tag.
- **Support Vector Machine**: Another model for classification tasks.
- **Naive Bayes Classifier**: Uses Bayes' Theorem to make classifications.  Performs well when you have a LOT of possible fields.

---

## Glossary: Clustering

- **k-means**: Technique for creating a pre-determined number of clusters (*k*) from data.
- **Hierarchical clustering**: Create a tree of pairwise similar items.  Continue to pair similar *groups* of items until there is one big group.
- **Cohort Analysis**: Analyzing users by the cohort to which they belong, which are typically found by a clustering algorithm. This can lead to identifying user personas, best segments (ROI, retention), etc.

---

## Glossary: Recommendation

- **Collaboritive Filtering**: Technique that assumes that similar people like similar things.  (And that similar things are liked by similar people.)


---

## Glossary: Anomaly Detection

- **Anomaly Detection**: Use regression, classification and clustering to detect outliers.
- **Outlier**: A record that is, by one or more data points, very different from other records.
- **Fraud Detection**: Fraud detection is a special case of anomaly detection.

---

## Glossary: Advanced

- **Bootstrap**: Taking smaller samples of a larger dataset multiple times, and running the analysis on the smaller sets.  When the output is aggregated across samples, this is sometimes used as a sort of pesudo-divide and conquer approach to analyze larger data sets.
- **Bagging**: Bootstrap aggregating, averaging the results of a bootstrap.
- **Random Forest**: Essentially a bagging with regression/classification trees.

---

## Glossary: Advanced

- **Neural Network**: Sophisticated approach to modeling non-linear relationships.  Very accurate, but a complete black box -- you can't tell how it built the model, but it works.
