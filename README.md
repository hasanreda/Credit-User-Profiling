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

The dataset comprises 10,695 records and consists of 10 columns. Unfortunately, the features lack detailed descriptions as provided by the data source.

Feature Variables:

    Discrete Features: Age, Work_Experience, Family_Size

    Boolean Features: Gender, Ever_Married, Graduated

    Nominal Features: Profession, Var_1

    Ordinal Features: Spending_Score

Target Label:

    Segmentation


## Models

The following machine learning models are used in this project:

- Logistic Regression
- Decision Tree
- K-Nearest Neighbors (KNN)
- XGBoost

Each model's performance is evaluated using the following metrics:

- Accuracy
- Precision
- Recall
- F1 Score

## Usage

To run the project, execute the Jupyter notebook `Customer segmentation.ipynb`.

## Results

The performance of each model is stored in a pandas DataFrame `df_models`. This DataFrame contains the accuracy, precision, recall, and F1 score for each model.

Based on the error metrics calculated for each model, it appears that none of the four models achieved an accuracy score higher than 50%, although it is much better than a coin flip, which would be of 25% accuracy, This could be due to a number of factors, such as the size and quality of the dataset, the complexity of the problem being solved, or the choice of features and hyperparameters used in each model.

XGBoost performed the best among the models, with the highest accuracy, precision, recall, and F1 score. Therefore, XGBoost would be the recommended model to use for now. It is important to note that further iterations and refinements may be necessary to improve the performance of the models.

## Dependencies

This project requires the following Python libraries:

- pandas
- sklearn
- xgboost

