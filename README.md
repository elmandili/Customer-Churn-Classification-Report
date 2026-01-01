# Customer Churn Prediction and Driver Analysis

## Project Overview

This project applies supervised machine learning techniques to predict customer churn and to analyze the main factors that influence customer attrition. The goal is to support data-driven decision-making for customer retention by identifying high-risk customers and understanding the drivers behind churn.

Three different classification models are trained and compared: Logistic Regression, Random Forest, and AdaBoost. Several resampling strategies are evaluated to handle class imbalance, and models are assessed using standard classification metrics such as accuracy, recall, F1-score, and AUC.

---

## Objectives

- Predict whether a customer will churn based on account, service, billing, and satisfaction data.
- Compare different classification models and sampling strategies.
- Identify the most important drivers of churn.
- Provide actionable insights for business stakeholders.
- Highlight limitations and propose future improvements.

---

## Dataset

The dataset contains customer-level information including:

- Service subscriptions (security, backup, protection, support, unlimited data)
- Account details (contract type, tenure in months)
- Billing information (monthly charges)
- Payment method (credit card, mailed check)
- Internet service type (DSL, Fiber Optic, None)
- Promotional offers (Offer A–E)
- Customer satisfaction indicators  
- Target variable: `churn_value` (0 = no churn, 1 = churn)

The dataset is imbalanced, with significantly more non-churned customers than churned customers.

---

## Project Structure



---

## Models Used

- Logistic Regression (baseline, interpretable)
- Random Forest (nonlinear ensemble)
- AdaBoost (boosting-based classifier)

---

## Evaluation Metrics

- Accuracy
- Precision
- Recall
- F1-score
- ROC AUC

Recall and AUC are emphasized because missing churned customers is costly from a business perspective.

---

## Key Findings

- Customers with shorter tenure and lower satisfaction are more likely to churn.
- Higher monthly charges and fewer service add-ons are associated with increased churn risk.
- Contract structure, internet service type, and promotional offers significantly influence churn behavior.
- Random Forest with undersampling provided the best overall predictive performance.

---

## Limitations

- The dataset does not include behavioral data such as customer support interactions or complaints.
- Temporal patterns in churn behavior are not modeled.
- Feature importance and explainability could be improved using tools like SHAP.

---

## Future Work

- Add behavioral and time-series features.
- Perform more extensive hyperparameter tuning.
- Optimize classification thresholds for business objectives.
- Apply model explainability techniques (SHAP, partial dependence).
- Integrate cost-sensitive learning based on business retention costs.

---

## How to Run

1. Clone the repository.
2. Install required dependencies.
3. Open `main.ipynb` and run all cells.




Author

Aymane El Mandili
Computer Science