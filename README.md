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
    ## Data Analysis 
# Univariate Analysis
<img width="729" height="761" alt="image" src="https://github.com/user-attachments/assets/9c702a78-18df-465d-b9d0-4bcc67ed140e" />
most of the applicants are male ith 82% compared to 18.2% of females
<img width="975" height="549" alt="image" src="https://github.com/user-attachments/assets/a1cc6b6c-aa1b-4314-a941-83fbd4314f9f" />
The applicant income distribution is highly right-skewed, with most applicants earning between 0 and 10,000. The mean (5,403) is noticeably higher than the median (3,812), indicating the presence of high-income outliers that stretch the distribution up to around 80,000–90,000. These extreme values could influence loan prediction models and may require preprocessing, such as capping or transformation.
<img width="975" height="549" alt="image" src="https://github.com/user-attachments/assets/8e675b56-d524-46e7-92a7-22f3be5de614" />
The loan amount distribution is right-skewed, with most loans concentrated between 100 and 200, peaking around 120 and 150. The mean (145.75) is slightly higher than the median (128), indicating some higher-value loans stretching the distribution. A few upper outliers exist in the 500–700 range, but overall, the distribution is relatively controlled and more standardized compared to applicant income
<img width="975" height="541" alt="image" src="https://github.com/user-attachments/assets/b8237c8f-4de7-47f6-9af9-e28bb841da5c" />
The loan term distribution is highly concentrated around 360 months, indicating that most applicants opt for a 30-year loan term. Other loan terms (like 120, 180, 240, 300, and 480 months) appear much less frequently, with very few applicants choosing these durations. This shows that lenders and borrowers strongly prefer the standard long-term option, while shorter or unusual terms are rare.
<img width="865" height="686" alt="image" src="https://github.com/user-attachments/assets/c931a826-1197-4509-9fcc-45126bc41ebe" />
The analysis shows that gender does not significantly affect loan approval. Although there are more male applicants than female applicants, both genders have similar approval rates (about 69% for males and 67% for females). This suggests that loan approval decisions are largely gender-neutral, and gender alone is not a key factor in determining loan status.
<img width="865" height="686" alt="image" src="https://github.com/user-attachments/assets/e3a7bb5f-0fd4-42d8-bd73-93af76f109f9" />
Education level appears to influence loan approval. Graduate applicants have a higher approval rate (about 71%) compared to non-graduates (about 61%). Although both groups receive more approvals than rejections, graduates are approved at a noticeably higher rate, suggesting that higher education may be associated with better loan approval outcomes in this dataset.




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



