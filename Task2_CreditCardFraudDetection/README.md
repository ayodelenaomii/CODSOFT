# Task2_CreditCardFraudDetection.

---

# Fraud Detection in Financial

This project aims to predict fraudulent transactions using a dataset containing transaction details. The model classifies transactions as either fraudulent or non-fraudulent based on multiple features, including transaction amount, category, customer location, and time of transaction.

## Dataset Overview

The dataset consists of over 1.2 million records with the following columns:

- **category**: Transaction category
- **amt**: Transaction amount
- **city_pop**: Population of the city where the transaction occurred
- **merch_lat**: Latitude of the merchant's location
- **merch_long**: Longitude of the merchant's location
- **is_fraud**: Target variable indicating whether the transaction is fraudulent (1) or not (0)
- **year**: Year of the transaction
- **month**: Month of the transaction
- **day**: Day of the transaction
- **hour**: Hour of the transaction
- **minute**: Minute of the transaction
- **weekday**: Weekday of the transaction
- **amt_bin_encoded**: Binned transaction amount for encoding

The dataset has been preprocessed, and features have been encoded for model training. The training set consists of 1,292,739 entries, while the test set contains 554,136 entries.

## Features and Target Variables

- **Features**: 
  - 12 input features such as `category`, `amt`, `city_pop`, `merch_lat`, `merch_long`, etc.
- **Target**: 
  - `is_fraud`: A binary variable indicating whether the transaction is fraudulent (1) or not (0).

## Data Preprocessing

- The dataset has been cleaned, with no missing values.
- Features like `amt` have been binarized into `amt_bin_encoded` for encoding purposes.

## Model: Random Forest

The model used for classification is a **Random Forest** classifier. Random Forest is an ensemble learning method that creates multiple decision trees and merges them together to get a more accurate and stable prediction.

### Model Performance

The model was trained using the Random Forest algorithm and evaluated on the test set. The results are summarized below:

- **ROC AUC**: 0.987
- **Accuracy**: 99.84%
- **Classification Report**: 
  - **Class 0 (Non-Fraudulent)**:
    - Precision: 99.87%
    - Recall: 99.98%
    - F1-Score: 99.92%
  - **Class 1 (Fraudulent)**:
    - Precision: 89.49%
    - Recall: 60.62%
    - F1-Score: 72.28%

The model shows excellent performance in detecting non-fraudulent transactions and reasonable performance for fraudulent transactions.
