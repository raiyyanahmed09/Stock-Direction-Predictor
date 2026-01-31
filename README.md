# 📈 Stock Direction Predictor using Machine Learning

This project implements a machine-learning based system to predict the **short-term direction (UP/DOWN)** of a stock using historical price data and technical indicators.  
Instead of predicting exact prices, the model outputs **probabilistic directional signals**, making it more realistic for financial decision-making.

---

## 🔍 Problem Statement
Predict whether a stock’s closing price will move **up or down on the next trading day** based on historical market data.

---

## 📊 Data Source
- Historical OHLCV data fetched using **Yahoo Finance (`yfinance`)**

---

## 🧠 Features Used
- Simple Moving Average (10-day, 50-day)
- Relative Strength Index (RSI)
- MACD
- Volume Ratio

---

## 🤖 Model
- **Random Forest Classifier**
- Time-series based train-test split (to avoid data leakage)
- Probability-based decision threshold

---

## 📈 Evaluation
- Precision
- Recall
- Backtested trading strategy vs Buy & Hold
- Visual comparison of cumulative returns

---

## 🖥 Interface
The notebook includes an interactive widget to:
- Input a stock ticker
- Run ML-based analysis
- View prediction, confidence, and historical strategy performance

---

## ⚠ Limitations
- No transaction costs or slippage included
- Model performance may vary across market regimes
- Not intended for live trading without further validation

---

## 🚀 How to Run
```bash
pip install -r requirements.txt
