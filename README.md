# Cluster-Analysis:

## Problem Statement:
A leading bank wants to develop a customer segmentation to give promotional offers to its customers. They collected a sample that summarizes the activities of users during the past few months. The task is to identify the segments based on credit card usage.

## EDA and Data Preprocessing:

Exploratory Data Analysis was performed. Data was chcecked for null values and duplicated rows.
Outlier checks were done using boxplots. Univariate and bivariate analysis of features were performed using histograms, skewness checks, pairplots, heatmaps and statistical measures such as covariance and correlations between the variables was checked.

## Checking for the need of Data Scaling:

Data Scaling is necessary in this case. Because, our dataset contains features varying in magnitudes, units and range.
Since, the algorithms we use for clustering use distance between two data points in their computations, this is a problem.
To supress this effect, we need to bring all features to the same level of magnitudes. This can be acheived by scaling.

Scaling was performed using standard scaler.

## Model Building:

Differnt clustering algorithms were applied such as hierarchical clustering and K-Means clustering.

Hierarchical Clustering:

Dendrograms were visualized to choose the number of clusters for our algorithm. 

![image](https://user-images.githubusercontent.com/33120664/222536808-59cc1dc8-1eeb-445b-8e2d-2fb0cf8260d8.png)
