# Customer Churn Prediction Using Machine Learning
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/MadishettiSwapna/Customer-Churn-Prediction/blob/main/Customer_Churn_Prediction.ipynb)
## Overview

Customer churn is a critical business problem in the telecommunications industry, as retaining existing customers is often more cost-effective than acquiring new ones. This project aims to predict customer churn using machine learning techniques and identify the key factors influencing customer retention.

The project follows a complete machine learning workflow, including data preprocessing, handling class imbalance, model building, evaluation, and business insight generation.

---

## Problem Statement

The objective of this project is to develop a machine learning model that can predict whether a customer is likely to leave a telecom service provider based on customer demographics, account information, and service usage patterns.

Accurate churn prediction enables businesses to identify at-risk customers and implement targeted retention strategies to reduce customer loss and improve customer satisfaction.

---

## Dataset

**Dataset:** Telco Customer Churn Dataset
**Source:** https://www.kaggle.com/datasets/blastchar/telco-customer-churn
The dataset contains customer information such as:

* Demographic details
* Subscription information
* Contract type
* Billing details
* Service usage patterns
* Churn status

**Target Variable:**

* Churn (Yes / No)

---

## Technologies Used

### Programming Language

* Python

### Libraries & Frameworks

* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn
* XGBoost
* Imbalanced-learn (SMOTE)
* Joblib

---

## Machine Learning Workflow

### 1. Data Preprocessing

* Data Cleaning
* Missing Value Handling
* Label Encoding
* Feature Scaling using MinMaxScaler

### 2. Exploratory Data Analysis (EDA)

* Churn Distribution Analysis
* Customer Behavior Analysis
* Service Usage Analysis

### 3. Handling Class Imbalance

* Applied SMOTE (Synthetic Minority Oversampling Technique) to balance churn classes.

### 4. Model Development

The following models were trained and evaluated:

* Logistic Regression
* Logistic Regression + SMOTE
* Random Forest + SMOTE
* XGBoost + SMOTE

### 5. Model Evaluation

Models were evaluated using:

* Accuracy
* Precision
* Recall
* F1-Score
* Confusion Matrix

---

## Model Performance

| Model                       | Accuracy | Recall | F1-Score |
| --------------------------- | -------- | ------ | -------- |
| Logistic Regression         | 80.9%    | 57%    | 0.59     |
| Logistic Regression + SMOTE | 75.4%    | 82%    | 0.62     |
| Random Forest + SMOTE       | 78.8%    | 62%    | 0.59     |
| XGBoost + SMOTE             | 79.0%    | 65%    | 0.61     |

---

## Final Model Selection

**Selected Model:** XGBoost + SMOTE

### Why XGBoost?

* Achieved the best balance between accuracy and churn detection.
* Produced the highest F1-Score among the evaluated ensemble models.
* Demonstrated strong predictive performance on imbalanced data.

### Final Performance

* Accuracy: 79.0%
* Recall: 65%
* F1-Score: 0.61

---

## Feature Importance Analysis

Feature importance analysis identified the following factors as the most influential predictors of customer churn:

1. Contract
2. Tenure
3. Monthly Charges
4. Total Charges
5. Payment Method
6. Online Security
7. Tech Support

---

## Key Business Insights

* Contract type is the strongest predictor of customer churn.
* Customers with shorter tenure are more likely to leave the company.
* Higher monthly charges increase churn probability.
* Customers using Online Security and Tech Support services tend to have lower churn rates.
* Retention efforts should focus on new customers and customers with unstable contract plans.

---

## Project Outcomes

This project successfully demonstrates:

* End-to-End Machine Learning Workflow
* Data Preprocessing and Feature Engineering
* Class Imbalance Handling using SMOTE
* Model Comparison and Selection
* Ensemble Learning Techniques
* Feature Importance Analysis
* Business Insight Generation

The developed solution can help telecom companies proactively identify customers at risk of churning and implement data-driven retention strategies.

---

## Future Improvements

* Hyperparameter Tuning using GridSearchCV
* Deployment using Streamlit or Flask
* Real-Time Churn Prediction System
* Deep Learning Approaches using TensorFlow or PyTorch

---

## Author

**Madishetti Swapna**

* LinkedIn: [https://www.linkedin.com/in/madishettiswapna/]
