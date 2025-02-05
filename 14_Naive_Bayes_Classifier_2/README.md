# Naive Bayes Classifier Implementation

This notebook demonstrates the implementation of the Naive Bayes Classifier using a dataset of SMS messages. The goal is to classify messages as either "ham" (not spam) or "spam" using the Multinomial Naive Bayes algorithm.

## Dataset Overview

- The dataset consists of SMS messages labeled as either "ham" or "spam".
- It contains a total of 5,572 messages, with the following categories:
  - **Ham**: 4,825 messages
  - **Spam**: 747 messages

## Data Preprocessing Steps

1. **Data Loading**: Loaded the dataset into a DataFrame.
2. **Data Exploration**: Used descriptive statistics to understand the distribution of messages in each category.
3. **Label Encoding**: Created a binary column (`spam`) where:
   - `1` indicates a spam message
   - `0` indicates a ham message
4. **Train-Test Split**: Split the dataset into training and testing sets (75% training, 25% testing).

## Naive Bayes Model Implementation

### 1. Feature Extraction

- Used `CountVectorizer` from `sklearn.feature_extraction.text` to convert the text messages into a matrix of token counts.

### 2. Model Training

- Implemented the Multinomial Naive Bayes classifier using `MultinomialNB` from `sklearn.naive_bayes`.
- Trained the model on the training dataset.

### 3. Model Evaluation

- Evaluated the model's performance on the test dataset.
- Achieved an accuracy score of approximately 98.35%, indicating high classification performance.

### 4. Predictions

- Tested the model with new email messages to classify them as spam or ham.
- The model successfully predicted the category of the test messages.

## Key Findings

1. The Naive Bayes classifier performed exceptionally well on the SMS dataset, achieving an accuracy of 98.35%.
2. The model effectively distinguishes between spam and ham messages based on the features extracted from the text.

## Dependencies

- numpy
- pandas
- scikit-learn

## Usage

The notebook can be run sequentially to understand the implementation of the Naive Bayes Classifier and its application to SMS message classification. It provides insights into data preprocessing, model training, evaluation, and prediction.
