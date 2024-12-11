# Predicting Customer Churn for Beta Bank

## Project Overview
Beta Bank seeks to predict whether a customer will leave the bank to proactively retain valuable clients. This project builds a machine learning model to classify customer churn with a target F1 score of at least **0.59**.

---

## Table of Contents
1. [Dataset Description](#dataset-description)
2. [Goal](#goal)
3. [Libraries Used](#libraries-used)
4. [Methodology](#methodology)
5. [Results](#results)
6. [Conclusion](#conclusion)
7. [How to Use](#how-to-use)
8. [Contact](#contact)

---

## Dataset Description
The dataset contains customer behavior data, demographics, and financial details, including:
- **Features**:
  - `CreditScore`: Customer credit score.
  - `Geography`: Country of residence.
  - `Gender`: Gender of the customer.
  - `Age`: Age of the customer.
  - `Tenure`: Years of fixed deposit maturity.
  - `Balance`: Customer account balance.
  - `NumOfProducts`: Number of banking products used.
  - `HasCrCard`: Whether the customer owns a credit card.
  - `IsActiveMember`: Whether the customer is an active member.
  - `EstimatedSalary`: Customer’s estimated salary.
- **Target**:
  - `Exited`: 1 if the customer left the bank, 0 otherwise.

---

## Goal
Develop a machine learning model that:
1. Predicts customer churn.
2. Achieves an F1 score of at least **0.59** on the test set.

---

## Libraries Used
The project uses the following Python libraries:
- **Pandas**: Data manipulation and analysis.
- **NumPy**: Numerical operations.
- **Matplotlib**: Data visualization.
- **Scikit-learn**: Model building and evaluation.
- **XGBoost**: Advanced boosting model for classification.

---

## Methodology
1. **Data Preparation**:
   - Filled missing values in the `Tenure` column with the median.
   - Encoded categorical features using One-Hot Encoding and binary encoding.
   - Split data into training, validation, and test sets.
2. **Class Imbalance Handling**:
   - Addressed imbalance using class weighting and upsampling.
3. **Model Training**:
   - Tested models: Logistic Regression, Random Forest, Gradient Boosting, and XGBoost.
   - Fine-tuned parameters for the best performance.
4. **Evaluation**:
   - Measured performance using F1 Score and AUC-ROC.

---

## Results
The final model, **XGBoost**, achieved:
- **F1 Score**: 0.5921 (on test set).
- **AUC-ROC**: 0.8378 (on test set).

---

## Conclusion
The XGBoost model met the project target of an F1 score ≥ **0.59**. Its performance demonstrates its ability to accurately predict customer churn, making it a valuable tool for Beta Bank to retain customers and optimize resources.