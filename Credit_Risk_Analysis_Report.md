# Credit Risk Classification Analysis Report

## Overview of the Analysis

The purpose of this analysis is to develop a machine learning model that predicts the credit risk of borrowers based on historical financial data. The goal is to classify loans as either high or low risk to help financial institutions mitigate risks when making lending decisions. The dataset used contains financial attributes like income, debt, and credit history. The target variable is binary: `1` for high-risk borrowers and `0` for low-risk borrowers. The main model used in this analysis is **logistic regression**.

### Stages of the Machine Learning Process:

1. **Data Preprocessing**: Handling missing values, feature selection, and data standardization.
2. **Model Training**: Logistic regression was selected and trained on the dataset.
3. **Model Evaluation**: Evaluated the model using accuracy, precision, and recall metrics.

## Results

### Logistic Regression Model:

- **Accuracy**: 99%
- **Precision (0 - Low Risk)**: 1.00 (Perfect precision for low-risk loans)
- **Precision (1 - High Risk)**: 0.85 (85% of predicted high-risk loans were correct)
- **Recall (0 - Low Risk)**: 0.99 (Identified 99% of actual low-risk loans)
- **Recall (1 - High Risk)**: 0.94 (Identified 94% of actual high-risk loans)
- **F1-Score (High Risk)**: 0.89 (Shows balanced precision and recall for high-risk loans)

## Summary

The logistic regression model achieved high performance with an overall accuracy of 99%. It performed exceptionally well in predicting low-risk loans, with perfect precision and near-perfect recall. For high-risk loans, it captured 94% of the actual high-risk cases, although its precision was slightly lower at 85%, meaning that 15% of predicted high-risk loans were false positives.

### Recommendation:

The **logistic regression model** is highly suitable for credit risk classification. Although it produced some false positives for high-risk loans, its high recall makes it a strong choice for identifying risky borrowers, which is crucial for reducing potential financial losses. Further improvements could focus on fine-tuning to enhance precision for high-risk loans while maintaining high recall.
