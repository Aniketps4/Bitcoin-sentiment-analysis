# 📊 Trader Behavior Insights Dashboard

This project explores the relationship between **Bitcoin market sentiment** (Fear/Greed Index) and **trader performance** using historical trading data from Hyperliquid.

---

## 🔍 Overview

**Objective:**  
Analyze how trader behavior and profitability vary under different market sentiments (Fear vs. Greed), and uncover insights that could guide smarter trading strategies.

---

## 📁 Dataset Descriptions

### 1. `fear_greed_index.csv`
- `date`: Calendar date (YYYY-MM-DD)
- `value`: Sentiment score (0–100)
- `classification`: Either `"Fear"` or `"Greed"`

### 2. `historical_data.csv`
- `Account`: Trader identifier
- `Coin`: Traded asset (e.g., BTC)
- `Execution Price`, `Size USD`, `Closed PnL`, etc.
- `Timestamp IST`: Trade time
- Other metadata for each trade

---

## 📊 Features of the Streamlit Dashboard

- **Sentiment Distribution Bar Chart**
- **Closed PnL Distribution by Sentiment (Boxplot)**
- **Daily Average PnL Trend Line Chart**
- **Aggregated Stats Table**: Avg. PnL, trade size, fees, etc.
- **T-Test**: Statistical test for PnL difference between Fear and Greed days

---

## 🚀 How to Run in Google Colab

### 1. Upload the two CSV files:
- `fear_greed_index.csv`
- `historical_data.csv`

### 2. Install dependencies:
```bash
!pip install streamlit pyngrok --quiet
