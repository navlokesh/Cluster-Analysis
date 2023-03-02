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

#### Hierarchical Clustering:

Dendrograms were visualized to choose the number of clusters for our algorithm. 

![image](https://user-images.githubusercontent.com/33120664/222536808-59cc1dc8-1eeb-445b-8e2d-2fb0cf8260d8.png)

The above dendrogram suggests the optimal number of clusters. Below is the truncated dendrogram:
![image](https://user-images.githubusercontent.com/33120664/222537066-b164e1a9-1af3-49b7-a66d-485dd11bd816.png)

#### K-Means Clustering:

WSS plot was checked to determine the number of clusters for our model. The below graph shows the optimal number of clusters as 3:
![image](https://user-images.githubusercontent.com/33120664/222537347-de82ab03-9392-49f2-97b7-763f72bad9e2.png)

silhouette scores was checked to determine the model's performance.


## Cluster characteristics:
Further, various characteristics of out clusters were analyzed.

Cluster 1: Averages of variables

spending - 	18.37
Advance Payment -	16.14
Prob of full payment -	0.88
Current balance - 	6.15
Credit Limit - 		3.68
min payment amt - 	3.63
Max spent in single sh- 6.01

Cluster 2: Averages of variables

spending - 	11.87
Advance Payment -	13.25
Prob of full payment -	0.84
Current balance - 	5.23
Credit Limit - 		2.84
min payment amt - 	4.94
Max spent in single sh- 5.12

Cluster 3: Averages of variables

spending - 	14.19
Advance Payment -	14.23
Prob of full payment -	0.87
Current balance - 	5.47
Credit Limit - 		3.22
min payment amt - 	2.61
Max spent in single sh- 5.08

## Inference or Conclusion:

The bank wants to develop a customer segmentation to give promotional offers to its customers.

So, if the bank attracts the customers spedning the least by giving them promotional offers, those customers may start spending more. Hence focusing more on the cluster of customers spedning would benefit the bank.

The Probability of full payment is almost same for all the clusters. Hence, bank need not concentrate on this factor when they are devoloping the customer segmentation to give promotional offers.

From the averages above, we can see that a customer with higher credit limit seems to spend high.
So, Bank may consider increasing the credit limit for the customers with lower limit, after evaluating the customer's credit scores or repayment ebility.
Customers from cluster 1 are utilizing thier credit limit by 50%, while other 2 clusters seem to be utilizing lesser when compared to cluser 1.

Banks may use this insight to give attractive promotional offers to the customers from cluster 2 and 3 which would make the customer increase the utilization.
