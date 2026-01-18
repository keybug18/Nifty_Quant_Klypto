# 📈 NIFTY 50 Quantitative Trading System

**Regime-Aware Trading Strategy with Machine Learning Enhancement**

---

## 🧠 Project Overview
An end-to-end quantitative trading pipeline for **NIFTY 50 intraday data**, focused on:
- Correct methodology
- Regime awareness
- Time-safe machine learning

The project builds a **rule-based baseline strategy** and improves it using **ML & Deep Learning**.

---

## 🎯 Objective
- Detect market regimes
- Build a baseline trading strategy
- Enhance trade quality using ML
- Evaluate performance on unseen data

---

## 🏗️ Pipeline
Synthetic Data <br>
↓<br>
Data Cleaning<br>
↓<br>
Feature Engineering<br>
↓<br>
Regime Detection (HMM)<br>
↓<br>
Baseline Strategy<br>
↓<br>
ML / LSTM Enhancement<br>


---

## 📊 Data
- **Type:** Synthetic (realistic & reproducible)
- **Period:** Jan 2024 – Jan 2025
- **Frequency:** 5-minute
- **Instruments:** NIFTY Spot, Futures, Options

✅ ~99.87% data retained after cleaning

---

## 🧩 Features
- Log returns
- EMA indicators & EMA spread
- Rolling volatility
- Market regime labels (HMM)

---

## 🔍 Regime Detection
- Hidden Markov Model (HMM)
- Identifies: **Uptrend / Sideways / Downtrend**
- Used as **context**, not direct signals

---

## 📉 Baseline Strategy
- Rule-based, regime-aware
- Short-biased during bearish regimes
- Serves as benchmark (no ML)

### 📈 Test Performance
- Trades: ~313  
- Win Rate: ~31%  
- Total Return: ~11.4%  
- Sharpe Ratio: ~1.34  

---

## 🤖 Machine Learning Layer
ML is used to **filter low-quality trades**, not predict prices.

### Models Used
- Logistic Regression
- Random Forest
- XGBoost
- LSTM (time-series modeling)

### Training
- Time-based train/test split
- No shuffling (no data leakage)

---

## ⚠️ Limitations
- Synthetic data
- No transaction costs
- No live deployment

---

## 🚀 Future Work
- Live data integration
- Position sizing & risk management
- Portfolio-level optimization

---

## 📂 Repository Structure
├── 01_data_acquisition.ipynb
├── 02_data_cleaning.ipynb
├── 03_feature_engineering.ipynb
├── 04_regime_detection.txt
├── 05_baseline_strategy.ipynb
├── 06_model_training.ipynb
├── 07_outlier.ipynb
├── README.md
