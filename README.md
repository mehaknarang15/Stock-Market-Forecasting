# 📈 Stock Market Forecasting using LSTM

A time series forecasting project using **Stacked LSTM** to predict stock closing prices and forecast the next 30 days of market behavior.

---

## 📌 Overview

This project demonstrates the use of deep learning (Stacked LSTM) to model and predict stock market trends. It uses historical stock data (2015–2020) to train a sequential model and predict future closing prices with a focus on short-term forecasting.

---

## 🧰 Tools & Technologies

- Python  
- TensorFlow / Keras  
- Pandas & NumPy  
- Matplotlib  
- LSTM (Long Short-Term Memory Neural Network)  

---

## 📊 Workflow

1. **Data Source**: Historical stock data from Yahoo Finance (`AAPL.csv`)  
2. **Data Preprocessing**:  
   - Index reset and closing price extraction  
   - MinMax Scaling for normalization  
   - Sequence generation for time series modeling  
3. **Model**:  
   - Built a **Stacked LSTM** model with multiple LSTM layers  
   - Trained on past 100 days of data to predict the next day  
4. **Evaluation & Plotting**:  
   - Visualized predicted vs actual stock prices  
   - Extended prediction for future **30 days** using recursive input  
5. **Results**:  
   - Accurate short-term trend capture  
   - Future price range estimation with plotted line chart

---

## 📈 Key Features

- Stacked LSTM architecture for better sequence learning  
- Future 30-day forecasting using last known window  
- Original vs Predicted closing price visualization  
- No data shuffling to preserve temporal integrity  

---

## 📎 How to Run

1. Clone the repository  
2. Place `AAPL.csv` in the root directory  
3. Run the notebook `Stock_Market_Forecasting.ipynb`  
4. View plots for actual vs predicted and 30-day forecast

---

## 📂 Files

- `Stock_Market_Forecasting.ipynb` – Main notebook  
- `AAPL.csv` – Dataset (not included; fetch from Yahoo Finance)  
- `README.md` – Project documentation  

---

## 📌 Future Improvements

- Compare LSTM with ARIMA and Prophet models  

