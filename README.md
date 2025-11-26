# Predicting Price Moves with News Sentiment

A data science project analyzing financial news headlines to understand their impact on stock price movements.  
This repository contains data cleaning, exploratory data analysis (EDA), topic modeling, sentiment analysis, and time-series insights.

---

## 📌 Project Structure

project/
│── data/
│ └── raw_analyst_ratings.csv
│── notebooks/
│ ├── EDA_Descriptive_Stats.ipynb
│ ├── EDA_Text_Analysis.ipynb
│ ├── EDA_TimeSeries_Analysis.ipynb
│ └── EDA_Publisher_Analysis.ipynb
│── src/
│── README.md
│── requirements.txt
│── .gitignore


## 🧪 Task 1 – Exploratory Data Analysis (EDA)

- Cleaned and processed dataset  
- Performed descriptive statistics  
- Headline length & word count analysis  
- Extracted keywords + LDA topic modeling  
- Publication time-series analysis  
- Publisher distribution and activity  
- Generated four Jupyter notebooks

🚀 Task 2 — Technical Indicator & Financial Analysis of Stock Prices

The second part of the project focuses on market data

📊 Task 2 Steps
1. Load & Clean Price Data

Loaded CSVs into DataFrames

Standardized column names

Ensured date index

Added ticker field

2. Apply Technical Indicators (TA-Lib)

  Computed for each stock:

    -  SMA (20, 50)

    -  EMA (20)

    -  RSI (14)

    -  MACD (Line, Signal, Histogram)

    -  Bollinger Bands

Each stock DataFrame now contains all indicators.

3. Use PyNance for Portfolio Metrics

Included:

   - Max Sharpe ratio portfolio

   - Minimum variance portfolio

    - Portfolio weights

    - Portfolio report generation

4. Visualizations

Generated:

- Price + SMA + Bollinger Bands plots

- Volume trends

- MACD & RSI visualizations

- Portfolio summary report (portfolio_report.html)

🎯 Task 3 – News Sentiment & Stock Correlation

- Processed 100,000 news headlines with TextBlob sentiment analysis

- Calculated daily stock returns for 6 tech stocks (AAPL, AMZN, GOOG, META, MSFT, NVDA)

- Computed Pearson correlations between daily sentiment scores and stock returns

- Key Findings: AAPL (r=0.32), AMZN (r=-0.43), GOOG/NVDA weak correlations