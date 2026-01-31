# AI-ML-Task9

Project Overview

This project focuses on detecting fraudulent credit card transactions. The primary challenge of this task was handling a highly imbalanced dataset where fraud cases represent a tiny fraction of the total transactions

Dataset

Source: Kaggle Credit Card Fraud Dataset.

Description: Contains transactions made by European cardholders in September 2013.

Imbalance: The dataset is heavily skewed toward "Non-Fraud" transactions, requiring specific evaluation metrics like Precision-Recall and F1-score rather than simple accuracy.

Implementation Steps

Data Loading: Used Pandas to load the dataset and verified the class distribution.

Preprocessing: Removed non-useful identifiers like 'Time' and separated features from the target.

Stratified Sampling: Split the data into training and testing sets while maintaining the original fraud ratio to ensure a fair evaluation.

Baseline Modeling: Trained a Logistic Regression model as a baseline for performance comparison.

Random Forest Classifier: Implemented a Random Forest model with n_estimators=100 to utilize ensemble learning for better stability.

Feature Importance: Plotted the top indicators of fraud to understand the key drivers of the model's decisions.

Model Persistence: Saved the final model using joblib for future deployment.

Key Results

Ensemble Learning: Random Forest outperformed the baseline model in catching minority class (fraud) instances.

Evaluation Metrics: Focused on Recall (to catch as many frauds as possible) and F1-score to balance precision and sensitivity
