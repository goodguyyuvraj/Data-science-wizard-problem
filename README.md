# Loan default Prediction Pipeline

## Overview

This project implements a machine learning pipeline for predicting loan status using two popular models: Random Forest and XGBoost. The code processes loan-related data, trains models, evaluates performance, and applies hyperparameter tuning techniques to improve model accuracy.

## Key Features

1. **Data Loading:**

   - Training and testing datasets are loaded from Excel files.

2. **Preprocessing:**

   - Feature engineering: Extracts `transaction_year` and `transaction_month` from `transaction_date`.
   - Encodes categorical variables using `LabelEncoder`.
   - Scales numerical features with `StandardScaler`.

3. **Model Implementation:**

   - **Random Forest Model:**
     - Uses a balanced class weight to handle imbalanced data.
   - **XGBoost Model:**
     - Supports advanced tree-based learning and allows hyperparameter tuning.

4. **Model Training and Testing:**

   - Train models using `fit()` method.
   - Evaluate performance using `classification_report` and `confusion_matrix`.

5. **Hyperparameter Tuning:**

   - **GridSearchCV:** Systematic tuning of XGBoost hyperparameters.
   - **RandomizedSearchCV:** Efficient sampling of XGBoost hyperparameter combinations for optimization.

## Pipeline Usage

- **Random Forest Model:**

  - Loads and preprocesses data.
  - Trains and evaluates the model.

- **XGBoost Model:**

  - Includes additional hyperparameter tuning using both Grid Search and Randomized Search.

## Conclusion

**The tuned XGBoost model achieves similar accuracy but higher recall compared to the default XGBoost model, making it the preferred choice for this problem.**

