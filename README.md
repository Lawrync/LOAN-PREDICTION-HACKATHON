# LOAN-PREDICTION-HACKATHON
 
 ## Introduction
Dream Housing Finance Company needs a forecasting mechanism that will make or deny an application for a home loan. The current manual review process is not effective and can not be applied in a large-scale application. The challenge is to develop a machine learning classification system, which will be based on the previous loan history and attributes of the applicant, to carefully forecast the loan approval.

## Problem Statement
Dream Housing Finance Company needs a forecasting mechanism that will make or deny an application for a home loan. The current manual review process is not effective and can not be applied in a large-scale application. The challenge is to develop a machine learning classification system, which will be based on the previous loan history and attributes of the applicant, to carefully forecast the loan approval.
## Objectives
To build a machine learning model for predicting loan approval status.

To preprocess and transform customer data for effective modeling.

To analyze the influence of applicant features on loan eligibility.

To achieve reliable prediction accuracy on unseen test data.

To support automated and scalable loan approval decisions.


##  Input Features

The model uses applicant details provided during the loan application process, including:

* Gender
* Marital Status
* Education Level
* Number of Dependents
* Applicant & Co-applicant Income
* Loan Amount
* Loan Term
* Credit History
* Property Area (Urban, Semi-urban, Rural)

---

##  Target Variable

* **Loan_Status**

  * `1` → Loan Approved
  * `0` → Loan Rejected

---

##  Solution Approach

* Data preprocessing and feature engineering
* Handling class imbalance using **SMOTE**
* Feature scaling for numerical variables
* Training and comparison of multiple machine learning models
* Model evaluation using **ROC-AUC, precision, recall, and F1-score**
* Selection of an interpretable and high-performing final model

---

##  Final Outcome

A **Logistic Regression model** was selected as the final solution due to:

* Strong predictive performance (ROC-AUC ≈ 0.86)
* High recall for eligible applicants
* Transparent and interpretable feature contributions

This model enables **real-time loan eligibility prediction**, helping Dream Housing Finance Company efficiently identify eligible applicants while maintaining fairness and explainability.



