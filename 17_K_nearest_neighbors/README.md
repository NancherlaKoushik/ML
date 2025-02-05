# K-Nearest Neighbors (KNN) Implementation

This notebook demonstrates the implementation of the K-Nearest Neighbors (KNN) algorithm using the Iris dataset. The goal is to classify iris flowers based on their features using KNN and evaluate its performance.

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

1. Loaded the Iris dataset using `sklearn.datasets`.
2. Created a DataFrame to visualize the features and target variable.
3. Explored the dataset to understand its structure and dimensions.

## KNN Model Implementation

### 1. Model Training

- Used `KNeighborsClassifier` from `sklearn.neighbors`.
- Set the number of neighbors (`n_neighbors`) to 5.
- Trained the model on the training dataset.

### 2. Model Evaluation

- Evaluated the model's performance on the test dataset.
- Achieved an accuracy score of 1.0, indicating perfect classification on the test set.

### 3. Confusion Matrix

- Generated a confusion matrix to visualize the performance of the model.
- Used a heatmap to represent the confusion matrix, showing true vs. predicted classifications.

### 4. Classification Report

- Generated a classification report that includes precision, recall, and F1-score for each class.
- The model achieved perfect scores across all metrics, indicating excellent performance.

## Key Findings

1. The KNN algorithm performed exceptionally well on the Iris dataset, achieving 100% accuracy.
2. The confusion matrix and classification report confirmed the model's effectiveness in classifying the iris flower species.

## Dependencies

- numpy
- pandas
- scikit-learn
- matplotlib
- seaborn

## Usage

The notebook can be run sequentially to understand the implementation of the K-Nearest Neighbors algorithm and its application to the Iris dataset. It provides insights into model training, evaluation, and performance metrics.
