# Customer Churn Prediction Project

## Overview

This project focuses on predicting customer churn using a telecom dataset of over 7,000 customer records. The objective is to identify customers who are likely to leave the service so that businesses can take preventive action.

Customer churn prediction is important because retaining existing customers is more cost-effective than acquiring new ones.


## Dataset

The dataset used is the Telco Customer Churn dataset, which contains:

* Customer tenure
* Monthly charges
* Total charges
* Contract type
* Internet service
* Payment method
* Churn label (Target Variable)

Target Variable:

* 0 = Customer Stayed
* 1 = Customer Churned


## Project Workflow

### 1. Data Cleaning

* Removed irrelevant columns (customerID)
* Converted TotalCharges to numeric
* Handled missing values

### 2. Exploratory Data Analysis (EDA)

Performed visualization to understand:

* Churn distribution (class imbalance)
* Tenure vs churn relationship
* Monthly charges impact on churn
* Feature correlations

### 3. Feature Engineering

* Created a new feature: AvgChargePerMonth
  This helps capture customer spending behavior more effectively.

### 4. Handling Class Imbalance

* Applied SMOTE (Synthetic Minority Oversampling Technique)
  This balanced the minority churn class.

### 5. Model Training

* Trained an XGBoost classifier
* Compared performance using classification metrics

### 6. Model Evaluation

Evaluation metrics used:

* Precision
* Recall
* F1-Score
* ROC-AUC Score

Final AUC Score: ~0.85–0.89


## Key Insights

* Customers with shorter tenure are more likely to churn
* Higher monthly charges increase churn probability
* Contract type plays a significant role

## Technologies Used

* Python
* Pandas
* NumPy
* Seaborn & Matplotlib
* Scikit-learn
* XGBoost
* SMOTE (Imbalanced-Learn)

## Conclusion

This project demonstrates a complete end-to-end machine learning pipeline including:

* Data preprocessing
* Feature engineering
* Handling class imbalance
* Model training
* Performance evaluation

The solution can help telecom companies proactively identify at-risk customers and improve retention strategies.


## Author

Arshiyan Elahi
Computer Engineering | AI & Data Science
