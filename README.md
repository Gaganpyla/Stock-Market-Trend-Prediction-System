# 📈 Stock Market Trend Prediction System

[![Python 3.8+](https://img.shields.io/badge/Python-3.8%2B-blue.svg)](https://www.python.org/)
[![yfinance](https://img.shields.io/badge/Data-yfinance-green.svg)](https://github.com/ranaroussi/yfinance)
[![Matplotlib](https://img.shields.io/badge/Library-Matplotlib-orange.svg)](https://matplotlib.org/)
[![Pandas](https://img.shields.io/badge/Library-Pandas-red.svg)](https://pandas.pydata.org/)

## 📌 Project Overview
This project is a technical analysis tool designed to predict stock market trends and backtest trading strategies using **Moving Average Crossovers**. It automates the process of fetching historical stock data, calculating technical indicators (SMA/EMA), generating buy/sell signals, and evaluating strategy performance through comprehensive financial metrics.

## 🚀 Key Features
* **Automated Data Retrieval**: Fetches real-time and historical stock data directly from Yahoo Finance using the `yfinance` API.
* **Dual MA Strategy**: Supports both **Simple Moving Average (SMA)** and **Exponential Moving Average (EMA)** crossovers.
* **Comprehensive Backtesting**: Simulates trading over a specified period to calculate:
    * **Total Return %**
    * **CAGR** (Compound Annual Growth Rate)
    * **Sharpe Ratio** (Risk-adjusted return)
    * **Max Drawdown** (Portfolio risk)
    * **Win Rate** & Average Trade Return.
* **Visual Analytics**: Generates clear, high-resolution plots showing:
    * Price crossovers with Buy/Sell markers.
    * Strategy Equity Curves (Normalized).
* **Trade Logging**: Outputs a tabular summary of every buy/sell event for audit and analysis.

## 🛠️ Technical Stack
* **Language:** Python
* **Data Handling:** `Pandas`, `NumPy`
* **Data Source:** `yfinance`, `pandas_datareader`
* **Visualization:** `Matplotlib`
* **Formatting:** `tabulate`

## 📊 Strategy Logic
The system generates signals based on the interaction between a **Short-window MA** (Faster) and a **Long-window MA** (Slower):
1.  **Buy Signal (Golden Cross)**: Triggered when the short-term average crosses above the long-term average.
2.  **Sell Signal (Death Cross)**: Triggered when the short-term average crosses below the long-term average.

## 🚀 Getting Started

### 1. Installation
Install the required Python libraries:
```bash
pip install pandas numpy matplotlib yfinance tabulate pandas_datareader
```
### Key Sections explained:
1.  **Project Overview**: Describes the core goal of using technical analysis for trend prediction.
2.  **Backtesting Metrics**: Lists the specific financial formulas implemented in your notebook (CAGR, Sharpe, etc.).
3.  **Basic Usage**: Provides a code snippet that matches your actual function signature (`MovingAverageCrossStrategy_YF`).
4.  **Strategy Logic**: Clearly explains the crossover rules that drive the code.
