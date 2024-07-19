# SHAP-Values-with-Acute-Poisonings-Dataset

## Overview

This project aims to predict the severity of poisoning based on various features such as age, gender, symptoms, and type of poison. The main techniques used include data balancing, feature importance analysis using SHAP values, and model evaluation metrics.

## Files

- `code.ipynb`: Jupyter notebook containing the code for data preprocessing, model training, evaluation, and feature importance analysis.

## Requirements

- Python 3.8 or higher
- Jupyter Notebook
- pandas
- numpy
- scikit-learn
- imbalanced-learn
- shap

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/your-repo/poisoning-severity-prediction.git
   ```

Explanation of SHAP Values
What are SHAP Values?
SHAP (SHapley Additive exPlanations) values are a method to explain individual predictions of machine learning models. The SHAP values are based on cooperative game theory and Shapley values, which provide a way to fairly distribute the "payout" (in this case, the model's prediction) among the features based on their contribution.

How SHAP Values Work
SHAP values assign each feature an importance value for a particular prediction. They provide insights into how each feature influences the prediction by considering all possible combinations of features. The main idea is to compute the average marginal contribution of a feature across all possible subsets of features.

Why Use SHAP Values?
Interpretability: SHAP values make it easy to understand the contribution of each feature to the model's predictions.
Fairness: SHAP values provide a fair distribution of feature importance based on Shapley values from game theory.
Global and Local Explanations: SHAP values can be used to explain individual predictions (local explanations) as well as overall feature importance (global explanations).
Steps in the Notebook
Data Preprocessing:

Load the data
Handle missing values
Encode categorical variables
Balance the dataset using SMOTE
Model Training:

Train a machine learning model (e.g., Random Forest)
Model Evaluation:

Evaluate the model using accuracy, precision, recall, and F1-score
Feature Importance Analysis:

Calculate feature importance using SHAP values
Identify the most and least important features
Comparison of Features:

Identify highly correlated features with the target class
Compare these features with the top features identified by SHAP values
