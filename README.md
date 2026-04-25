# Uber-Dynamic-Pricing-Analysis
A Python data analysis project exploring Uber dynamic pricing patterns using regression and visualization.

# Uber Dynamic Pricing Analysis (Sydney)

## 📊 Project Overview
This project analyzes Uber ride data in Sydney to identify the key factors influencing ride pricing and to simulate the logic behind Uber’s dynamic pricing system.

The analysis is based on a dataset of 30,195 Uber trips, which was cleaned and filtered to 23,717 valid observations.

## 🎯 Objectives
- Identify key drivers of Uber fare
- Analyze demand patterns across time and location
- Quantify the impact of distance and duration on pricing
- Provide business insights into dynamic pricing strategies

## 📁 Dataset
- Source: Kaggle (Synthetic Uber Dataset - Sydney 2021)
- Original: 30,195 records
- Cleaned: 23,717 records

## ⚙️ Data Processing
- Removed irrelevant columns (Trip ID, country info, etc.)
- Dropped missing suburb values
- Filtered:
  - Drive Time: 5–60 minutes
  - Positive fare and distance
- Converted datetime features for time-based analysis

## 📈 Key Analysis

### 1. Time-based Demand
- Peak demand: 8–10 AM and 6–8 PM
- Lowest demand: Late night (10 PM – 6 AM)
- Median fare is higher during peak hours

### 2. Geographic Impact
- CBD: High demand, stable prices
- Remote suburbs: Higher fares due to limited supply
- Tourist areas: Higher willingness to pay

### 3. Distance & Time Impact

Linear regression models show strong relationships:

- Drive Time → Fare ↑
- Drive Distance → Fare ↑

The combined model:
Fare = β₁ × Time + β₂ × Distance + ε

suggests that distance has a slightly stronger impact than time.

## 💡 Key Insights

- Uber pricing reflects supply-demand imbalance
- Peak-hour pricing aligns with commuting patterns
- Remote areas have higher fares due to limited drivers
- Distance is a primary pricing driver

## 💼 Business Implications

- Dynamic pricing can be optimized by region and time
- Incentives could improve driver supply in remote areas
- Peak-hour pricing could be further segmented

## 🛠️ Tech Stack
- Python (Pandas, NumPy)
- Matplotlib / Seaborn
- Scikit-learn (Linear Regression)
- Folium (Geospatial Visualization)

## 📌 Author
Hetong Wang
Nina Fan
Xiaojing Liu
Boshen Jiang
Yilin Li
