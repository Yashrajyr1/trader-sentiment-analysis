# 📊 Trader Performance vs Market Sentiment Analysis
> This project focuses not just on data analysis, but on extracting behavioral insights that can inform real-world trading strategies.

## 📌 Objective
This project analyzes how Bitcoin market sentiment (Fear vs Greed) influences trader behavior and performance on Hyperliquid. The goal is to uncover patterns that can inform more effective and risk-aware trading strategies.

---

## 📌 Datasets Used
1. Bitcoin Market Sentiment (Fear/Greed Index)  
2. Historical Trader Data (Hyperliquid)

---

## 📌 Methodology

### 1. Data Cleaning
- Standardized column names across datasets
- Converted timestamps into datetime format
- Aligned both datasets on daily granularity
- Checked and handled missing values and duplicates

### 2. Feature Engineering
Created key metrics:
- Daily PnL per trader
- Win rate
- Trade frequency (trades per day)
- Average position size
- Long/Short ratio
- Trader consistency (based on win rate)

### 3. Analysis
- Compared trader performance across sentiment regimes
- Analyzed behavioral changes (trade frequency, size, direction)
- Performed segmentation:
  - Frequent vs Infrequent traders
  - Consistent vs Inconsistent traders

---

## 📌 Key Insights

- Traders are more active during **Fear phases** than Greed, indicating panic-driven or reactive trading behavior.
- Position sizes remain high during Fear, suggesting lack of effective risk management.
- Traders show **contrarian behavior**:
  - More short positions during Extreme Greed
  - Continued long bias during Fear (attempting reversals)
- A large portion of profits comes from **inconsistent traders**, indicating high-risk, high-reward dynamics.
- **Consistent traders perform best in Neutral markets**, where conditions are more stable.

> Overall, trader performance is strongly influenced by behavioral biases rather than sentiment alone.

---

## 📌 Strategy Recommendations

### 1. Risk Control in Fear Markets
- Reduce trade frequency and position sizes  
- Avoid aggressive positioning  
- Focus on capital preservation  

---

### 2. Controlled Contrarian Strategy in Greed
- Use selective short positions  
- Avoid over-leveraging  
- Time entries carefully  

---

### 3. Segment-Based Strategy
- Allocate more capital to **consistent traders in stable markets**
- Limit exposure to **inconsistent traders during volatile phases**

---

### 4. Sentiment Timing Strategy
- Avoid trading during extreme sentiment spikes  
- Enter trades after volatility stabilizes  

---

## 📌 Additional Report

A concise summary of insights and strategy recommendations is also available in PDF format for quick review:

- `insights_strategy.pdf`

## 📌 How to Run

```bash
pip install pandas matplotlib seaborn
jupyter notebook
