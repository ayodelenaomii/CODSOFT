# Task1_MovieGenreClassification

## Overview

This project focuses on building a machine learning model to classify movies into one of 27 genres based on the dataset's features. The genres range from **Action** and **Comedy** to less common ones like **Western** and **Game-Show**. The model's performance has been evaluated using standard metrics such as precision, recall, F1-score, and ROC AUC score.

---

## Dataset Details

- **Number of Classes**: 27  
  Each genre is represented by a label, where:
  - `0` is Action  
  - `1` is Adult  
  - ...  
  - `26` is Western.
  
  Refer to the "Genre Labels" section below for the full mapping.

- **Imbalance in Classes**:  
  The dataset contains a significant imbalance, with some genres like **Drama** and **Documentary** being much more common than others like **War** and **Fantasy**. This impacts the model's overall performance, especially for underrepresented classes.

---

## Model Performance

### Key Metrics:
- **Accuracy**: 47.43%  
- **ROC AUC Score**: 0.8848  

### Detailed Classification Report:
The performance varies significantly across different genres. Here are a few highlights:
- **Comedy**: F1-score of 0.516, reflecting decent performance for a well-represented class.  
- **Documentary**: The model performs best here, achieving an F1-score of 0.676.  
- **Genres like Biography and Fantasy**: Struggle with F1-scores below 0.2 due to their lower representation in the dataset.

### Summary Metrics:
- **Macro Average**: Reflects the average performance across all genres, regardless of their class sizes.  
  - Precision: 30.7%  
  - Recall: 41.3%  
  - F1-score: 33.9%

- **Weighted Average**: Accounts for the imbalance by weighing performance by class size.  
  - Precision: 56.7%  
  - Recall: 47.4%  
  - F1-score: 50.3%

---

## Genre Labels

| Label | Genre          | Label | Genre         |
|-------|----------------|-------|---------------|
| 0     | Action         | 14    | Music         |
| 1     | Adult          | 15    | Musical       |
| 2     | Adventure      | 16    | Mystery       |
| 3     | Animation      | 17    | News          |
| 4     | Biography      | 18    | Reality-TV    |
| 5     | Comedy         | 19    | Romance       |
| 6     | Crime          | 20    | Sci-Fi        |
| 7     | Documentary    | 21    | Short         |
| 8     | Drama          | 22    | Sport         |
| 9     | Family         | 23    | Talk-Show     |
| 10    | Fantasy        | 24    | Thriller      |
| 11    | Game-Show      | 25    | War           |
| 12    | History        | 26    | Western       |
| 13    | Horror         |       |               |

---


## Observations and Next Steps

1. **Strengths**:  
   The model achieves decent results for well-represented genres like Comedy and Documentary.

2. **Weaknesses**:  
   Underrepresented genres like Fantasy and Biography show poor performance due to class imbalance.



