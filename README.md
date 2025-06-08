
# 🪙 ABC Gold – Procurement Strategy Dashboard (2024–2025)

> **Tools Used**: Python, Pandas, Plotly, Scikit-learn, Statsmodels, Power BI  
> **Dataset Sources**: Internal sales data, gold market prices, GoldBees ETF data

---

## 📌 Project Overview

ABC Gold is a premium jewellery retailer operating in a volatile gold pricing environment. The objective of this project is to:

- Analyze sales and pricing patterns
- Reduce financial risk from price fluctuations
- Inform **data-driven procurement strategies**

This solution combines **data science**, **visualization**, and **machine learning** to support better buying decisions and boost profitability.

---

## 📊 Datasets

### 🔹 Raw Data Files:
- `Sales Data 1.csv` – Sales from Apr 2024 to Sept 2024  
- `Sales Data 2.csv` – Sales from Oct 2024 to Mar 2025  
- `Daily Rate Capture.csv` – Daily metal prices (gold, silver, platinum)  
- `GoldBees Data.csv` – Indian gold ETF data (market price reflection)

### 🔹 Cleaned Datasets:
- `Sales Data.csv` – Merged and cleaned sales records  
- `Daily Rate Capture.csv` – Cleaned pricing dataset  
- `GoldBees Data.csv` – Cleaned ETF dataset  

**Cleaning Steps**:
- Missing value imputation  
- Unit standardization  
- Z-score based outlier removal  
- Date/time parsing  
- One-hot encoding  
- Type casting and formatting

---

## 📈 Exploratory Data Analysis (EDA)

Conducted using `Trend_and_Pattern_Analysis.ipynb`:

### Insights Explored:
- 📅 Monthly sales trends and seasonal peaks
- 📈 Profit/Loss correlation with purchase behavior
- 🗓️ Impact of Muhurtham (auspicious days) on pricing
- 🔍 Anomaly detection using **Local Outlier Factor (LOF)**

### Techniques Used:
- Descriptive statistics & group-wise aggregation  
- K-Means clustering with Elbow Method  
- Seasonal decomposition & trend smoothing  
- Correlation heatmaps

---

## 🤖 Predictive Modeling & Risk Analysis

Performed in `ML models.ipynb`:

### ✅ Volatility Modeling
- **GARCH Model**: Measures gold price volatility to inform bulk purchase decisions  
  📌 *Insight*: Market volatility is currently low → favorable for high-volume procurement

- **Bollinger Bands**: Used to detect overbought/oversold zones  
  📌 *Action*: Buy near lower band, avoid near upper band

### ✅ Anomaly Detection
- **Local Outlier Factor (LOF)**: Flags abnormal transactions (sudden spikes, price manipulation, etc.)

### ✅ Customer Segmentation
- **K-Means Clustering** yields:
  - Cluster 0: High-margin, low-volume customers  
  - Cluster 1: Low-margin, low-frequency buyers  
  - Cluster 2: Bulk buyers

---

## 📊 Power BI Dashboard

Built in `ABC_Gold_Insights.pbix`, this dynamic dashboard offers:

### Dashboard Highlights:
- 📆 Monthly overview of purchases and sales  
- 📉 Net Profit/Loss trends  
- 🧊 Cluster-based customer segments  
- 📦 Transaction patterns & pricing insights  
- 🧠 Actionable KPIs for procurement decisions

---

## 📂 Files Included

| File | Description |
|------|-------------|
| `Sales Data.csv` | Cleaned, merged sales data |
| `Daily Rate Capture.csv` | Cleaned metal prices |
| `GoldBees Data.csv` | ETF data for Indian gold market |
| `Trend_and_Pattern_Analysis.ipynb` | EDA and visual analysis |
| `ML models.ipynb` | Predictive modeling and risk analysis |
| `ABC_Gold_Insights.pbix` | Power BI Dashboard |
| `Project report.pdf` | Project summary report |

---

## 🔍 Key Insights

| Focus Area | Insight |
|------------|---------|
| 🪙 Volatility Control | GARCH & Bollinger Bands recommend low-risk purchase windows |
| 📈 Sales Trends | High volatility; peak months influence inventory timing |
| 🔍 Anomaly Detection | LOF detects irregular pricing/volume transactions |
| 👥 Customer Segments | Data-backed segmentation enables targeted marketing |
| 📊 Strategy Drivers | MA7 trends > Weekday/Festival pricing logic |

---

## 🚀 Recommendations

- Delay purchases when prices touch the **upper Bollinger Band**
- Prioritize buying during **low volatility periods** (GARCH signal)
- Use **LOF anomalies + MA7** for stock reordering signals
- Plan promotions and inventory for **identified seasonal peaks**

---

## 🧠 Final Reflections

This project exemplifies how **data science** can enhance strategic decision-making in volatile markets. By fusing time series modeling, anomaly detection, and customer clustering into a visual decision-support tool, **ABC Gold** can:

- Mitigate financial risks  
- Time purchases more effectively  
- Personalize engagement with buyer segments  
- Gain a long-term competitive edge

---

