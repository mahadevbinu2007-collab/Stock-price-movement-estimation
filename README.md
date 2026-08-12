# Stock Price Movement Estimation 📈

A machine learning project designed to predict the daily price movement of META stock using historical market data and technical indicators. 

## Overview
This project utilizes a **Random Forest Classifier** to forecast whether a stock's price will close higher or lower on the following trading day. The model processes over a decade of historical data, relying on engineered financial features to identify market trends, momentum, and volatility. 

## Key Features
* **Exploratory Data Analysis (EDA):** Visualizes long-term stock trajectories and major market events (2012–Present).
* **Feature Engineering:** Incorporates standard technical analysis indicators used by professional traders:
  * 20-Day & 50-Day Simple Moving Averages (SMA)
  * Price Volatility
  * Relative Strength Index (RSI)
  * Moving Average Convergence Divergence (MACD)
  * Bollinger Bands
* **Predictive Modeling:** Implements a Random Forest algorithm trained on a strict chronological 80/20 train-test split to prevent data leakage.
* **Model Interpretability:** Includes Feature Importance visualization to reveal which technical indicators carry the most predictive weight.

## Tech Stack
* **Language:** Python
* **Environment:** Google Colab / Jupyter Notebook
* **Libraries:** `pandas`, `numpy`, `matplotlib`, `scikit-learn`

## Results
The initial baseline model achieved a directional accuracy of **51.15%**. While predicting the stock market is inherently complex, this baseline demonstrates the pipeline's ability to ingest raw market data, clean it, generate momentum signals, and identify subtle predictive patterns.

## How to Use
1. Clone this repository to your local machine.
2. Open the `.ipynb` notebook in Google Colab or your preferred local Jupyter environment.
3. Ensure the target dataset (`META_things.csv`) is placed in the correct working directory.
4. Run all cells sequentially to preprocess the data, train the classification model, and generate the evaluation charts.
