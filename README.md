 # 📈 Crypto Sentiment vs Trade Outcome Analysis

This project explores the relationship between **cryptocurrency market sentiment** (Fear & Greed Index) and **trade outcomes** (Closed PnL) using historical trading data for BTC and ETH.

### 🔗 [View Full Notebook in Google Colab](https://colab.research.google.com/drive/1TzHdXP2lmfM7QfApNtEBMkE__STU7qOq?usp=sharing)

---

## 📊 Project Overview

This notebook analyzes:
- Individual crypto trades (`historical_data.csv`)
- Daily sentiment scores (`fear_greed_index.csv`)

It investigates how trader performance correlates with sentiment levels like **Extreme Fear** and **Extreme Greed**.

---

## 🧹 Data Preparation
- Merged trade and sentiment data on timestamp
- Removed outliers using IQR method
- Filtered coins with >300 trades (BTC and ETH remained)
- Cleaned and engineered features for modeling

---

## 📊 Exploratory Data Analysis (EDA)
- Visualized PnL distribution, sentiment classifications, and trade volumes
- Found BTC had slightly better average PnL
- Identified trade patterns across sentiment states

---

## 🧠 Predictive Modeling
Two regression models were used to predict logged `Closed PnL`:
- **Random Forest**
  - R²: `0.1734`, RMSE: `0.1300`
- **XGBoost**
  - R²: `0.1970`, RMSE: `0.1281`

---

## 💡 Key Findings
- There is modest predictive power in using sentiment + trade features to forecast outcomes.
- Visualizations indicate a pattern of profitability depending on sentiment classification.

---
 

## 📁 Files Required
- `historical_data.csv`
- `fear_greed_index.csv`

 

