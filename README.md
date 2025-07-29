# 📊 Bank Marketing - Term Deposit Prediction

This project analyzes a Portuguese banking dataset to predict whether a client will subscribe to a term deposit.

## 🔍 Problem Statement
The bank wants to improve the efficiency of its telemarketing campaigns. The objective is to build a classification model that can predict client subscription to a term deposit (`y` column: yes/no).

## 📁 Dataset
- **Source:** UCI Bank Marketing Dataset
- **File Used:** `bank-additional-full.csv`
- **Features:** 20+ variables including age, job, marital status, previous contact, etc.
- **Target:** `y` (Yes/No - term deposit subscription)

## ⚙️ Tools & Libraries Used
- Python (Pandas, NumPy, Matplotlib, Seaborn)
- Scikit-learn (Logistic Regression, Random Forest, SMOTE)
- SHAP (for model explainability)
- Google Colab

## 🧼 Data Preprocessing
- Handled missing values and 'unknown' values in categorical columns
- Dropped leakage column: `duration`
- Encoded categorical variables using OneHotEncoding
- Balanced the target class using SMOTE

## 📈 Model Building
- Split data into train-test sets
- Trained multiple models:
  - Logistic Regression
  - Random Forest (Best Performing)
- Evaluated using Accuracy, Precision, Recall, and Confusion Matrix

## 🔍 Model Explainability
- Used SHAP to understand feature importance and how individual variables affect predictions.

## ✅ Key Results
- Random Forest gave highest accuracy.
- Top factors influencing subscription: contact type, previous campaign outcome, month of contact, etc.

## 📊 Visualizations
- Distribution of Target Variable
- Subscription by Job & Marital Status
- Age Distribution
- SHAP Summary Plot

## 🚀 How to Run
1. Clone this repo
2. Run the Jupyter Notebook / Google Colab
3. Install dependencies using:
