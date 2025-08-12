# Project Overview
This project applies supervised and unsupervised machine learning techniques to analyze customer data from a streaming service. The primary goals are to predict customer spending patterns, determine customer churn, and identify distinct customer clusters to help inform business strategies.

# Methodology
The analysis followed these key steps:
Data Cleaning: Handled missing values in the dataset by filling them with the median age and replacing null Satisfaction_Score values with "0".

## Regression Analysis:
Simple Linear Regression: Compared single numerical features to predict Monthly_Spend.
Multiple Linear Regression: Used multiple numerical features to improve the prediction accuracy of Monthly_Spend.
Random Forest Regressor: Incorporated both numerical and categorical features (Gender, Region, Payment_Method) to predict Monthly_Spend.

## Churn Prediction (Classification):
Trained and evaluated several classification models to predict whether a customer would churn (1) or not churn (0).
Models included K-Nearest Neighbors, Decision Tree, Random Forest, and an Artificial Neural Network (ANN).

## Customer Segmentation (Clustering):
Applied unsupervised learning algorithms, including k-Means and Hierarchical Clustering, to identify patterns in customer behavior.

## Key Findings & Results
_Predicting Monthly Spending_
The Random Forest Regressor model provided the best performance for predicting Monthly_Spend. Its metrics were significantly better than the other models, demonstrating the value of including multiple and categorical features.
_Churn Prediction_
The Decision Tree and Random Forest models were the most effective for predicting customer churn.

The high ROC-AUC score for both models confirms their ability to accurately distinguish between customers who churn and those who do not.

## Customer Segmentation
Using the Elbow Method, the optimal number of clusters for the dataset was determined to be 6. The k-Means algorithm provided a better segmentation of customer behavior compared to Hierarchical Clustering.

# Technologies Used
- Python: The core programming language for the project.
- Pandas: Used for data manipulation and cleaning.
- NumPy: Essential for numerical operations.
- Scikit-learn: Key library for implementing regression, classification, and clustering algorithms.
- Keras/TensorFlow: Used to build and train the Artificial Neural Network (ANN) model.
- Matplotlib/Seaborn: For data visualization and plotting the results.
