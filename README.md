# Quantitative Analysis and Financial Market Forecasting with Machine Learning

## Overview

This project applies Data Science, Quantitative Finance, and Machine Learning techniques for financial asset analysis, risk management, and market movement forecasting.

The study uses historical data from both Brazilian and international financial markets to evaluate:

* risk
* return
* volatility
* diversification
* asset forecasting
* portfolio performance

Additionally, the pandemic period was removed from the analysis due to the structural break caused by extreme market volatility.

---

# Objective

The main objective of this project is to investigate how macroeconomic and financial variables can support financial market forecasting and the development of quantitative investment strategies.

The project also aims to:

* evaluate risk and return
* analyze diversification
* apply quantitative risk metrics
* test Machine Learning models
* perform strategy backtesting

---

# Assets Used

| Asset                | Ticker                 |
| -------------------- | ---------------------- |
| IBOVESPA             | ^BVSP                  |
| S&P500               | ^GSPC                  |
| VIX                  | ^VIX                   |
| US Dollar            | USDBRL=X               |
| Gold                 | GC=F                   |
| IPCA Inflation Index | Central Bank of Brazil |

---

# Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-Learn
* yfinance
* Jupyter Notebook

---

# Methodology

## 1. Data Collection

Historical financial data was collected using:

* Yahoo Finance API
* Central Bank of Brazil API

The analyzed period ranges from 2014 to 2025.

---

## 2. Data Preprocessing

The following procedures were performed:

* data cleaning
* missing value treatment
* temporal alignment
* time series standardization

---

## 3. Pandemic Removal

The pandemic period was removed from the model training process due to the structural break caused by COVID-19 in financial markets.

This approach reduces statistical distortions and improves model stability.

---

## 4. Feature Engineering

Derived variables were created, including:

* logarithmic returns
* rolling volatility
* moving averages
* momentum indicators
* dynamic correlation metrics

---

## 5. Modeling

The Random Forest model was used to identify historical patterns and forecast market behavior.

---

# Financial Metrics

The project applies quantitative financial metrics such as:

* Value at Risk (VaR)
* Conditional Value at Risk (CVaR)
* Volatility
* Correlation
* Drawdown
* Sharpe Ratio
* Cumulative Return

---

# Results

The results demonstrated that:

* diversified portfolios reduced total risk
* the VIX presented the highest volatility
* the S&P500 showed more consistent growth
* gold acted as a hedge asset
* the model identified relevant patterns between macroeconomic variables and market movements

---

# Project Structure

portfolio-analysis/
│
├── data/
├── notebooks/
├── src/
├── images/
├── reports/
├── models/
├── README.md
└── requirements.txt

---

# How to Run

```bash
git clone https://github.com/JPmascena/Portfolio-Analysis.git

cd Portfolio-Analysis

pip install -r requirements.txt

jupyter notebook
```
