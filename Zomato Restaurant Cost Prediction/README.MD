# 🍽️ Zomato Restaurant Cost Prediction – Machine Learning Project

## 📌 Project Overview
This project explores restaurant data from Zomato to build a machine learning model that predicts the **average cost for two people** based on key restaurant features.  
The goal is to understand how attributes such as location, rating, cuisines, and votes influence pricing and to develop a regression model that provides cost estimates.

---

## 🛠 Tools & Technologies
- **Python**  
- **pandas** – data preprocessing  
- **NumPy** – numerical operations  
- **scikit-learn** – ML modelling & evaluation  
- **Matplotlib & Seaborn** – visualizations  
- **Jupyter Notebook**  

---

## 📂 Dataset
- **File:** `zomato.csv`  
- Contains features such as:
  - Restaurant name  
  - Location  
  - Online delivery availability  
  - Ratings  
  - Votes  
  - Type of cuisines  
  - Price for two  

---

## 🔧 Workflow Summary
### 1. **Data Cleaning**
- Removed missing and duplicate entries  
- Normalized "price" column  
- Converted categorical variables via one-hot encoding  
- Cleaned cuisine and location columns  

### 2. **Feature Engineering**
- Extracted cuisine count  
- Simplified location tags  
- Converted ratings into numeric format  

### 3. **Model Development**
Tested multiple regression models:
- Linear Regression  
- Decision Tree Regressor  
- Random Forest Regressor  

### 4. **Evaluation**
- Split dataset: **80% train / 20% test**  
- Metrics used:
  - **R² Score**
  - **MAE (Mean Absolute Error)**
  - **RMSE (Root Mean Squared Error)**  

📌 **Best performing model: Random Forest (R² ≈ 0.70)**

---

## 📊 Key Insights
- Restaurants located in premium areas tend to have higher prices.  
- Average cost strongly correlates with **ratings + votes** (popular restaurants cost more).  
- Multi-cuisine restaurants show higher price variation.  
- Online delivery availability did **not** significantly impact cost.  

---

## 📘 What I Learned
- How to preprocess messy real-world restaurant data  
- Applying one-hot encoding for categorical features  
- Comparing machine learning regression models  
- Understanding evaluation metrics (R², MAE, RMSE)  
- Communicating model insights effectively  

---

