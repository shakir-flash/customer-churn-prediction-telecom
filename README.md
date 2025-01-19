# Customer Churn Prediction

This repository contains the code and methodology for predicting customer churn using various machine learning models. The project aims to identify churn drivers and optimize prediction accuracy through data preprocessing, feature engineering, model training, and hyperparameter tuning.

## Table of Contents
1. [Project Overview](#project-overview)
2. [Data Preprocessing](#data-preprocessing)
3. [Feature Engineering](#feature-engineering)
4. [Model Training](#model-training)
5. [Hyperparameter Tuning](#hyperparameter-tuning)
6. [Results](#results)
7. [Key Findings](#key-findings)
8. [How to Run](#how-to-run)
9. [Requirements](#requirements)

---

## Project Overview

Customer churn prediction is crucial for businesses to retain customers and reduce operational costs. This project employs supervised machine learning models to predict whether a customer is likely to churn, based on historical and demographic data.

---

## Data Preprocessing

The dataset underwent:
- **Cleaning**: Handling missing values and outliers.
- **Encoding**: Converting categorical variables to numerical format.
- **Scaling**: Normalizing continuous features to improve model performance.
- **Splitting**: Dividing the dataset into training (80%) and testing (20%) sets.

---

## Feature Engineering

Feature engineering steps included:
- Removing irrelevant or highly correlated features.
- Creating new features to capture potential churn drivers.
- Using correlation matrices and domain knowledge to refine feature selection.

---

## Model Training

The following models were trained and evaluated:
1. Logistic Regression
2. Decision Tree
3. Random Forest
4. Support Vector Machine (SVM)
5. XGBoost

Performance metrics:
- Accuracy
- ROC-AUC Score

---

## Hyperparameter Tuning

RandomizedSearchCV was used to optimize hyperparameters for each model:
- **Logistic Regression**: Best parameters - `C=0.014, penalty='l2', solver='lbfgs'`
- **Decision Tree**: Best parameters - `max_depth=5, min_samples_leaf=2, min_samples_split=13`
- **Random Forest**: Best parameters - `max_depth=7, n_estimators=180, min_samples_split=9, min_samples_leaf=1`
- **SVM**: Best parameters - `C=0.064, gamma=0.048, kernel='rbf'`
- **XGBoost**: Best parameters - `colsample_bytree=0.508, learning_rate=0.071, max_depth=5, n_estimators=252, subsample=0.304`

---

## Results

### Model Performance
| Model               | Accuracy (%) | ROC-AUC Score |
|---------------------|--------------|---------------|
| Logistic Regression | 80           | 0.831         |
| Decision Tree       | 80           | 0.643         |
| Random Forest       | 80           | 0.784         |
| SVM                 | 80           | 0.783         |
| XGBoost             | 80           | 0.806         |

### Key Observations:
- Logistic Regression provided consistent results, with minimal gains from hyperparameter tuning.
- Random Forest and XGBoost achieved competitive performance, showing robustness with fine-tuned parameters.

---

## How to Run

1. Clone this repository:
   ```bash
   git clone https://github.com/shakir-flash/customer-churn-prediction-telecom.git
   ```
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Run the Jupyter Notebook to explore the code and results.

---

## Requirements

- Python 3.8+
- Libraries: `numpy`, `pandas`, `matplotlib`, `seaborn`, `scikit-learn`, `xgboost`, `scipy`

---

## Key Findings

- Hyperparameter tuning significantly improved Decision Tree and Random Forest performance, highlighting the importance of parameter optimization.
- Churn prediction can be efficiently achieved with interpretable models like Logistic Regression or more complex ensembles like XGBoost.

Feel free to contribute, suggest improvements, or raise issues. Together, let's refine churn prediction models and deliver impactful solutions!

---
