# ProjectML

📈 **Bitcoin Price Prediction using Machine Learning & Mathematical Models**

A deep-dive into modeling Bitcoin closing prices using classical regression, machine learning, and time series techniques — with **Exponential Fit** emerging as the top performer.

---

## 📘 Overview

This project aims to predict the closing price of Bitcoin (BTC) using a mix of traditional regression methods, statistical techniques, and machine learning models. The performance of each model is evaluated using multiple error metrics and **k-Fold cross-validation**.  

To enhance model reliability and generalization:
- I applied **Grid Search**, **Random Search**, and a **custom Hybrid Search** (combining both approaches) for hyperparameter tuning.
- Models were **fine-tuned individually** for optimal performance.
- A **short time series analysis** was conducted to identify trend dynamics and stationarity.
- **Technical analysis indicators** were used as features to help capture market behavior.
- Elements of **fundamental analysis** and **psychological analysis** (market sentiment & investor behavior) were considered to contextualize trends and modeling.

---

## 📊 Dataset

- **Source:** Yahoo Finance  
- **Time Range:** Weekly data over several years  
- **Features Used:**
  - Open  
  - High  
  - Low  
  - Volume  
  - **Technical indicators used for feature selection:**
    - RSI  
    - MACD  
    - OBV  
    - Williams %R  
- **Target Variable:** Close price

---

## ⚙️ Preprocessing & Techniques

- Cleaned and converted to weekly chart  
- Applied normalization (Min-Max scaling)  
- Feature selection via correlation analysis  
- Applied k-Fold Cross-Validation to assess model stability  
- Applied hyperparameter tuning via Grid Search, Random Search, and Hybrid Search  
- Incorporated time series decomposition and smoothing

---

## 🧠 Models & Techniques Used

**Technical Indicators Used for Features:**

- SMA50 (50-day Simple Moving Average)  
- RSI  
- MACD  
- Williams %R  

**Models Used:**

- Linear Regression  
- Logarithmic Fit  
- Exponential Fit  
- kNN  
- SMA50  
- Random Forest  
- SVR  
- LSTM  

---

## 📏 Evaluation Metrics

- RMSE (Root Mean Square Error)  
- MSE (Mean Squared Error)  
- MAE (Mean Absolute Error)  
- MAPE (Mean Absolute Percentage Error)  
- R² Score  

---

## 🥇 Results

| Model             | Best Metric Value             | Notes                               |
|------------------|-------------------------------|-------------------------------------|
| Exponential Fit   | ✅ Lowest errors & highest R² | ✅ Best overall performer            |
| Linear Regression | Moderate                      | Baseline model                      |
| Logarithmic Fit   | Decent                        | Slightly underperformed Exp Fit     |
| kNN               | Varies                        | Sensitive to hyperparameters        |
| Random Forest     | Good                          | Solid performance, but slower       |
| SVR               | Fair                          | Required normalization              |
| SMA50             | Baseline smoothing            | Not predictive, used for trend only |
| LSTM              | Experimental                  | Needs more tuning/data              |

![image](https://github.com/user-attachments/assets/fd4b55f5-93fb-4bd8-af68-502751bbea03)

---

## 🔍 Key Insights

- Exponential Fit captured BTC price growth trends best, outperforming ML models.  
- Classical models can rival or beat black-box models on financial time series with the right transformation (especially for assets like Bitcoin with steady exponential growth).  
- Smoothing methods (like SMA) help in understanding trends but are poor predictors alone.  
- LSTM had potential but needs much more data and tuning for reliable results.  
- Combining domain knowledge from **technical, fundamental, and psychological analysis** adds practical value to the modeling process and improves interpretation of results.

---

