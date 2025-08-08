# titanic-survival-prediction
Titanic ML project using logistic regression.
# Titanic Survival Prediction

Predict survival on the Titanic using a machine learning classification model. This project demonstrates how to clean data, train a logistic regression model, and evaluate its performance.

![Titanic](https://upload.wikimedia.org/wikipedia/commons/f/fd/RMS_Titanic_3.jpg)

---

## Overview

This beginner-friendly machine learning project solves a binary classification problem — predicting which passengers survived the Titanic disaster using demographic and ticket data.

The model was trained using **Logistic Regression** with performance evaluated on a validation set. The final results are prepared for Kaggle submission.

---

## echnologies Used

- Python 3.x  
- pandas, numpy  
- matplotlib, seaborn  
- scikit-learn  
- Google Colab

---

## Dataset

Dataset from the [Kaggle Titanic Competition](https://www.kaggle.com/competitions/titanic):

- `train.csv` — Training data (used to build model)  
- `test.csv` — Test data (used for prediction submission)  
- `gender_submission.csv` — Optional sample submission

> *Note: Do not push raw data files to public GitHub repos.*

---

## Preprocessing

- Filled missing values in `Age`, `Fare`, `Embarked`
- Categorical encoding for `Sex`, `Embarked`
- Dropped irrelevant features: `Name`, `Ticket`, `Cabin`, `PassengerId`
- Normalized feature selection for modeling

---

## Features Used

| Feature        | Description                        |
|----------------|------------------------------------|
| Pclass         | Ticket class (1 = 1st, 2 = 2nd...) |
| Sex            | Gender (0 = male, 1 = female)      |
| Age            | Age in years                       |
| SibSp          | # of siblings/spouses aboard       |
| Parch          | # of parents/children aboard       |
| Fare           | Passenger fare                     |
| Embarked       | Port of embarkation (0=S, 1=C, 2=Q) |

---

## Model

- Algorithm: **Logistic Regression** (`sklearn.linear_model`)
- Split: 80% train / 20% validation
- Metrics:
  - Accuracy: ~80%
  - Confusion Matrix
  - Precision, Recall, F1 Score

### Sample Output

