# Naive Bayes Classifier Implementation

This notebook demonstrates the implementation of the Naive Bayes Classifier using the Titanic dataset. The goal is to classify passengers as either "survived" or "not survived" based on various features using the Gaussian Naive Bayes algorithm.

## Dataset Overview

- The Titanic dataset contains information about the passengers aboard the Titanic.
- It consists of various features, including:
  - PassengerId
  - Name
  - Pclass (Passenger Class)
  - Sex
  - Age
  - SibSp (Number of Siblings/Spouses Aboard)
  - Parch (Number of Parents/Children Aboard)
  - Ticket
  - Fare
  - Cabin
  - Embarked (Port of Embarkation)
  - Survived (Target Variable)

## Data Preprocessing Steps

1. **Data Loading**: Loaded the dataset into a DataFrame.
2. **Data Exploration**: Explored the dataset to understand its structure and summary statistics.
3. **Missing Values Check**: Checked for any missing values in the dataset.
4. **Feature and Target Separation**: Separated the features (X) from the target variable (y).
5. **Encoding Categorical Variables**: Converted categorical variables into numerical format for model training.

## Naive Bayes Model Implementation

### 1. Feature Extraction

- Used `CountVectorizer` from `sklearn.feature_extraction.text` to convert the text messages into a matrix of token counts.

### 2. Model Training

- Implemented the Gaussian Naive Bayes classifier using `GaussianNB` from `sklearn.naive_bayes`.
- Trained the model on the training dataset.

### 3. Model Evaluation

- Evaluated the model's performance on the test dataset.
- Achieved an accuracy score of approximately 80.45%, indicating good classification performance.

### 4. Predictions

- Tested the model with new passenger data to classify them as survived or not survived.
- The model successfully predicted the category of the test passengers.

## Key Findings

1. The Naive Bayes classifier performed well on the Titanic dataset, achieving an accuracy of 80.45%.
2. The model effectively distinguishes between survived and not survived passengers based on the features extracted from the dataset.

## Dependencies

- numpy
- pandas
- scikit-learn

## Usage

The notebook can be run sequentially to understand the implementation of the Naive Bayes Classifier and its application to the Titanic dataset. It provides insights into data preprocessing, model training, evaluation, and prediction.
