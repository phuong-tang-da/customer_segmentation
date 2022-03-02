# Customer Segmentation
## Inspirations
Market segmentation is an advanced technique in marketing research. **A simple, traditional and easy-to-understand method of segmentation**, which can be used is groupings based on intuitions and arbitrary thresholds. For example, deciding to segment customers into different income tiers based on $10,000 increments. However, traditional approach becomes much more complex to apply on large dataset with many variables. This project will look at a more powerful technique for performing customer segmentation, which can be easily used by most companies for a bigger and more complicated dataset: **unsupervised machine learning**. This machine learning technique help finds data points that are most like each other and groups them together, which is exactly what good customer segmentation techniques should do.

## Overview of dataset
In this project, I will use a dataset of Instacart, a grocery ordering and delivery app. Data consists of information about purchase behavior of 131,209 customers.
Source: https://www.kaggle.com/c/instacart-market-basket-analysis 

## Objectives
- To understand customer behaviors (frequency & pattern of purchase) and product preferences
- To perform behavioral segmentation and identify unique profile of different customer segments and make relevant recommendations for each segment

## Summary of approach
#### 1.	Data preparation (Numpy, Pandas) 
-	To identify potential relationships between variables
-	To understand general behaviors of customers in term of purchase frequency, purchase pattern, product preferences
-	To create relevant variables and dataset for modeling
#### 2.	Data modeling (PCA, k-mean clustering)
##### 2.1.	Segmentation by Product aisle preference using absolute data: the result is not interpretable because of below reasons:
-	The only differences between segments is total number of products purchased per user: users who order many products vs. users who order less products
-	The model fails to record the aisle preference of each segment: The top 5 popular aisles remain similar across 4 segments (fresh fruits, fresh vegetables...) 
##### 2.2.	Segmentation by Product aisle preference using normalized data (eliminate the impact of basket size on final result)
##### 2.3.	Segmentation by User behaviors
##### 2.4.	Segmentation by both User behavior & Product aisle preference
#### 3.	User segment exploration: 
-	To identify best approach for a comprehensive data interpretation
-	To identify unique profile of each segment

## Results

