# 📈 Stock Market Forecasting using Time Series Models & LSTM  

A time series forecasting project comparing **classical models (ARIMA, SARIMAX, Prophet)** with a **Stacked LSTM** neural network to predict stock closing prices and forecast short-term market behavior.  

---

## 📌 Overview  

This project explores different approaches to **time series forecasting** on stock market data. Using 5 years of historical stock prices (2015–2020), the goal was to predict short-term future prices and compare how **statistical models** vs. **deep learning models** perform on financial data.  

🔑 **Key finding** → Traditional models capture trends but struggle with volatility, while LSTMs provide a strong historical fit but face challenges in forecasting due to noisy, non-stationary markets influenced by external factors (news, sentiment, earnings, etc.).  

---

## 🧰 Tools & Technologies  

- Python  
- TensorFlow / Keras  
- Statsmodels  
- Facebook Prophet  
- Pandas & NumPy  
- Matplotlib & Seaborn  

---

## 📊 Workflow  

1. **Data Source**: Historical stock data from Yahoo Finance (`AAPL.csv`)  
2. **Data Preprocessing**:  
   - Index reset and closing price extraction  
   - Stationarity checks (ADF test)  
   - Train-test split and scaling (for LSTM)  
3. **Modeling**:  
   - **ARIMA / SARIMAX** → for statistical baselines  
   - **Facebook Prophet** → for trend + seasonality detection  
   - **Stacked LSTM** → deep learning sequence model with sliding windows (150-day input → 1-day prediction)  
4. **Evaluation & Plotting**:  
   - Visualized predicted vs. actual stock prices  
   - Extended predictions for **next 50 days** using recursive forecasting  
   - Compared models on trend-capturing ability vs. volatility handling  
5. **Results**:  
   - **ARIMA/SARIMAX**: captured basic trends, limited forecasting accuracy  
   - **Prophet**: good trend detection, missed volatility  
   - **LSTM**: strong historical fit, weaker generalization for future forecasting  

---

## 📈 Key Features  

- End-to-end pipeline for time series forecasting  
- Comparison of classical vs. deep learning approaches  
- 150-day sliding window with 50-day future prediction (LSTM)  
- Actual vs. Predicted visualization across models  
- Insights on limitations of time series-only forecasting in financial markets  

---

## 📎 How to Run  

1. Clone the repository  
2. Place `AAPL.csv` in the root directory  
3. Run the notebooks:  
   - `Stock_Market_Forecasting_ARIMA_SARIMAX_Prophet.ipynb` → Classical models  
   - `Stock_Market_Forecasting_LSTM.ipynb` → LSTM model  
4. View plots for **actual vs. predicted** and **future 50-day forecast**  

---

## 📂 Files  

- `Stock_Market_Forecasting_ARIMA_SARIMAX_Prophet.ipynb` – Classical time series models  
- `Stock_Market_Forecasting_LSTM.ipynb` – Deep learning model  
- `AAPL.csv` – Dataset (not included; fetch from Yahoo Finance)  
- `README.md` – Project documentation  

---
