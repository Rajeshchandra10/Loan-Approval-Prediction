# Loan-Approval-Prediction
 
## Overview

This project demonstrates a comprehensive machine learning workflow to predict the approval status of loan applications. By leveraging a variety of machine learning models and robust data preprocessing techniques, it addresses a real-world classification problem. The goal is to build and evaluate models that can accurately determine whether a loan should be approved based on key applicant and financial data.

## Project Goal
The primary objective of this project is to develop a predictive model that can classify loan applications as either approved or rejected. The process involves:

 Data Preprocessing: Cleaning and preparing the dataset for modeling.

 Feature Engineering: Creating a new target variable based on business logic.

 Model Building: Implementing and training multiple classification models.

 Performance Evaluation: Comparing models using a variety of metrics to select the best one.

## Dataset
The project utilizes the loan_approval_prediction_train.csv dataset. The dataset contains various features about loan applicants. The Loan_Status variable, which serves as the classification target, was engineered from existing features (Credit Score and Annual Income).

## Methodology
Data Preprocessing and Feature Engineering
  
- Missing Value Imputation: Handled missing values to ensure data integrity.

- One-Hot Encoding: Converted categorical data into a numerical format suitable for machine learning algorithms.

- Feature Scaling: Applied RobustScaler to normalize numerical features, which is particularly beneficial for models like SVM and KNN.

- Target Variable Creation: A new Loan_Status column was created where a loan is approved (1) if the Credit Score is 700 or greater AND the Annual Income is $50,000 or greater; otherwise, it is rejected (0).

Model Implementation and Evaluation

Three distinct classification models were trained and their performance was evaluated using a confusion matrix and a classification report.
- Support Vector Machine (SVM)
- Logistic Regression
- K-Nearest Neighbors (KNN)

## Code and Dependencies
- Jupyter Notebook: Loan-Approval-Prediction.ipynb

- Python Script: ml_project.py

Libraries:

- pandas

- numpy

- scikit-learn

- matplotlib

- seaborn
