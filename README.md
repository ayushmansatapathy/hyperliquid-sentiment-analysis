# 📊 Hyperliquid Market Sentiment Analysis  
### Fear & Greed Index vs Trader Behavior

---

## 🔍 Overview

This project analyzes how **market sentiment (Fear vs Greed)** impacts trader behavior and performance on Hyperliquid.

🎯 Objectives:
- Understand trader behavior across sentiment regimes  
- Compare performance (PnL, win rate)  
- Generate **actionable trading strategies**  

---

## 🧠 Key Insights

### 📉 1. Traders Perform Better During Fear

| Metric | Fear | Greed |
|--------|------|-------|
| Win Rate | Higher | Lower |
| Avg PnL | Higher | Lower |

👉 Fear encourages disciplined decisions, while Greed leads to overconfidence.

---

### ⚠️ 2. Risk Increases During Greed

- Trade Size ↑ **+34.5%**  
- Leverage ↑ **+15.2%**  
- Long Bias ↑ **48% → 62%**  

👉 Higher risk → lower performance  

---

### 🏆 3. Best Trader Profile

✔ Low trading frequency  
✔ Moderate leverage  
✔ Consistent win rate (>50%)  

👉 Most stable and profitable segment  

---

## 📁 Dataset

### 📊 Fear & Greed Index
- Daily sentiment data (2018–2025)  
- Categories: Extreme Fear → Extreme Greed  

### 📈 Hyperliquid Trading Data
- ~6000 trades  
- Includes:
  - Trade size  
  - Buy/Sell side  
  - PnL  
  - Timestamp  

---

## ⚙️ Methodology

### 1. Data Preparation
- Cleaned missing values & duplicates  
- Converted timestamps to daily format  
- Merged sentiment + trading data  

### 2. Feature Engineering
- Daily PnL  
- Win rate  
- Trade size  
- Trade frequency  
- Long/Short ratio  

### 3. Analysis
- Performance comparison (Fear vs Greed)  
- Behavioral changes  
- Trader segmentation:
  - High vs Low frequency  
  - High vs Moderate leverage  

---

## 📊 Visual Analysis

The project includes:

- 📈 Win Rate by Sentiment  
- 💰 Avg PnL per Trade  
- 📊 Trade Size Analysis  
- 🔄 Long vs Short Behavior  
- 📉 Trader Clustering (PCA, Radar)  

---

## 🎯 Strategy Recommendations

### 🚀 Strategy 1: Fear-Day Contrarian


IF sentiment = Fear:
Increase position size (+20%)
Prefer LONG positions
Take profit = 8%
Stop loss = -4%


👉 Expected improvement: **+15–20%**

---

### 🚀 Strategy 2: Segment-Based Strategy

| Trader Type | Greed | Fear |
|------------|------|------|
| High Frequency | Reduce size (-40%) | Maintain |
| Low Frequency | Slight reduction | Increase size (+25%) |

---

### 🚀 Strategy 3: Sentiment-Based Exit

- Greed → exit early (5%)  
- Fear → let profits run (8%)  

---

## 📁 Project Structure

```bash
hyperliquid-sentiment-analysis/
│
├── data/
│   ├── raw/                    # Original datasets
│   └── processed/              # Cleaned & transformed data
│
├── models/                     # Trained ML models
│   ├── clustering_scaler.pkl
│   ├── gradient_boosting_model.pkl
│   ├── kmeans_model.pkl
│   ├── random_forest_model.pkl
│   └── sentiment_encoder.pkl
│
├── notebooks/                  # Analysis notebooks
│   ├── eda.ipynb
│   └── predictive_modeling_clustering.ipynb
│
├── outputs/                    # Visualizations & results
│   ├── feature_importance.png
│   ├── model_comparison.png
│   ├── optimal_clusters.png
│   ├── performance_by_sentiment.png
│   ├── trader_archetypes_radar.png
│   └── trader_clusters_pca.png
│
├── src/                        # Utility scripts (if any)
│
├── README.md
└── requirements.txt

## ⚠️ Limitations

- Limited number of traders  
- Approximate leverage calculation  
- Short trading time window  
- Exchange-specific data  

---

## 🔮 Future Work

- Build predictive ML model for profitability  
- Add real-time sentiment integration  
- Create interactive dashboard  
- Expand to multiple exchanges  

---

## 🧾 Conclusion

Market sentiment significantly influences trader behavior and performance.

💡 Key takeaway:
> Traders perform better during Fear due to disciplined decision-making.

👉 Smart trading approach:
- Reduce risk during Greed  
- Stay disciplined during Fear  

---

## 🙌 Acknowledgment

- Fear & Greed Index: Alternative.me  
- Hyperliquid trading dataset  

---
