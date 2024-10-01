# Module 12 Report Template

## Overview of the Analysis

The purpose of this analysis is to create machine learning models that can predict the credit risk of borrowers using historical financial data. The primary goal is to classify potential loans as either high or low risk based on various features present in the dataset. This kind of classification is crucial for financial institutions to mitigate risks and ensure that they make informed lending decisions.

The dataset used in this analysis includes a variety of financial features about borrowers, including their income, debt, and credit history. The key target variable we are trying to predict is whether a borrower falls under the "high risk" or "low risk" category. The variable being predicted is binary, with `1` indicating a high-risk borrower and `0` indicating a low-risk borrower.

To achieve accurate predictions, several machine learning models were implemented. These models include logistic regression and random forest classifier algorithms, which went through a standard machine learning process involving data preprocessing, model training, evaluation, and refinement.

The stages of the machine learning process used in this analysis were:

1. Data Preprocessing: Handling missing values, feature selection, and standardizing the data.
2. Model Training: Training the data on logistic regression and random forest classifiers.
3. Model Evaluation: Using accuracy, precision, and recall to evaluate the models' performance.

## Results

### Logistic Regression Model:

- **Accuracy**: The logistic regression model achieved an accuracy score of approximately 95.7%.
- **Precision**: The precision score for predicting high-risk loans was about 85.71%.
- **Recall**: The recall score for high-risk loans was around 91%.

### Random Forest Classifier Model:

- **Accuracy**: The random forest classifier achieved a slightly lower accuracy score of approximately 93.9%.
- **Precision**: The precision score for high-risk loans was around 84.62%.
- **Recall**: The recall score for high-risk loans was 100%, meaning that the model captured all high-risk loans correctly.

## Summary

Both machine learning models provide high accuracy, precision, and recall scores, making them viable options for predicting credit risk. However, based on the results:

- The **random forest classifier** stands out for its perfect recall score (100%), meaning it correctly identified all high-risk loans. This is a critical factor in credit risk scenarios because it ensures that all potential high-risk borrowers are identified.

- The logistic regression model, while slightly more accurate overall, does not have as high recall as the random forest model, making it less favorable for this specific task where identifying all high-risk loans is crucial.

### Recommendation:

Given the higher recall score of the random forest model, I would recommend using it for credit risk classification. In credit risk analysis, the ability to correctly identify high-risk loans (even at the expense of a few false positives) is often more important than overall accuracy, as it helps in minimizing financial losses due to risky loans.