# Support Vector Machine (SVM) Implementation

This notebook demonstrates the implementation of Support Vector Machine (SVM) using the Iris dataset. The goal is to classify iris flowers into different species based on their features using the SVM algorithm.

## Dataset Overview

- The Iris dataset is a classic dataset in machine learning.
- It contains 150 samples of iris flowers, with 4 features:
  - Sepal length (cm)
  - Sepal width (cm)
  - Petal length (cm)
  - Petal width (cm)
- The target variable consists of three classes of iris flowers:
  - Setosa
  - Versicolor
  - Virginica

## Data Preprocessing Steps

1. **Data Loading**: Loaded the Iris dataset using `sklearn.datasets`.
2. **Data Exploration**: Created a DataFrame to visualize the features and target variable.
3. **Feature Visualization**: Plotted different feature combinations to understand the data distribution.
4. **Train-Test Split**: Split the dataset into training and testing sets for model evaluation.

## SVM Model Implementation

### 1. Model Training

- Used `SVC` from `sklearn.svm` with a linear kernel.
- Trained the model on the training dataset.

### 2. Model Evaluation

- Evaluated the model's performance on the test dataset.
- Calculated the accuracy score to measure classification performance.

## Key Findings

1. The SVM classifier performs well on the Iris dataset, achieving high accuracy.
2. The model effectively distinguishes between different iris species based on their features.
3. Visualization of feature combinations shows clear separation between classes, especially for the setosa species.

## Dependencies

- numpy
- pandas
- scikit-learn
- matplotlib

## Usage

The notebook can be run sequentially to understand the implementation of Support Vector Machine and its application to the Iris dataset. It provides insights into data preprocessing, model training, evaluation, and visualization of results.