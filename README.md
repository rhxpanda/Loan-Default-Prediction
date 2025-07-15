# 💰 Loan Default Risk Prediction

## 🧠 Project Overview

This project analyzes loan application and repayment data to predict **whether a borrower is likely to default**. The goal is to assist financial institutions in risk management and credit decision-making.

---

## 📂 Dataset

- **Source:** The dataset for this project is sourced from Kaggle, available at [Loan Prediction with 3 Problem Statements](https://www.kaggle.com/datasets/yashpaloswal/loan-prediction-with-3-problem-statement)
- **Features include:**
  - Loan amount, interest rate, term
  - Borrower income, employment status
  - Credit history (e.g. delinquencies, credit score)
  - Loan status (defaulted or fully paid)

---

## 🔍 Exploratory Data Analysis (EDA)

- **Target Variable:** `loan_status` (Fully Paid vs Charged Off)
- **Key Insights:**
  - Higher interest rates are associated with higher default rates
  - Shorter loan terms tend to have lower default probabilities
  - Delinquency history is a strong indicator of risk
- **Visualizations:** Boxplots, density curves, and bar charts were used to explore feature distributions and class separability.

---

## 🤖 Modeling

We tested three classification models:

| Model             | Engine   |
|------------------|----------|
| Logistic Regression | `glm`     |
| Decision Tree     | `rpart`   |
| Random Forest     | `randomForest` |

### 🔧 Workflow:

- Data was preprocessed using `recipe()` from the `tidymodels` framework
- Models were compared using `roc_auc` as the primary metric
- Evaluation used both training-validation split and final holdout testing (`last_fit()`)

---

## 📈 Results

- **Random Forest** outperformed other models in terms of ROC AUC and accuracy
- Logistic Regression provided interpretability and useful feature coefficients
- The final confusion matrix and ROC curve confirmed robustness on unseen data

---

## ✅ Key Takeaways

- Borrower features like interest rate, delinquencies, and loan term are strong indicators of default risk
- Ensemble models like Random Forest can significantly improve predictive performance
- A structured modeling pipeline with `tidymodels` ensures reproducibility and interpretability

> _This project was submitted as part of the final assignment for STAT5125: Statistical Computing._
