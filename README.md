# ProjectML
 📈 Bitcoin Price Prediction using Machine Learning & Mathematical Models
A deep-dive into modeling Bitcoin closing prices using classical regression, machine learning, and time series techniques — with Exponential Fit emerging as the top performer.

📘 Overview
This project aims to predict the closing price of Bitcoin (BTC) using a mix of traditional regression methods, statistical techniques, and machine learning models. The performance of each model is evaluated using multiple error metrics and k-Fold cross-validation.

📊 Dataset
Source: Yahoo Finance

Time Range: Daily data over several years

Features Used:

Open

High

Low

Volume

Market Cap

Target Variable: Close price

⚙️ Preprocessing & Techniques
Cleaned and converted volume/market cap formats

Applied normalization (Min-Max scaling)

Feature selection via correlation analysis

Implemented logarithmic/exponential transformations where applicable

Applied k-Fold Cross-Validation to assess model stability

🧠 Models & Techniques Used
Category	Models/Techniques
Classical Regression	Linear Regression, Logarithmic Fit, Exponential Fit
Statistical Smoothing	SMA50 (50-day Simple Moving Average)
Machine Learning	kNN, Random Forest, Support Vector Regression (SVR)
Deep Learning	LSTM (Long Short-Term Memory networks)

📈 Evaluation Metrics
RMSE (Root Mean Square Error)

MSE (Mean Square Error)

MAE (Mean Absolute Error)

MAPE (Mean Absolute Percentage Error)

R² Score

🥇 Results
Model	Best Metric Value	Notes
Exponential Fit	✅ Lowest errors & highest R²	✅ Best overall performer
Linear Regression	Moderate	Baseline model
Logarithmic Fit	Decent	Slightly underperformed Exp Fit
kNN	Varies	Sensitive to hyperparameters
Random Forest	Good	Solid performance, but slower
SVR	Fair	Required normalization
SMA50	Baseline smoothing	Not predictive, used for trend
LSTM	Experimental	Needs more tuning/data

🧠 Key Insights
Exponential Fit captured BTC price growth trends best, outperforming ML models.

Classical models can rival or beat black-box models on financial time series with the right transformation.

Smoothing methods (like SMA) help in understanding trends but are poor predictors alone.

LSTM had potential but needs much more data and tuning for reliable results.
