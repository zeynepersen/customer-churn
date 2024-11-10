# Telco Customer Churn Feature Engineering

## Overview

This project involves building a machine learning model that predicts which customers are likely to churn (leave the service) from a telecommunications company. The task is to first perform the necessary data analysis and feature engineering steps before developing the model.

The data represents information from a fictional telecommunications company that provides home phone and internet services to 7,043 customers in California during the third quarter. The dataset includes details about which customers have left, stayed, or signed up for services.

### Dataset Description
- **Number of observations**: 7,043
- **Number of features**: 21

### Features:

1. **CustomerId**: Unique ID for each customer.
2. **Gender**: Customer's gender.
3. **SeniorCitizen**: Whether the customer is a senior citizen (1 = Yes, 0 = No).
4. **Partner**: Whether the customer has a partner (Yes, No).
5. **Dependents**: Whether the customer has dependents (Yes, No) (e.g., children, elderly parents).
6. **tenure**: Number of months the customer has stayed with the company.
7. **PhoneService**: Whether the customer has phone service (Yes, No).
8. **MultipleLines**: Whether the customer has multiple phone lines (Yes, No, No Phone Service).
9. **InternetService**: Type of internet service the customer has (DSL, Fiber optic, No).
10. **OnlineSecurity**: Whether the customer has online security (Yes, No, No Internet Service).
11. **OnlineBackup**: Whether the customer has online backup (Yes, No, No Internet Service).
12. **DeviceProtection**: Whether the customer has device protection (Yes, No, No Internet Service).
13. **TechSupport**: Whether the customer receives technical support (Yes, No, No Internet Service).
14. **StreamingTV**: Whether the customer streams TV (Yes, No, No Internet Service).
15. **StreamingMovies**: Whether the customer streams movies (Yes, No, No Internet Service).
16. **Contract**: Customer’s contract term (Month-to-month, One year, Two years).
17. **PaperlessBilling**: Whether the customer has paperless billing (Yes, No).
18. **PaymentMethod**: Customer’s payment method (Electronic check, Mailed check, Bank transfer (automatic), Credit card (automatic)).
19. **MonthlyCharges**: Monthly charges billed to the customer.
20. **TotalCharges**: Total charges billed to the customer.
21. **Churn**: Whether the customer churned (Yes or No) — customers who left in the past month or quarter.

## Objective

Before developing a machine learning model, we aim to conduct the following tasks:

1. **Data Preprocessing**: Handling missing values, converting categorical variables into numeric representations, scaling numerical features, and handling outliers.
2. **Feature Engineering**: Creating new features from existing ones to improve model performance, such as tenure-related features, total charges per month, and interaction terms between various services and customer demographics.
3. **Exploratory Data Analysis (EDA)**: Understanding the distribution of the data, identifying trends, and visualizing relationships between features and the target variable (Churn).

## Approach

1. **Data Cleaning**: Handling missing data, removing duplicates, and encoding categorical variables like `Gender`, `Partner`, and `Contract`.
2. **Feature Creation**: Developing new features, such as monthly spending based on `TotalCharges` and `tenure`, and customer segmentation based on their contract and service usage.
3. **Correlation Analysis**: Identifying the features that are most correlated with churn and focusing on them for the model.
4. **Visualization**: Creating plots to visualize the relationships between variables, especially to understand churn patterns.
5. **Model Development**: After the feature engineering phase, a suitable machine learning model can be developed to predict customer churn.

## Requirements

- Python 3.x
- pandas
- numpy
- scikit-learn
- matplotlib
- seaborn

## Conclusion

By analyzing and transforming this dataset, we aim to build a machine learning model capable of predicting which customers are likely to leave the service, helping the company take proactive measures to retain customers.
