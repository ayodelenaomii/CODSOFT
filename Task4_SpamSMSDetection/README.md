
---

# SMS Spam Detection Project

## Overview

This project aims to build a machine learning model to classify SMS messages as either **spam** or **ham** (non-spam). Using a labeled dataset of SMS messages, the project focuses on preprocessing the text data and applying a Naive Bayes classifier to classify messages with high accuracy.

---

## Dataset

The dataset contains 5,572 SMS messages, each labeled with either spam or ham:
- **Label**: Represents whether the message is `spam` (1) or `ham` (0).
- **Message**: Contains the text of the SMS.

### Dataset Details:
- Total messages: 5,572
- Spam messages: Around 13.4%
- Ham messages: Around 86.6%
- Some irrelevant columns (`Unnamed: 2`, `Unnamed: 3`, `Unnamed: 4`) were excluded during preprocessing as they contained little useful information.

---

## Data Preprocessing

### The following preprocessing steps were performed:
1. **Data Cleaning**: 
   - Removed unnecessary columns and ensured the dataset had no missing values in the key fields (`Label` and `Message`).
2. **Text Normalization**: 
   - Converted all text to lowercase.
   - Tokenized the text and removed stopwords and non-alphanumeric characters.
3. **Feature Extraction**: 
   - Applied Bag-of-Words (BoW) and TF-IDF methods to convert text into numerical features.
4. **Data Splitting**: 
   - The dataset was split into training and testing sets (80% training, 20% testing).

---

## Model

The model used for classification is **Multinomial Naive Bayes**, which is particularly effective for text classification tasks involving discrete features such as word frequencies.

### Model Performance:
- **Accuracy**: 98%
- **Precision**: 
  - Ham: 98%
  - Spam: 100%
- **Recall**: 
  - Ham: 100%
  - Spam: 85%
- **F1-Score**: 
  - Ham: 99%
  - Spam: 92%

---

## Key Files

1. **`sms_spam_dataset.csv`**: The raw dataset containing SMS messages and their corresponding labels.
2. **`sms_spam_detection.ipynb`**: A Jupyter notebook that handles data preprocessing, model training, and evaluation.

---


## Results

The model achieved an impressive accuracy of 98%, demonstrating its ability to effectively distinguish between spam and legitimate messages. It shows particularly high precision for spam detection, with minimal false positives.

---


## Contributors

- **Naomi Ayodele**  
  Email: [ayodelenaomi88@gmail.com](mailto:ayodelenaomi88@gmail.com)  
  GitHub: [ayodelenaomii](https://github.com/ayodelenaomii/ayodelenaomii)

---

## Acknowledgments

The dataset used in this project is available for public use and is commonly used in text classification tasks. Thanks to all contributors who provide open data resources, enabling projects like this to move forward.

---
