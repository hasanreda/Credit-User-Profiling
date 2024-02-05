# Customer Segmentation and Behavioral Analysis for Enhanced Credit Card Services

## Project's objectives

The objective of clustering on financial data to create customer segments is to identify distinct groups or segments of customers based on their financial behavior and characteristics. By clustering customers into segments, we can gain insights into their preferences, needs, and behaviors, which can inform targeted marketing strategies and personalized offerings.

The specific objectives of this analysis may include:

1. **Customer Segmentation**: Divide customers into homogeneous groups based on their financial attributes, such as credit card usage, purchase behavior, payment patterns, and credit limits.

2. **Identify Key Features**: Determine the key features or variables that differentiate the customer segments and contribute the most to the clustering results. This can help in understanding the factors that drive customer behavior and preferences.

3. **Segment Profiling**: Profile each customer segment by analyzing their demographic information, transactional patterns, and other relevant characteristics. This can provide a deeper understanding of the unique characteristics and needs of each segment.

4. **Targeted Marketing**: Develop targeted marketing strategies and campaigns tailored to each customer segment. By understanding the preferences and needs of different segments, we can create personalized offers, promotions, and communication strategies to maximize customer engagement and satisfaction.

5. **Business Insights**: Gain insights into the overall customer base and identify opportunities for business growth and improvement. By analyzing the distribution of customers across segments, we can identify potential market gaps, areas of high profitability, and areas for improvement in customer satisfaction and retention.

Overall, the objective of clustering on financial data is to leverage data-driven techniques to uncover meaningful patterns and segments within the customer base. This can enable businesses to make informed decisions, optimize marketing efforts, and enhance customer experiences.

## Overview:

This case requires to develop a customer segmentation to define marketing strategy. The
sample Dataset summarizes the usage behavior of about 9000 active credit card holders during the last 6 months. The file is at a customer level with 18 behavioral variables.

Following is the Data Dictionary for Credit Card dataset :-

CUST_ID : Identification of Credit Card holder (Categorical)

BALANCE : Balance amount left in their account to make purchases 

BALANCE_FREQUENCY : How frequently the Balance is updated, score between 0 and 1 (1 = frequently updated, 0 = not frequently updated)

PURCHASES : Amount of purchases made from account

ONEOFF_PURCHASES : Maximum purchase amount done in one-go

INSTALLMENTS_PURCHASES : Amount of purchase done in installment

CASH_ADVANCE : Cash in advance given by the user

PURCHASES_FREQUENCY : How frequently the Purchases are being made, score between 0 and 1 (1 = frequently purchased, 0 = not frequently purchased)

ONEOFFPURCHASESFREQUENCY : How frequently Purchases are happening in one-go (1 = frequently purchased, 0 = not frequently purchased)

PURCHASESINSTALLMENTSFREQUENCY : How frequently purchases in installments are being done (1 = frequently done, 0 = not frequently done)

CASHADVANCEFREQUENCY : How frequently the cash in advance being paid

CASHADVANCETRX : Number of Transactions made with "Cash in Advanced"

PURCHASES_TRX : Numbe of purchase transactions made

CREDIT_LIMIT : Limit of Credit Card for user

PAYMENTS : Amount of Payment done by user

MINIMUM_PAYMENTS : Minimum amount of payments made by user

PRCFULLPAYMENT : Percent of full payment paid by user

TENURE : Tenure of credit card service for user


## Models

The following machine learning models are used in this project:

- PCA
- K-means
- DBSCAN
- Hierarchical Clustering

Each model's performance is evaluated using the following metrics:

- Davies-Bouldin Index
- Silhouette Score
- Calinski-Harabasz Index

## Usage

To run the project, execute the Jupyter notebook `Customer segmentation.ipynb`.

## Results

We can infer the following insights about each customer segment by grouping customer data into three distinct clusters, based on the mean values and using the best model:

**Cluster 1:**

Lower Balance: Customers have the lowest average balance compared to the other clusters.

Moderate Purchasing Behavior: Their purchases are moderate, both in terms of one-off and installment purchases.

Lower Credit Limit: They have the lowest average credit limit, which could be indicative of lower creditworthiness or a newer customer base.

Higher Full Payment Rate: The proportion of full payment is higher, suggesting these customers may be more conscientious about paying off balances.

**Cluster 2:**

High Balance and Credit Limit: These customers have a high average balance and the highest credit limit, indicating they are likely more affluent or trusted customers.
High Purchase Activity: This segment shows significantly higher one-off purchases, suggesting these customers may engage in larger, less frequent purchases.
High Payments: They make the highest payments on average, which is consistent with their high credit limit and high balance.
Moderate to High Purchasing Frequency: Purchase frequency is moderate to high, with a particular affinity for installment purchases, implying comfort with regular, possibly planned spending.

**Cluster 3:**

Moderate Balance with Lower Cash Advances: Customers have a moderate balance and take the least cash advances, suggesting they may use their credit card more judiciously.
Lowest Purchase Activity: This group has the lowest average for both one-off and installment purchases, which could suggest a more savings-oriented mindset or a preference for using other payment methods.
Moderate Credit Limit: Their credit limit is higher than Cluster 1 but significantly lower than Cluster 2, indicating a middle-ground in terms of creditworthiness.
Lowest Full Payment Rate: They have the lowest rate of full payments, which may indicate a tendency to carry a balance or potentially struggle with full payments.

**General Observations:**

Tenure: All clusters have a similar average tenure, suggesting that the length of time as a customer may not be a distinguishing factor in their credit card usage behaviors.

Cash Advance Usage: Cluster 1 and Cluster 2 take more cash advances than Cluster 3, yet Cluster 2 seems to have a much higher frequency of cash advances. This could correlate with their high balance and credit limits, indicating that they may be using cash advances in a strategic financial manner.

Payment Behavior: Clusters 1 and 2 have higher payments relative to their balances, which might suggest better financial health or a more aggressive payment strategy to avoid interest.

**Caution:**

It is important to note that these insights are purely based on averages and do not account for the distribution within each cluster. Outliers or varying distributions can significantly affect the interpretation.

