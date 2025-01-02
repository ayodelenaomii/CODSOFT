# Task3_CustomerChurnPrediction

# Customer Churn Prediction

## Overview

This project aims to predict customer churn for a telecommunications company using various customer data features. The dataset consists of information such as the customer's geographical location, demographic details, and account attributes. By applying machine learning algorithms, the goal is to predict whether a customer will stay or leave (i.e., churn) based on the available features.

## Dataset

The dataset contains **10,000 customer records** with the following features:
- **CreditScore**: The credit score assigned to the customer.
- **Geography**: The country where the customer resides (France, Spain, Germany).
- **Gender**: The gender of the customer (Male/Female).
- **Age**: The customer's age.
- **Tenure**: The number of years the customer has been with the company.
- **Balance**: The balance in the customer's account.
- **NumOfProducts**: The number of products the customer has with the company.
- **HasCrCard**: Whether the customer has a credit card (1 for Yes, 0 for No).
- **IsActiveMember**: Whether the customer is an active member (1 for Yes, 0 for No).
- **EstimatedSalary**: The estimated salary of the customer.
- **Exited**: The target variable indicating whether the customer churned (1 for Yes, 0 for No).

### Example data:
| RowNumber | CustomerId | Surname  | CreditScore | Geography | Gender | Age | Tenure | Balance | NumOfProducts | HasCrCard | IsActiveMember | EstimatedSalary | Exited |
|-----------|------------|----------|-------------|-----------|--------|-----|--------|---------|---------------|-----------|----------------|-----------------|--------|
| 1         | 15634602   | Hargrave | 619         | France    | Female | 42  | 2      | 0.00    | 1             | 1         | 1              | 101348.88       | 1      |
| 2         | 15647311   | Hill     | 608         | Spain     | Female | 41  | 1      | 83807.86| 1             | 0         | 1              | 112542.58       | 0      |

### Data Information:
- Total Records: **10,000**
- Features: **11 columns** (including the target variable `Exited`)
- Missing Values: None (all values are complete)

---

## Preprocessing Steps

1. **Data Cleaning**:
   - Removed irrelevant columns (e.g., `RowNumber`, `CustomerId`, `Surname`).
   - Ensured no missing values were present.
   
2. **Feature Encoding**: **One-Hot Encoding** to convert them into numerical values.
   
3. **Feature Scaling**:
   - Normalized continuous features (e.g., `Age`, `CreditScore`, `Balance`) using **StandardScaler** to ensure all features contribute equally during model training.

---

## Model Training

 **Gradient Boosting**:
   - Accuracy: **87.0%**
   - Key Metrics: Slightly improved precision and recall compared to Random Forest.

### Performance Metrics for Gradient Boosting:
- **Precision (Class 0)**: 88%
- **Precision (Class 1)**: 79%
- **Recall (Class 0)**: 97%
- **Recall (Class 1)**: 49%
- **F1-Score (Class 0)**: 92%
- **F1-Score (Class 1)**: 60%

---


## Contributors

- **Naomi Ayodele**  
  GitHub: [ayodelenaomii](https://github.com/ayodelenaomii/ayodelenaomii)  
  Email: [ayodelenaomi88@gmail.com](mailto:ayodelenaomi88@gmail.com)

---

## Acknowledgments

Special thanks to the developers and contributors of open-source machine learning tools like **scikit-learn** and **pandas**, which were crucial in building and evaluating this model.

---

This README structure ensures that all key details about the project are clearly communicated, while avoiding plagiarism.
Description for Task3_CustomerChurnPrediction goes here.