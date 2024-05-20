# classification-challenge
Module 13 Challenge

## Project Overview

This project involves building and evaluating two supervised machine learning models, Logistic Regression and Random Forest, to detect spam emails. The goal is to improve the email filtering system for an Internet Service Provider (ISP) by accurately classifying emails as spam or not spam.

## Data

The dataset used in this project can be downloaded from the following link:
- [Spam Data CSV](https://static.bc-edx.com/ai/ail-v-1-0/m13/challenge/spam-data.csv)

The dataset contains various features extracted from emails, with a `spam` column indicating whether an email is spam (1) or not spam (0).

## Project Steps

### 1. Data Loading and Preparation

- Load the data into a Pandas DataFrame.
- Make a prediction about which model is expected to perform better.
- Create the labels set (`y`) from the `spam` column.
- Create the features DataFrame (`X`) from the remaining columns.
- Check the balance of the labels using the `value_counts` function.
- Split the data into training and testing sets using `train_test_split`.

### 2. Feature Scaling

- Create an instance of `StandardScaler`.
- Fit the scaler with the training data.
- Scale the training and testing feature sets using the `transform` function.

### 3. Logistic Regression Model

- Create and fit a logistic regression model using the scaled training data.
- Make predictions on the testing data.
- Evaluate the model's performance using the `accuracy_score` function.

### 4. Random Forest Model

- Create and fit a random forest classifier using the scaled training data.
- Make predictions on the testing data.
- Evaluate the model's performance using the `accuracy_score` function.

### 5. Model Evaluation

- Compare the performance of the Logistic Regression and Random Forest models.
- Document which model performed better and how it compares to the initial prediction.

## Results

- The accuracy of both models is calculated and compared.
- The model that performed better in detecting spam emails is highlighted.

## Conclusion

- The project concludes with a discussion on which model is more suitable for the ISP's email filtering system based on the accuracy scores obtained.
