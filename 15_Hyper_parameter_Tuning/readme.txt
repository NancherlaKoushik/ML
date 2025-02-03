# Hyperparameter Tuning with Scikit-learn

This notebook demonstrates hyperparameter tuning techniques using Scikit-learn on the Iris dataset. The example shows how to optimize Support Vector Machine (SVM) classifier parameters using different methods.

## Overview

The code covers:
1. Loading and preparing the Iris dataset
2. Basic SVM model training
3. Cross-validation with different parameters
4. Grid Search CV
5. Random Search CV

## Dataset
The code uses the famous Iris dataset which includes:
- 150 samples
- 4 features (sepal length, sepal width, petal length, petal width)
- 3 target classes (setosa, versicolor, virginica)

## Methods Demonstrated

### 1. Basic SVM Model
- Initial SVM model with manual parameters (kernel='rbf', C=30)
- Simple train-test split evaluation

### 2. Manual Cross-validation
- Testing different combinations of:
  - Kernels: ['rbf', 'linear']
  - C values: [1, 10, 20]
- Using cross_val_score for more robust evaluation

### 3. Grid Search CV
Systematic grid search through parameters:
- Parameters tested:
  - kernel: ['rbf', 'linear']
  - C: [1, 10, 20]
- Uses 5-fold cross-validation
- Provides detailed results including:
  - Mean fit time
  - Mean score time
  - Test scores for each split
  - Mean test scores
  - Rank of parameter combinations

### 4. Random Search CV
- Similar to Grid Search but randomly samples parameter combinations
- Tests fewer combinations (n_iter=2)
- Faster alternative when parameter space is large

## Key Results

The Grid Search results showed:
- Best parameters: {'C': 1, 'kernel': 'rbf'}
- Best score: 0.98 (98% accuracy)
- Multiple parameter combinations achieved similar performance:
  - C=1 with both rbf and linear kernels
  - C=10 with rbf kernel

## Dependencies
- pandas
- numpy
- scikit-learn

## Usage
The notebook can be run sequentially to understand each step of the hyperparameter tuning process. Each section builds upon the previous ones to show different approaches to parameter optimization.

This example serves as a practical guide for implementing hyperparameter tuning in machine learning models using scikit-learn's various search methods.