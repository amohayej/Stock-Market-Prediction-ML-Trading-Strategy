# Stock-Market-Prediction-ML-Trading-Strategy
This project implements a machine learning-based trading strategy using historical stock data from Yahoo Finance. It applies technical indicators and trains an XGBoost classifier to predict next-day price direction, then evaluates performance through cumulative returns and ROC analysis.

Computing technical indicators:
RSI (14-day)
MACD and Signal line
SMA(10) and SMA(50)
Rolling volatility (10-day standard deviation)

Feature Engineering:
Merges all indicators into a single dataset.
Defines the target variable as the next-day price direction (up = 1, down = 0).

Model Training:
Splits data into 80% training and 20% testing sets.
Trains an XGBoost binary classifier with logloss evaluation metric.

Evaluation:
Computes confusion matrix and ROC curve.
Reports AUC = 0.52985492373, indicating modest predictive power.
Simulates trading performance based on model predictions
