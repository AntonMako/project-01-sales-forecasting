# 📊 E-commerce Sales Forecasting & Customer Churn Analysis

## Project Overview
This project presents an end-to-end data science analysis of e-commerce transactional data, focusing on two key business problems:

1. **Sales forecasting** – predicting future monthly revenue
2. **Customer churn analysis** – identifying customers at risk of becoming inactive

The project demonstrates the full data science workflow, including data preparation, feature engineering, modeling, evaluation, and business interpretation.

---

## 📁 Dataset
The analysis uses publicly available e-commerce transaction data containing:
- Invoice and product information
- Customer identifiers
- Purchase dates
- Quantities and unit prices
- Country / region details

The data is included for reproducibility and learning purposes.

---

## 🔹 Sales Forecasting

**Objective:**  
Forecast future monthly revenue to support planning and decision-making.

**Approach:**
- Aggregated transactional data into monthly revenue
- Used a time-aware train/test split
- Compared multiple forecasting models

**Models evaluated:**
- Seasonal Naive (baseline)
- ARIMA
- SARIMA (tested and rejected due to unstable seasonality)
- Random Forest with lag and rolling features

**Evaluation metrics:**
- Mean Absolute Error (MAE)
- Root Mean Squared Error (RMSE)

**Outcome:**
- The Random Forest model achieved the lowest forecasting error
- ARIMA served as a strong classical baseline
- Model performance was interpreted relative to revenue scale

---

## 🔹 Customer Churn Analysis

**Objective:**  
Identify customers likely to churn based on purchasing behavior.

**Churn definition:**  
Customers are considered churned if they have not made a purchase within a defined recency threshold.

**Features (RFM):**
- **Recency:** Days since last purchase
- **Frequency:** Number of unique invoices
- **Monetary:** Total customer spend

**Models used:**
- Logistic Regression (baseline)
- Random Forest Classifier

**Key insights:**
- Recency is the strongest predictor of churn
- Probability-based churn predictions enable customer ranking
- Churn risk tiers support targeted retention strategies

---

## 📈 Business Value
- Sales forecasts support inventory and revenue planning
- Churn probabilities allow prioritization of customer retention efforts
- Feature importance improves model interpretability for stakeholders

---

## ⚠️ Notes & Limitations
- Churn labels are behavior-based and derived from transactional activity
- Class imbalance is discussed and handled through appropriate evaluation
- Models are intended for analytical insight rather than production deployment

---

## 🛠️ Tools & Libraries
- Python
- pandas, numpy
- scikit-learn
- statsmodels
- matplotlib, seaborn

---

## 👤 Author
**Lungile Makondo**  
Aspiring Data Scientist  

GitHub: https://github.com/AntonMako