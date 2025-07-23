## *Project Title:**

**Telecom Customer Churn Prediction**



Telecom companies face high customer turnover. This project aims to **predict customer churn** using machine learning so that retention teams can **proactively target high-risk customers** with personalized offers, improving customer loyalty and reducing revenue loss.

--

##  Approach & Workflow:

#1. Exploratory Data Analysis (EDA):

* Analyzed customer demographics, services used, account information, and payment behaviors.
* Identified key churn indicators:

  * Short tenure (new customers)
  * Monthly contracts
  * High monthly charges
  * Lack of additional services (e.g., no online security or tech support)



### 2. Data Preprocessing:

* Removed irrelevant columns (e.g., customer ID).
* Converted non-numeric features to numeric using label encoding.
* Handled missing values in `TotalCharges` by imputing with the median.
* Ensured correct data types for all features.



# 3. Class Imbalance Handling:

* Churned customers were the minority (\~26%).
* Applied SMOTE (Synthetic Minority Over-sampling Technique)to balance the dataset.
* Ensured fair model learning for both churned and non-churned customers.



# 4. Modeling & Evaluation:

* Trained multiple models including **Random Forest, Logistic Regression, and XGBoost.
* Random Forest gave the best performance:

  * Accuracy: \~85%
  * Precision: \~84%
  * Recall: \~82%
  * ROC AUC Score: \~0.87
* Evaluation metrics showed strong ability to identify churners without many false positives.



# 5. Model Explainability:

* Used SHAP (SHapley Additive exPlanations) to interpret model decisions.
* Key insights from SHAP:

  * Short tenure→ High churn risk
  * Electronic check payments** → Higher likelihood of churn
  * No tech support or online security → Strong indicators of dissatisfaction
* Provided transparent feature-level explanations for business stakeholders.


## 3 Major Actionable Business Insights:

1. Contract Type Matters:

   * Monthly contract customers churn the most.
   * Promote longer-term contracts with loyalty incentives or discounts.

2. Service Add-Ons Influence Retention:

   * Customers without tech support or online security are at higher churn risk.
   * Offer bundled or discounted support services to enhance perceived value.

3. Payment Method Predicts Churn:

   * Electronic check users are less stable and more likely to leave.
   * Encourage auto-pay options or credit card use via discounts or rewards.



Conclusion:

This project provides a robust, interpretable ML solution for predicting churn. It equips telecom businesses with the ability to understand who is likely to churn and why, and enables targeted, data-driven retention strategies that directly reduce customer loss and boost revenue.


. TASK:

https://colab.research.google.com/drive/1miNfRoikcg2N-HeV-EzW2adOZfYJLlkr#scrollTo=1FM5XxES5rQf
