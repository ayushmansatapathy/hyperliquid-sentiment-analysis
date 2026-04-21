# 📊 Market Sentiment Analysis: Fear & Greed vs Trader Behavior (Hyperliquid)

## 🔍 Overview

This project analyzes how **market sentiment (Fear vs Greed)** affects trader behavior and performance on Hyperliquid.

🎯 Goal:
- Understand behavioral patterns
- Measure performance differences
- Build **actionable trading strategies**

---

## 🧠 Key Insights

### 1. Traders Perform Better During Fear 😮

| Metric | Fear | Greed |
|--------|------|-------|
| Win Rate | Higher | Lower |
| Avg PnL | Higher | Lower |

👉 **Insight:**  
Fear leads to disciplined trading, while Greed causes overconfidence.

---

### 2. Risk Increases During Greed

- Trade size ↑ **+34.5%**
- Leverage ↑ **+15.2%**
- Long bias ↑ **48% → 62%**

👉 More risk → worse performance

---

### 3. Best Trader Profile 🏆

✔ Low trading frequency  
✔ Moderate leverage  
✔ Consistent win rate (>50%)  

👉 Most stable and profitable

---

## 📁 Dataset

### 1. Fear & Greed Index
- Daily sentiment data (2018–2025)
- Categories: Fear → Extreme Greed

### 2. Hyperliquid Trades
- ~6000 trades
- Fields: size, side, PnL, timestamp

---

## ⚙️ Methodology

1. Data cleaning & preprocessing  
2. Date alignment (daily level)  
3. Feature engineering:
   - Win rate  
   - Avg PnL  
   - Trade size  
   - Long/short ratio  
4. Segmentation:
   - High vs Low frequency  
   - High vs Moderate leverage  

---

## 📊 Analysis Performed

- Performance comparison (Fear vs Greed)
- Behavioral changes (size, leverage, bias)
- Trader segmentation
- Visualization (PnL, win rate, distribution)

---

## 🎯 Strategy Recommendations

### 🚀 Strategy 1: Fear-Day Contrarian


IF sentiment = Fear:
Increase position size (+20%)
Prefer LONG positions
Wider profit targets (8%)


👉 Expected improvement: **+15–20%**

---

### 🚀 Strategy 2: Segment-Based Adjustment

| Trader Type | Greed | Fear |
|------------|------|------|
| High Frequency | Reduce size (-40%) | Normal |
| Low Frequency | Slight reduction | Increase size (+25%) |

---

### 🚀 Strategy 3: Sentiment-Based Exit

- Greed → exit early (5%)
- Fear → let profits run (8%)

---

## 📁 Project Structure


hyperliquid-sentiment-analysis/
│
├── data/
│ ├── fear_greed_index.csv
│ └── historical_data.csv
│
├── notebook.ipynb
├── README.md
├── requirements.txt


---

## ⚠️ Limitations

- Limited trader sample size  
- Approximate leverage calculation  
- Short trading time window  
- Exchange-specific data  

---

## 🔮 Future Improvements

- Add ML prediction model  
- Build Streamlit dashboard  
- Cluster trader behavior  
- Real-time sentiment integration  

---

## 🧾 Conclusion

Market sentiment strongly impacts trader behavior.

💡 Key takeaway:
> Traders perform better during Fear because they act more cautiously.

👉 Smart traders should:
- Reduce risk during Greed  
- Stay disciplined during Fear  

---

## 🙌 Acknowledgment

- Fear & Greed Index: Alternative.me  
- Hyperliquid trading data  
