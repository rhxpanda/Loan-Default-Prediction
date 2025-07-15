# 💰 Loan Default Risk Prediction

## 🧠 Project Overview

This project analyzes loan application and repayment data to predict **whether a borrower is likely to default**. The goal is to assist financial institutions in risk management and credit decision-making.

---

## 📂 Dataset

- **Source:** The dataset for this project is sourced from Kaggle, available at [Loan Prediction with 3 Problem Statements](https://www.kaggle.com/datasets/yashpaloswal/loan-prediction-with-3-problem-statement)
- **Key Features**:
- `ApplicantIncome`: Applicant's income
- `CoapplicantIncome`: Co-applicant's income
- `LoanAmount`: Loan amount
- `Credit_History`: Credit history
- `Property_Area`: Property area
- `Loan_Status`: Loan approval status (target variable)

---

## 🧹 Data Processing

1. Handle missing values  
2. Encode categorical variables  
3. Scale and normalize features  
4. Split into training and testing sets

---

## 🤖 Models

- **Logistic Regression**  
- **Random Forest**  
- **XGBoost**  
- **Neural Network** (10 layers, 10 nodes per layer)

---

## 📈 Results

| Model               | Performance         |
|---------------------|---------------------|
| Logistic Regression | 91.03% accuracy     |
| XGBoost             | 91.03% accuracy     |
| Random Forest       | 89.74% accuracy     |
| Neural Network      | AUC = 0.689         |

> _This project was submitted as part of the final assignment for STAT5125: Statistical Computing._
