# Default-of-Credit-Card-Clients

## 🧠 Project Overview

This project focuses on building a robust machine learning pipeline to predict **credit card default** using a real-world dataset from the **UCI Machine Learning Repository**. The goal is to assist financial institutions in risk management by classifying clients who are likely to default on their payments.

## 📊 Dataset Information

* **Source**: UCI Machine Learning Repository
* **Instances**: 30,000
* **Features**: 24
* **Target**: `Default payment next month` (1 = Yes, 0 = No)
* **Type**: Classification
* **Demographics**: Age, Gender, Marital Status, Education
* **Time Range**: April 2005 – September 2005

## 🧹 Data Preprocessing

* **Outlier Handling**: Winsorization
* **Missing Data**: Removed irregular entries
* **Encoding**: One-Hot Encoding for categorical variables
* **Scaling**: Min-Max Normalization
* **Imbalance Handling**: SMOTE (Synthetic Minority Oversampling Technique)
* **Feature Reduction**: Lasso Regression, Wrapper Methods (Bi-directional Elimination)

## 📈 Exploratory Data Analysis

* Target distribution visualizations
* Analysis by:

  * Gender
  * Marital status
  * Education level

Key insights:

* Males and married individuals showed a higher tendency to default.
* Higher education levels surprisingly correlated with higher default rates.

## 🤖 Machine Learning Models

The following models were implemented and tuned:

* **Logistic Regression**
* **K-Nearest Neighbors (KNN)**
* **Random Forest**
* **Support Vector Machines (Linear & RBF kernels)**
* **Decision Trees**

### Hyperparameter Tuning

* Used **Grid Search** with **5-fold Cross-Validation**
* Metrics Evaluated:

  * Accuracy
  * Precision
  * Recall
  * F1-Score
  * ROC-AUC
  * Confusion Matrix

## 🚀 Advanced Models

* **XGBoost**
* **Deep Learning (2-layer Neural Network)**
* **Extreme Machine Learning (MLP Classifier)**
* **Ensemble Model**: Combines top 3 models for better robustness

## ✅ Best Performing Model

* **XGBoost**

  * Highest accuracy and F1-score
  * Efficient with imbalanced data
  * Less complex and faster than ensemble model

## 🏁 Final Conclusion

The project successfully identifies key features influencing credit card default and develops models with strong predictive capability. **XGBoost** emerged as the optimal model for its balance of performance and complexity, making it ideal for real-world credit risk assessment applications.


