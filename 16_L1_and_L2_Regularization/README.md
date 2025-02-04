# L1 and L2 Regularization Implementation

This notebook demonstrates the implementation of L1 (Lasso) and L2 (Ridge) regularization techniques using the Melbourne Housing dataset. The goal is to compare different regression models and understand how regularization affects model performance.

## Dataset Overview

- Using the Melbourne Housing dataset
- Contains features like Suburb, Rooms, Type, Price, etc.
- Original dataset has 34,857 rows and 21 columns
- Target variable: House Price

## Data Preprocessing Steps

1. Selected relevant features for analysis
2. Handled missing values:
   - Filled numeric columns (Propertycount, Distance, Bedroom2, Bathroom, Car) with 0
   - Filled Landsize and BuildingArea with mean values
   - Removed remaining rows with missing values
3. Performed one-hot encoding on categorical variables

## Models Implemented

### 1. Linear Regression (Base Model)

- Train Score: 0.685
- Test Score: 0.676

### 2. Lasso Regression (L1 Regularization)

Parameters:

- alpha = 50
- max_iterations = 100
- tolerance = 0.1

Performance:

- Train Score: 0.681
- Test Score: 0.680

### 3. Ridge Regression (L2 Regularization)

Parameters:

- alpha = 50
- max_iterations = 100
- tolerance = 0.1

Performance:

- Train Score: 0.669
- Test Score: 0.669

## Key Findings

1. All three models show similar performance, with scores ranging between 0.67-0.68
2. Lasso regression slightly outperformed both Linear and Ridge regression
3. Ridge regression shows identical train and test scores, indicating good generalization
4. The regularization helped in reducing overfitting, as seen in the closer train and test scores compared to the base model

## Dependencies

- numpy
- pandas
- scikit-learn
- matplotlib
- seaborn

## Usage

The notebook can be run sequentially to understand the implementation of L1 and L2 regularization techniques and their effects on model performance.
