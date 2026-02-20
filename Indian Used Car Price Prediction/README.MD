# 📘 Project Overview  
The goal of this data science project is to **predict the price of used cars** in major Indian metro cities.  
The prediction is based on various car features, including:  

- Manufacturer, model, variant  
- Fuel type, color, kilometers driven  
- Body style, transmission type  
- Manufacture date, model year, and CNG kit availability  
- Ownership history, dealer details, and quality score  

This project applies **Exploratory Data Analysis (EDA)** and **Machine Learning techniques** to uncover patterns and predict prices, ultimately helping both **buyers and sellers** make informed decisions in the used car market.

---

# 🧾 Data Dictionary  

Here’s the detailed data dictionary for the columns in the *“Indian IT Cities Used Car Dataset 2023”*:  

| **Column Name** | **Description** |
|------------------|-----------------|
| ID | Unique ID for each listing |
| Company | Name of the car manufacturer |
| Model | Name of the car model |
| Variant | Name of the car variant |
| Fuel Type | Fuel type of the car |
| Color | Color of the car |
| Kilometer | Number of kilometers driven by the car |
| Body Style | Body style of the car |
| Transmission Type | Transmission type of the car |
| Manufacture Date | Manufacture date of the car |
| Model Year | Model year of the car |
| CngKit | Whether the car has a CNG kit or not |
| Price | Price of the car |
| Owner Type | Number of previous owners of the car |
| Dealer State | State in which the car is being sold |
| Dealer Name | Name of the dealer selling the car |
| City | City in which the car is being sold |
| Warranty | Warranty offered by the dealer |
| Quality Score | Quality score of the car |

---

# 📊 Key Insights  

## 🔹 Demand and Price Trends  
Lower-priced used cars have higher demand, showing consumers’ preference for budget-friendly options.  
Luxury brands like **MG, Mercedes-Benz, BMW, Volvo, and KIA** command higher prices, indicating buyers often prefer new luxury cars over used ones.

## 🔹 Fuel Type Influence  
Fuel type plays an important role in pricing — **diesel cars** tend to be priced slightly higher than petrol ones.  

## 🔹 Color Preferences  
Common colors such as **white, grey, silver, and black** are in higher demand, while rare colors like **burgundy, riviera red, dark blue, and black magic** fetch premium prices.  

## 🔹 Kilometer Reading Impact  
Cars with **lower mileage (<10,000 km)** are priced higher, showing that odometer readings directly affect resale value.  

## 🔹 Body Style Preferences  
Top choices among buyers are **hatchbacks, SUVs, and sedans**, while MPVs and luxury SUVs are generally more expensive.  

## 🔹 Age and Resale Value  
Cars **less than 5 years old** hold higher resale value, emphasizing demand for newer used vehicles.  

## 🔹 Geographic Price Variation  
Cities in **Delhi, Maharashtra, and Rajasthan** show higher car prices.  
Dealers like **Car Estate**, **Star Auto India**, and **Car Choice** consistently list cars at higher price points.  

## 🔹 Owner Type and Warranty Impact  
**First-owner cars** and those offering **warranties** tend to sell at higher prices due to buyer trust and assurance.  

## 🔹 Quality Score and Pricing  
Higher **quality scores** directly correlate with higher car prices.  

---

# 🤖 Machine Learning Models  
Two regression models were implemented:  
- **Decision Tree Regressor**  
- **Random Forest Regressor**  

Among them, the **Random Forest Regressor** demonstrated superior performance with better prediction accuracy.  
Feature importance analysis revealed that **car age**, **body style**, and **manufacturer** are the most influential factors in determining price.  

---

# 🏁 Conclusion  
This project provides valuable, data-driven insights into the **Indian used car market**, empowering both buyers and sellers to make smarter decisions.  
By combining **EDA and Machine Learning**, the project successfully highlights key pricing drivers and improves transparency in car price estimation.

---

