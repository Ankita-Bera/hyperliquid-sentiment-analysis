# Trader Performance vs Market Sentiment (Hyperliquid)

## Overview
This project analyzes how Bitcoin market sentiment (Fear vs Greed) affects trader behavior and performance on the Hyperliquid exchange. By combining the Fear & Greed Index with historical trading data, we investigate patterns in trading outcomes and derive simple strategy recommendations.

---

## Setup

1. Clone the repository

git clone https://github.com/Ankita-Bera/hyperliquid-sentiment-analysis.git

cd hyperliquid-sentiment-analysis


2. Install required libraries

pip install pandas numpy matplotlib seaborn jupyter


3. Place the datasets in the project folder.

Fear & Greed dataset  
Historical Trader Data (Hyperliquid) dataset  

---

## How to Run

Open the Jupyter Notebook:

jupyter notebook trade.ipynb

Run the notebook cells step by step to reproduce the analysis and charts.

---

## Output Charts / Tables

The notebook generates the following visualizations:

- Average PnL by market sentiment
- Win rate by sentiment
- Trade frequency by sentiment
- Average trade size by sentiment

These charts help understand how trader performance and behavior change across different market conditions.

---

## Methodology

1. **Data Preparation**
   - Loaded the sentiment dataset and Hyperliquid trading dataset.
   - Checked dataset size, missing values, and duplicates.
   - Converted timestamps and aligned both datasets by date.

2. **Feature Engineering**
   Key metrics were created:
   - Daily PnL per trader
   - Win rate
   - Average trade size
   - Number of trades per day
   - Long/short ratio

3. **Analysis**
   - Compared trader performance across sentiment categories.
   - Examined behavioral changes such as position sizes and trading activity.
   - Identified patterns between market sentiment and trading outcomes.

---

## Key Insights

1. **Trader losses are highest during Extreme Fear markets.**  
   The average PnL is most negative during Extreme Fear, indicating that panic-driven markets are difficult to trade profitably.

2. **Win rates improve during positive sentiment.**  
   Extreme Greed sentiment shows the highest win rate, suggesting that bullish market conditions lead to more successful trades.

3. **Trade sizes vary with sentiment.**  
   Traders tend to take larger positions during Fear sentiment, possibly attempting to capture market rebounds.

---

## Strategy Recommendations

**Strategy 1 — Reduce risk during Fear markets**

During Fear or Extreme Fear sentiment:
- Reduce leverage
- Use smaller position sizes
- Trade cautiously

These periods show higher losses and market uncertainty.

**Strategy 2 — Take advantage of Greed markets**

During Greed or Extreme Greed sentiment:
- Favor long positions
- Trade moderately more frequently
- Follow momentum strategies

Positive sentiment tends to create stronger price trends.

---

## Conclusion

The analysis shows that market sentiment has a noticeable impact on trader behavior and performance. Fear-driven markets tend to produce larger losses, while Greed sentiment provides better trading conditions. Incorporating sentiment indicators into trading strategies may help traders manage risk and improve decision-making.
