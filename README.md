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
    │   ├── credit_risk_classification.ipynb  
    │   ├── lending_data.csv                  
    ├── Credit_Risk_Analysis_Report.md 
    └── README.md                     

**Notes:**

1. The dataset is located in the `Resources` folder (`lending_data.csv`).
2. The Jupyter Notebook file `credit_risk_classification.ipynb` contains the full analysis.
3. You can run the notebook to train the logistic regression model, make predictions, and evaluate the model's performance.

## Analysis Process

The analysis is broken down into the following steps:

1. Data Preprocessing: Handling missing values, feature selection, and data standardization.

2. Model Training: Logistic regression was selected and trained on the dataset.

3. Model Evaluation: Evaluated the model using accuracy, precision, and recall metrics.

## Results

### Logistic Regression Model:

- **Accuracy**: 99%
- **Precision (High-Risk Loans)**: 0.85
- **Recall (High-Risk Loans)**: 0.94

The logistic regression model performs well in predicting high-risk loans, making it a useful tool for financial institutions assessing credit risk. While the precision for high-risk loans is 85%, meaning that 15% of predicted high-risk loans are false positives, the recall is high at 94%, indicating that the model correctly identifies most high-risk borrowers.

### Confusion Matrix:

|  | Predicted 0 | Predicted 1 | 
| ---- | ---- | ----  |
| **Actual 0** | 14,895 | 86 | 
| **Actual 1** | 32 | 495 | 

### Classification Report:



    
                     precision    recall  f1-score   support
    
    0 (Low-Risk)       1.00       0.99      1.00      14981
    1 (High-Risk)      0.85       0.94      0.89        527
    
    Accuracy                               0.99      15508
    Macro Avg         0.92       0.97      0.94      15508
    Weighted Avg      0.99       0.99      0.99      15508


### Summary:

Based on the results, the logistic regression model is recommended for identifying high-risk loans, especially due to its strong recall score (94%) for predicting high-risk borrowers. The model accurately classifies the majority of high-risk loans, which can help reduce financial risks for lenders. However, further tuning may improve precision to reduce false positives.

Thanks for your time. Have a wonderful day.