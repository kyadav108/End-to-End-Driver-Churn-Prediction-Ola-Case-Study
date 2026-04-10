# 🚖 Driver Churn Prediction & Analysis (Ola Case Study)

## 📌 Overview

This project focuses on analyzing driver behavior and predicting churn for a ride-sharing platform like Ola. The goal is to identify patterns that indicate potential churn and build a machine learning model to predict drivers at risk of leaving.

---

## 📊 Dataset

* ~19,000 records
* Features include:

  * Demographics: Age, Gender, Education
  * Job Info: Joining Designation, Grade
  * Performance: Quarterly Rating
  * Financials: Income, Total Business Value
  * Temporal: Date of Joining, Reporting Month

---

## 🔍 Key Steps

### 1. Exploratory Data Analysis (EDA)

* Checked missing values and distributions
* Identified skewness and outliers
* Analyzed relationships between:

  * Income vs Grade
  * Rating vs Churn
  * City vs Performance

---

### 2. Data Preprocessing

* Missing value treatment (median/mode)
* Outlier handling using IQR capping
* Log transformation for skewed features
* Datetime conversion

---

### 3. Feature Engineering

* Created:

  * `Churn` (target variable)
  * `Employee Tenure`
  * `Age Categories`
* Extracted:

  * Month, Year, Quarter features

---

### 4. Encoding

* Label Encoding (binary features)
* One-Hot Encoding (low cardinality)
* Target Encoding (City)

---

### 5. Handling Imbalance

* Applied **SMOTE** to balance churn classes

---

## 🤖 Model Used

* **Random Forest Classifier**

---

## ❓ Why Random Forest?

* Handles **non-linear relationships** effectively
* Works well with **mixed data types** (categorical + numerical)
* Reduces overfitting using **bagging and feature randomness**
* Provides **robust performance without heavy tuning**
* Suitable for datasets with **many features and interactions**

---

## 📈 Model Performance

| Metric    | Score        |
| --------- | ------------ |
| Accuracy  | 95%          |
| ROC-AUC   | 0.91         |
| Precision | 0.84 (Churn) |
| Recall    | 0.47 (Churn) |

---

## 🔑 Key Insights

* Low-rated drivers are more likely to churn
* Lower income → higher churn probability
* Short tenure drivers leave more frequently
* Higher-performing drivers generate more business and stay longer

---

## 🚀 Business Impact

* Helps identify at-risk drivers early
* Enables targeted retention strategies
* Improves driver satisfaction & revenue

---

## 🛠️ Tech Stack

* Python (Pandas, NumPy)
* Visualization: Matplotlib, Seaborn
* Machine Learning: Scikit-learn
* Imbalance Handling: SMOTE

---
