# LOAN-PREDICTION-HACKATHON

## 🏦 Project Objective: Loan Eligibility Prediction

Dream Housing Finance Company provides home loans across **urban, semi-urban, and rural** regions. To improve operational efficiency and reduce manual processing time, the company aims to **automate the loan eligibility decision process in real time** using customer data submitted through online applications.

The goal of this project is to build a **machine learning–based classification system** that predicts whether a customer is eligible for a home loan based on their demographic and financial information.

---

## 📊 Problem Statement

Loan eligibility assessment is traditionally a manual, time-consuming process that may be prone to inconsistencies. Automating this process enables the company to:

* Reduce loan processing time
* Improve decision consistency
* Minimize human bias
* Scale eligibility checks efficiently

---

## 🧾 Input Features

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

## 🎯 Target Variable

* **Loan_Status**

  * `1` → Loan Approved
  * `0` → Loan Rejected

---

## ⚙️ Solution Approach

* Data preprocessing and feature engineering
* Handling class imbalance using **SMOTE**
* Feature scaling for numerical variables
* Training and comparison of multiple machine learning models
* Model evaluation using **ROC-AUC, precision, recall, and F1-score**
* Selection of an interpretable and high-performing final model

---

## 🏆 Final Outcome

A **Logistic Regression model** was selected as the final solution due to:

* Strong predictive performance (ROC-AUC ≈ 0.86)
* High recall for eligible applicants
* Transparent and interpretable feature contributions

This model enables **real-time loan eligibility prediction**, helping Dream Housing Finance Company efficiently identify eligible applicants while maintaining fairness and explainability.

---


