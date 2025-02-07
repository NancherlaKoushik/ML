# Ensemble Learning Implementation

This notebook demonstrates the implementation of Ensemble Learning techniques using the Diabetes dataset. The goal is to compare the performance of different ensemble methods, specifically Bagging and Random Forest classifiers, in predicting diabetes outcomes.

## Dataset Overview

- The Diabetes dataset contains various health-related features used to predict whether a patient has diabetes.
- It consists of 768 samples with the following features:
  - Pregnancies
  - Glucose
  - Blood Pressure
  - Skin Thickness
  - Insulin
  - BMI
  - Diabetes Pedigree Function
  - Age
  - Outcome (target variable)

## Data Preprocessing Steps

1. **Data Loading**: Loaded the dataset into a DataFrame.
2. **Data Exploration**: Explored the dataset to understand its structure and summary statistics.
3. **Missing Values Check**: Checked for any missing values in the dataset.
4. **Feature and Target Separation**: Separated the features (X) from the target variable (y).

## Ensemble Learning Implementation

### 1. Data Standardization

- Used `StandardScaler` from `sklearn.preprocessing` to standardize the features by removing the mean and scaling to unit variance.

### 2. Train-Test Split

- Split the dataset into training and testing sets (80% training, 20% testing) while maintaining the distribution of the target variable.

### 3. Decision Tree Classifier

- Implemented a Decision Tree Classifier and evaluated its performance using cross-validation.
- Achieved a mean accuracy score of approximately 71.10%.

### 4. Bagging Classifier

- Implemented a Bagging Classifier using a Decision Tree as the base estimator.
- Trained the model and evaluated its out-of-bag score and test score.
- Achieved an out-of-bag score of approximately 80.52% and a test score of approximately 80.52%.

### 5. Random Forest Classifier

- Implemented a Random Forest Classifier and evaluated its performance using cross-validation.
- Achieved a mean accuracy score of approximately 75.79%.

## Key Findings

1. The Bagging Classifier significantly improved the model's performance compared to the base Decision Tree Classifier.
2. The Random Forest Classifier also provided a good performance, but the Bagging Classifier outperformed it in this case.
3. Ensemble methods like Bagging and Random Forest are effective in improving model accuracy and robustness.

## Dependencies

- numpy
- pandas
- scikit-learn

## Usage

The notebook can be run sequentially to understand the implementation of Ensemble Learning techniques and their application to the Diabetes dataset. It provides insights into data preprocessing, model training, evaluation, and performance comparison of different ensemble methods.
