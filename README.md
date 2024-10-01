# Credit Risk Classification

## Overview

This project aims to develop a machine learning model to classify loan applicants as either high or low credit risks. By leveraging financial and personal information about borrowers, the goal is to predict whether a borrower is likely to default on their loan, thus helping financial institutions make more informed lending decisions.

The dataset used for this analysis comes from `lending_data.csv`, which includes a variety of features such as loan amount, income, and credit history. The target variable is `loan_status`, where `1` indicates a high-risk loan and `0` represents a low-risk loan.

## Technologies Used

- **Python 3.12**
- **Pandas**: For data manipulation.
- **Scikit-learn**: For machine learning model building and evaluation.

## Directory Structure
    
    CREDIT-RISK-CLASSIFICATION/
    ├── Credit_Risk/
    │   ├── credit_risk_classification.ipynb  # Jupyter Notebook with analysis
    │   ├── lending_data.csv                  # Dataset for model training and evaluation
    ├── Credit_Risk_Analysis_Report.md # Additional analysis report
    └── README.md                     # Project documentation (this file)

**Notes:**

1. The dataset is located in the `Resources` folder (`lending_data.csv`).
2. The Jupyter Notebook file `credit_risk_classification.ipynb` contains the full analysis.
3. You can run the notebook to train the logistic regression model, make predictions, and evaluate the model's performance.

## Analysis Process

The analysis is broken down into the following steps:

1. **Data Loading**:

    - The data is loaded into a Pandas DataFrame from the provided `lending_data.csv` file.
2. **Data Preprocessing**:

    - Features (X) and the target variable (y) are separated.
    - The data is split into training and testing sets using `train_test_split`.
3. **Logistic Regression Model**:

    - A logistic regression model is trained on the training data.
    - Predictions are made using the testing dataset.
4. **Model Evaluation**:

    - The model's performance is evaluated using a confusion matrix and a classification report to assess accuracy, precision, and recall.

## Results

### Logistic Regression Model:

- **Accuracy**: 98%
- **Precision**: 77% (for high-risk loans)
- **Recall**: 94% (for high-risk loans)

The logistic regression model performs well in predicting high-risk loans, making it a useful tool for financial institutions looking to assess loan applicants' credit risk.

### Confusion Matrix:

|  | Predicted 0 | Predicted 1 | 
| ---- | ---- | ----  |
| Actual 0 | 1862 | 21 | 
| Actual 1 | 23 | 71 | 

### Classification Report:
    
    
    
                  precision    recall  f1-score   support
    
    0 (Low-Risk)       0.99       0.99      0.99      1883
    1 (High-Risk)      0.77       0.94      0.85        94
    
    Accuracy                           0.98      1977
    


Based on the results, the logistic regression model is recommended for identifying high-risk loans, particularly due to its high recall score (94%) for predicting high-risk applicants. The model correctly classifies most of the high-risk loans, which can help mitigate financial risks. However, further tuning may be required to improve precision and minimize false positives.

Thanks for your time. Have a wonderful day.