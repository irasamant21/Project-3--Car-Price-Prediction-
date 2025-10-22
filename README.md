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
## 🏁 Key Findings
- Higher **horsepower** correlates with higher **price** and faster **acceleration**.  
- **Feature engineering** had the biggest positive impact on model performance.  
- **Random Forest** with engineered features was the **best-performing model** overall.

| Experiment | Model | R² | RMSE | Notes |
|-------------|--------|-----|------|-------|
| 1 | Linear Regression | 0.64 | \$431K | Best baseline |
| 1 | Random Forest | 0.33 | \$593K | Underfit baseline |
| 2 | Random Forest (Engineered) | **0.87** | **\$260K** | Best overall |
| 3 | Tuned Random Forest | 0.87 | \$264K | No significant gain |

---

## 🧠 Best Model
**✅ Random Forest Regressor with engineered features (Experiment 2)**  
Delivered the most balanced performance between **accuracy** and **interpretability**.
