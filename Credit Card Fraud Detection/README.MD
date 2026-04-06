# 💳 Credit Card Fraud Detection Using Machine Learning

## 📌 Project Overview
This project focuses on detecting fraudulent credit card transactions using machine learning.  
The goal is to accurately classify rare fraudulent transactions within a highly imbalanced dataset.

The dataset is sourced from Kaggle and contains **284,807 transactions**, of which **only 492 (~0.17%)** are fraud — making this a challenging predictive modeling task.

Dataset link: https://www.kaggle.com/mlg-ulb/creditcardfraud

---

## 🛠 Tools & Technologies
- **Python**
- **pandas**, **NumPy** – preprocessing & data exploration  
- **scikit-learn** – ML modeling  
- **Matplotlib, Seaborn** – visualizations  
- **Jupyter Notebook**  

---

## ⚙️ Problem Description
Fraud detection is difficult because fraudulent transactions are rare and often resemble normal transactions.  
The aim of this project is to:

- Identify fraudulent credit card transactions  
- Minimize false negatives (missed fraud)  
- Handle extreme class imbalance effectively  

---

## 🧹 Data Preprocessing
### ✔ Handled Highly Imbalanced Classes  
- Used **SMOTE**, **Random Undersampling**, or **Class Weights**  
- Ensured that the minority class (fraud) is represented properly  

### ✔ Feature Scaling  
- Most features are already PCA-transformed (V1–V28)  
- Scaled `Amount` and `Time`  

### ✔ Data Cleaning  
- Removed duplicates  
- Checked missing values  
- Validated class distribution  

---

## 🧪 Exploratory Data Analysis (EDA)
Key EDA steps included:

- Visualizing class imbalance  
- Plotting amount distribution for fraudulent vs. normal transactions  
- Correlation heatmaps  
- Time-based fraud frequency  
- Outlier inspection  

---

## 🤖 Machine Learning Models

### Models Tested:
- Logistic Regression  
- Random Forest Classifier  
- Gradient Boosting  
- XGBoost (optional)  
- Isolation Forest (for anomaly detection)*

### Techniques Used:
- 80/20 train-test split  
- Cross-validation  
- Hyperparameter tuning  

---

## 🔍 Key Insights
- Fraud transactions are extremely rare → require specialized handling.  
- Fraudulent transactions often have significantly different PCA feature distributions.  
- Model performance improves drastically when using **class weights** or **SMOTE**.  
- Recall is the most important metric — missing fraud is expensive.  

---

## 📘 What I Learned
- Handling highly imbalanced datasets  
- Applying ML models to real-world financial security problems  
- Importance of precision/recall over accuracy  
- Fraud detection strategies used in industry  
- Improving ML models with techniques like SMOTE, scaling, and tuning  



