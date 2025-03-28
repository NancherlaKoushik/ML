# Decision Tree Classifier Implementation

This notebook demonstrates the implementation of a Decision Tree Classifier using a salary prediction dataset. The goal is to predict whether an individual's salary is more than $100k based on company, job role, and education degree.

## Dataset Overview

- The dataset contains information about employees including:
  - Company name
  - Job role
  - Education degree
  - Target variable: Whether salary is more than $100k (binary)

## Data Preprocessing Steps

1. **Data Loading**: Loaded the salary dataset from 'salaries.csv'.
2. **Feature and Target Separation**: Separated the features from the target variable.
3. **Categorical Encoding**: Used LabelEncoder to convert categorical variables (company, job, degree) into numerical format.
4. **Feature Selection**: Created a new input dataset with only the encoded numerical features.

## Decision Tree Model Implementation

### 1. Model Training

- Used `DecisionTreeClassifier` from `sklearn.tree`.
- Trained the model on the preprocessed dataset.

### 2. Model Evaluation

- Evaluated the model's performance using the accuracy score.
- Demonstrated how to make predictions with new data points.

## Key Findings

1. The Decision Tree classifier effectively predicts salary ranges based on company, job, and education features.
2. The model demonstrates how categorical data can be processed for use in decision tree algorithms.
3. The implementation shows the simplicity and interpretability of decision tree models.

## Dependencies

- pandas
- scikit-learn

## Usage

The notebook can be run sequentially to understand the implementation of Decision Tree Classifier and its application to salary prediction. It provides insights into data preprocessing, categorical encoding, model training, and prediction.