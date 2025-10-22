# 🚗 Project 3 — Car Price Prediction (Regression)

## 📋 Overview
This project explores the use of **regression models** to predict the **price of cars** based on their specifications.  
It involves **data cleaning**, **exploratory data analysis (EDA)**, **feature engineering**, and **model evaluation** using a dataset scraped from the web (`cars_data.csv`).

---

## 📊 Dataset
The dataset **`cars_data.csv`** contains detailed information about various cars, including:
- Company and model  
- Engine details  
- Performance metrics (horsepower, speed, acceleration)  
- Fuel type and seats  
- Torque and price  

### ⚠️ Challenges
The raw dataset required **significant cleaning** due to:
- Numerical values stored as strings with units (e.g., `'963 hp'`, `'3990 cc'`, `'$1,100,000'`)  
- Presence of **ranges** (e.g., `'70-85 hp'`)  
- **Missing values** (`'N/A'`) 
