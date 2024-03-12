---
title: "Outliers in machine learning"
datePublished: Fri Jan 27 2023 17:06:43 GMT+0000 (Coordinated Universal Time)
cuid: cldes0of800020al76p6ph1wj
slug: outliers-in-machine-learning
cover: https://cdn.hashnode.com/res/hashnode/image/stock/unsplash/Agx5_TLsIf4/upload/1ab2b4c1a204d056eb5209837b9d2923.jpeg
tags: machine-learning, outliers, outlierdetection

---

Outliers are those data points that are *visibly* different from the rest of the dataset. They are often known as abnormal observations that skew the data distribution and arise due to inconsistent data entry, or erroneous observations.

Outliers are data components or points that cannot be combined in a given class or cluster. These are the data objects which have several behaviors from the usual behavior of different data objects.

Outliers are different from noisy information. Noise is a random bug or variance in a computed variable. In general, noise is not fascinating in data analysis, such as outlier detection.

Outliers are fascinating because they are suspected of not being created by the same structure as the rest of the data. Hence, in outlier detection, it is essential to justify why the outliers identified are produced by several mechanisms.

### **Why Should You Detect Outliers?**

In the machine learning pipeline, *data cleaning* *and preprocessing* is an important step as it helps us better understand the data. During this step, you deal with missing values, detect outliers, and more.

As outliers are very different values—abnormally low or abnormally high—their presence can often skew the results of statistical analyses on the dataset. This could lead to less effective and less useful models.

But dealing with outliers often requires domain expertise, and none of the outlier detection techniques should be applied *without* understanding the data distribution and the use case.

# Problems caused by outliers

* Outliers in the data may cause problems during model fitting (esp. linear models).
    
* Outliers may inflate the error metrics which give higher weights to large errors (for example, mean squared error, RMSE).
    

It becomes pertinent to first detect and then remove the outliers present in your data before proceeding with model building. This certainly will help to build an efficient model in the end.

**Types of Outliers**

1. Type 1 – Global
    
2. Type 2 – Contextual
    
3. Type 3 – Collective
    

### **1\. Global Outliers**

Also known as “Point Anomalies,” are kinds of outliers that deviate significantly from the rest of the data. Measurement will be called a global outlier if it divers from the distribution of data regardless of the features because that measurement is far off the global distribution. It is the simplest type of outlier and is found in the majority of cases.

A global outlier remains distinct from other data points by representing its outliers. It can be better explained by considering a real-life example dataset of credit card fraud detection, which contains transactional data of a bank’s customer who holds a credit card. If we consider the daily transaction amount by the customer as one of the attributes, then a transaction with a very high amount as compared to the normal range of the individual’s expenditure will be considered a Point or Global outlier.

### **2\. Contextual Outliers** 

If a data instance is anomalous in a specific context, then it would be called a contextual outlier or a conditional outlier. Therefore, a contextual outlier will represent a small group of outliers in itself as compared to a significantly larger group of observations. The value might, however, be seen as normal in a different context.

The idea of a context is induced by the structure of the dataset and should be specified as a part of problem formulation. The alternative of applying a contextual outlier technique is decided by the meaningfulness of the contextual outliers in the target domain where it has to be applied.

### **3\. Collective Outliers**

When a subset of observations in a dataset, as a collection, deviates significantly from the entire dataset, it is called a collective outlier. Each instance within the collective outlier doesn't need to be also an outlier. When seeking outlier detection, it is very important to keep the context in mind because sometimes, a point or collective outlier can also be a contextual outlier given the context of the study.

## **Outlier Detection Methods**

### **1\. Statistical Methods**

It starts with visual analysis of the Univariate data by using Boxplots, Scatter plots, etc., which can help in finding the extreme values in the data. Assuming a normal distribution, calculate the z-score, which means the standard deviation (σ) times the data point is from the sample’s mean. Because we know from the Empirical Rule, which says that 68% of the data falls within one standard deviation, 95% percent within two standard deviations, and 99.7% within three standard deviations from the mean, we can identify data points that are more than three times the standard deviation, as outliers. Another way would be to use InterQuartile Range (IQR) as a criterion and treat outliers outside the range of 1.5 times from the first or the third quartile.

### **2\. Proximity Methods**

Proximity-based methods deploy clustering techniques to identify the clusters in the data and find out the centroid of each cluster. They assume that an object is an outlier if the nearest neighbors of the object are far away in feature space; that is, the proximity of the object to its neighbors significantly deviates from the proximity of most of the other objects to their neighbors in the same data set. The usual approach is as follows – Fix a threshold and evaluate the distance of each data point from the cluster centroid and then remove the outlier data points and go ahead with the modeling.

As intuitive as it gets, the success of such types of models heavily depends on the metric used as the distance measure. The drawbacks are that for some specific problem types, there can be a challenge to find the correct distance measure. Another drawback is that it is not that accurate when the group of outliers lies close to each other.

Proximity-based methods are classified into two types: Distance-based methods where a data point is based on the distance(s) to its neighbors. Density-based determines the degree of outlines of each data instance based on its local density. DBScan, k-means, and hierarchical clustering techniques are examples of density-based outlier detection methods.

###  **3\. Projection Methods**

Projection methods utilize techniques such as PCA to model the data into a lower-dimensional subspace using linear correlations. Post that, the distance of each data point to a plane that fits the sub-space is calculated. This distance can be used then to find the outliers. Projection methods are simple and easy to apply and can highlight irrelevant values.

The PCA-based method approaches a problem by analyzing available features to determine what constitutes a “normal” class. The module then applies distance metrics to identify cases that represent anomalies.

### Conclusion

So today we learned about outliers-what is it-why it is important to detect different types of methods. See you in the next blog.