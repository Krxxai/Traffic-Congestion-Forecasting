# 🚦 Traffic Congestion Forecasting & Analysis

## 🎯 Project Overview
An end-to-end machine learning project analyzing 
**48,120 hourly traffic records** across 4 major 
junctions in Pune to forecast congestion patterns 
and deliver operational insights for ride-hailing 
platforms like Uber.

This project was completed under **industry mentor 
guidance** with weekly review cycles on model 
optimization and business insight delivery.

---

## 🛠️ Tools & Technologies
| Tool | Purpose |
|------|---------|
| Python | Core programming language |
| Pandas & NumPy | Data manipulation & analysis |
| Scikit-learn | ML model building & evaluation |
| XGBoost | Gradient boosting model |
| Matplotlib & Seaborn | Data visualization |
| TimeSeriesSplit | Cross validation |
| RandomizedSearchCV | Hyperparameter tuning |

---

## 📁 Project Structure
```
Traffic-Congestion-Forecasting/
├── 01_EDA_Analysis.ipynb          ← Exploratory Data Analysis
├── 02_Modeling.ipynb              ← Model building & evaluation
├── 03_Trained_Models.ipynb        ← Final trained models
├── data_modeling_report.pdf       ← Detailed modeling report
├── peak_hour_analysis_summary.txt ← Peak hour insights
└── README.md
```

---

## 📊 Dataset
- **Source:** Pune Junction Traffic Dataset
- **Size:** 48,120 hourly traffic records
- **Duration:** November 2015 — June 2017
- **Junctions:** 4 major Pune junctions
- **Features:** Date, Time, Junction ID, 
  Vehicle Count

---

## 🔑 Key Findings

### ⏰ Peak Hour Analysis
- Peak congestion window: **7–9 PM**
- Identified using 4 statistical methods:
  - Percentile Analysis
  - Standard Deviation Thresholds
  - Z-Score Testing
  - Moving Average Trends
- Evening peak is **50-60% higher** than 
  daily average

### 🌧️ Weather Impact
- Rain increases peak congestion by 
  **~15-18%**
- Temperature & humidity showed weak 
  correlation
- Precipitation correlation: 0.011

### 📅 Event Impact
- Holidays reduce peak traffic by **~40%**
- Weekend reduction: **~22.7%**
- Saturday stays within 10% of weekday levels

### 🗺️ Junction Insights
- **Junction 1** has highest peak traffic
- Peak increase range: **25.9% to 49.5%**
- **Thursday** is busiest peak day
- **Sunday** is lowest peak day

---

## 🤖 Models Built

| Model | Performance |
|-------|------------|
| Linear Regression | Good baseline |
| Random Forest | ⭐ Best overall |
| Gradient Boosting | Stable results |

### Model Evaluation
- Metric: MAE, RMSE, R² Score
- Validation: TimeSeriesSplit (5 folds)
- Tuning: RandomizedSearchCV
- **No overfitting** — minimal gap between 
  train and test R²

### Feature Importance
- **Lag features** — strongest predictors
- **Time of day** — second most important
- Weather features — minimal impact

---

## 💡 Business Recommendations for Uber
```
1️⃣ Pre-position drivers 30-60 minutes 
   before 7-9 PM peak window

2️⃣ Prioritise Junction 1 for resource 
   allocation — highest congestion

3️⃣ Increase surge pricing during rainy 
   peak hours — 15-18% higher congestion

4️⃣ Reduce driver incentives on holidays
   — 40% lower demand

5️⃣ Thursday evening needs maximum 
   driver availability
```

---

## 📈 Feature Engineering
Created **20+ temporal features** including:
- Lag variables (1hr, 2hr, 24hr)
- Rolling statistics (mean, std)
- Time encodings (hour, day, month)
- Peak hour flags
- Weekend/holiday indicators

---

## 👤 Author
**Krishna Jaiswal**
Data Analyst | Pune, Maharashtra, IN
- 🔗 [LinkedIn](https://www.linkedin.com/in/krishna-jaiswal-83779531a/)
- 💻 [GitHub](https://github.com/Krxxai)
- 📧 krishnajaiswal0904@gmail.com
```
