# K-Fold Cross Validation Implementation

This notebook demonstrates the implementation of K-Fold Cross Validation using the Digits dataset. The goal is to compare the performance of different machine learning algorithms and evaluate their robustness using cross-validation techniques.

## Dataset Overview

- The Digits dataset is a classic dataset in machine learning.
- It contains images of handwritten digits (0-9).
- Each image is represented as a feature vector of length 64 (8x8 pixel values).
- The target variable consists of digit labels (0-9).

## Models Implemented

The notebook compares three different classification algorithms:

1. **Logistic Regression**
2. **Support Vector Machine (SVM)**
3. **Random Forest Classifier**

## K-Fold Cross Validation Implementation

### 1. Initial Model Evaluation

- Split the dataset into training and testing sets.
- Trained each model on the training data.
- Evaluated performance on the test data.

### 2. K-Fold Cross Validation

- Implemented K-Fold Cross Validation with 3 splits.
- Applied cross-validation to all three models.
- Calculated and compared mean accuracy scores across folds.

### 3. Using scikit-learn's cross_val_score

- Demonstrated the use of scikit-learn's built-in `cross_val_score` function.
- Simplified the cross-validation process.
- Compared results with manual implementation.

## Key Findings

1. Cross-validation provides a more robust evaluation of model performance than a single train-test split.
2. The performance of models can vary across different folds, highlighting the importance of cross-validation.
3. All three models show good performance on the Digits dataset, with slight variations in accuracy.

## Dependencies

- numpy
- scikit-learn

## Usage

The notebook can be run sequentially to understand the implementation of K-Fold Cross Validation and its application to model evaluation. It provides insights into how cross-validation helps in assessing model performance more reliably.