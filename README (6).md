# 📉 Churn Forecasting Model using Supervised Learning.

This project is focused on predicting customer churn using a machine learning pipeline. Churn prediction helps telecom companies retain customers by proactively identifying those likely to leave the service.

## 🧠 Project Overview

The goal of this project is to:
- Understand customer behavior through data
- Perform feature engineering and preprocessing
- Train and evaluate multiple machine learning models
- Build a predictive system to classify whether a customer is likely to churn

---

## 📁 Dataset Overview

- The dataset contains customer details like tenure, monthly charges, total charges, and various service subscriptions.
- The `Churn` column is the target variable (Yes/No).

### Key preprocessing steps:
- Removed irrelevant column (`CustomerID`)
- Handled missing values in `TotalCharges`
- Addressed class imbalance using **SMOTE (Synthetic Minority Oversampling Technique)**

---

## 🔍 Exploratory Data Analysis (EDA)

### Numerical Features:
- Distribution and outliers analyzed using boxplots
- Correlation heatmap created to understand relationships

### Categorical Features:
- Countplots used to understand distributions
- Label encoding applied for model compatibility

---

## 🛠️ Data Preprocessing

- Label Encoding of categorical features
- Train-test split for evaluation
- SMOTE applied to handle class imbalance

---

## 🤖 Model Training & Evaluation

Multiple classification models were trained:
- **Logistic Regression**
- **Decision Tree**
- **Random Forest**
- **XGBoost**

### 🔍 Key Finding:
Random Forest gave the **best accuracy** among all models with default parameters.

---

## 💾 Deployment Ready

- The best performing model is saved using `joblib`
- A predictive system is built to classify new customer data using the saved model

---

## 📌 Requirements

To run this notebook, install the following:

```bash
pip install pandas numpy seaborn matplotlib scikit-learn imbalanced-learn xgboost
