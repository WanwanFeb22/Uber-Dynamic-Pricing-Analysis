# Uber Dynamic Pricing Analysis (Sydney)

## 📊 Project Overview
This project analyzes Uber trip data in Sydney to identify key drivers of ride pricing and understand the mechanism behind dynamic pricing systems.

The dataset contains over 30,000 Uber trips, which were cleaned and filtered to 23,717 valid observations for analysis.

---

## 🎯 Key Objectives
- Identify the main factors influencing Uber fares  
- Analyze demand patterns across time and location  
- Quantify the impact of distance and duration on pricing  
- Provide data-driven insights into dynamic pricing strategies  

---

## ⚙️ Data Processing
- Removed irrelevant columns (Trip ID, country, postal data)
- Dropped missing suburb values
- Filtered invalid trips:
  - Duration < 5 mins or > 60 mins removed  
  - Negative or zero fare/distance removed  
- Converted datetime features for time-based analysis  

---

## 📈 Analysis & Findings

### 🕒 Time Impact
- Peak demand: **8–10 AM and 6–8 PM**
- Higher fares during commuting hours
- Lower and more stable prices during late night

### 📍 Location Impact
- CBD: high demand, stable pricing  
- Remote suburbs: higher fares due to limited driver supply  
- Tourist areas: higher willingness to pay  

### 📏 Distance & Duration Impact

Regression model:
Fare = β₁ × Time + β₂ × Distance

Key findings:
- Both variables strongly influence pricing  
- Distance has a slightly stronger effect than time  

---

## 💡 Key Insights
Uber pricing reflects a dynamic balance between:
- Demand (time of day)
- Supply (location)
- Trip characteristics (distance & duration)

---

## 💼 Business Implications
- Dynamic pricing can be optimized using time + location signals  
- Remote areas may require driver incentives to improve supply  
- Peak-hour pricing could be further segmented for efficiency  

---

## 🛠️ Tech Stack
Python, Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn, Folium  

---

## 📂 Project Files
- Notebook: full data analysis and modeling  
- Report: detailed explanation  
- Slides: presentation summary  

---

## 👤 Author
Hetong Wang (UNSW FinTech)  
