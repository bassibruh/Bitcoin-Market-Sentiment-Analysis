# Bitcoin Market Sentiment Analysis

## Project Overview

This project analyzes the relationship between Bitcoin market sentiment and trader performance by combining historical trading records with the Bitcoin Fear & Greed Index. The objective is to understand whether market emotions influence trading behavior, profitability, trade size, and overall performance.

---

## Objective

The main objective of this project is to:

- Analyze trader performance under different market sentiment conditions.
- Study how Fear and Greed affect trading decisions.
- Identify patterns in profitability and trading activity.
- Segment traders based on their behavior.
- Build a machine learning model to predict trading profitability.

---

## Datasets Used

### 1. Historical Trading Dataset
Contains detailed information about every trade, including:
- Account
- Coin
- Execution Price
- Trade Size
- Transaction Fee
- Closed PnL
- Trade Direction
- Timestamp

### 2. Bitcoin Fear & Greed Index
Contains daily market sentiment values categorized as:
- Extreme Fear
- Fear
- Neutral
- Greed
- Extreme Greed

---

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Scikit-learn
- Jupyter Notebook

---

## Project Workflow

### Data Preparation
- Loaded both datasets.
- Converted timestamps into datetime format.
- Removed duplicate records.
- Checked missing values.
- Created a common Date column.
- Merged trading data with Fear & Greed Index.

### Exploratory Data Analysis
Performed detailed analysis on:

- Market sentiment distribution
- Trading activity
- Average Closed PnL
- Trade Size
- Transaction Fees
- Buy vs Sell distribution
- Daily Profit/Loss trend
- Win Rate analysis
- Correlation analysis

### Trader Segmentation
Applied **K-Means Clustering** to group trades based on:
- Trade Size
- Closed PnL
- Trading Fee
- Fear & Greed Index

This helped identify different trading behavior patterns.

### Machine Learning
A **Random Forest Regressor** was trained to predict **Closed PnL** using:

- Execution Price
- Trade Size
- Trading Fee
- Fear & Greed Index

Feature Importance analysis was also performed to determine which variables contribute the most to profitability prediction.

---

# Key Findings

### 1. Market sentiment influences trader performance.
Profitability changes across Fear, Neutral and Greed market conditions.

### 2. Trade Size has a strong impact on profitability.
Larger trades generally contribute more significantly to overall profit and loss.

### 3. Trading behavior changes with market sentiment.
Trading activity and trade frequency vary depending on whether the market is fearful or greedy.

### 4. Different trader clusters exist.
K-Means clustering identified multiple trading behavior groups based on trade characteristics and profitability.

### 5. Market sentiment improves analysis.
Including the Fear & Greed Index provides additional context for understanding trading performance.

---

## Business Recommendations

- Reduce position size during Extreme Fear periods to manage downside risk.
- Use market sentiment as an additional risk management indicator.
- Monitor large trades more carefully since they have the highest impact on profitability.
- Segment traders based on historical behavior to design personalized trading strategies.
- Combine market sentiment with historical trade metrics for better decision-making.

---

## Repository Contents

```
Bitcoin-Market-Sentiment-Analysis/
│
├── Bitcoin_Market_Sentiment_Analysis.ipynb
├── Assignment_Report_Bitcoin_Market_Sentiment.docx
├── README.md
```

---

## Conclusion

This project demonstrates how market sentiment can be integrated with historical trading data to better understand trader behavior. Using data analysis, visualization, clustering, and machine learning, the project provides meaningful insights into trading performance and highlights the value of sentiment indicators in financial decision-making.

---

## Author

**Aditya Singh**
