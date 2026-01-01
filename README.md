---

# 📈 Stock Market Price Forecasting with RNN & LSTM

## 📌 Project Overview

This project focuses on **next-day stock price prediction** using **Recurrent Neural Networks (RNN)** and **Long Short-Term Memory (LSTM)** models.
Historical stock market data is used to train and evaluate both models, and their performances are compared using standard regression metrics.

---

## 🎯 Objective

The main objectives of this project are:

* Predict the **next-day closing price** of a stock using historical data
* Implement and compare **RNN** and **LSTM** models
* Evaluate models using **MSE, RMSE, and MAE**
* Analyze which model performs better on time-series stock data

---

## 📊 Dataset

* Source: **Yahoo Finance Stock Market Dataset**
* Accessed via: Kaggle / Yahoo Finance API
* Features used:

  * `Open`
  * `High`
  * `Low`
  * `Close`
  * `Volume`

The dataset contains daily stock price data over multiple years.

---

## 🧹 Data Preparation

The following preprocessing steps were applied:

* Handling missing values
* Sorting data by date
* Feature selection
* Feature engineering:

  * Weekly Moving Average (MA7)
  * Monthly Moving Average (MA30)
* Train/Test split:

  * 80% Training
  * 20% Testing
* Data scaling using **MinMaxScaler**
* Creation of time-series sequences (window size = 60 days)

---

## 🧠 Models Implemented

### 🔹 RNN Model

* Two `SimpleRNN` layers
* Dropout layers to reduce overfitting
* Dense output layer
* Optimizer: Adam
* Loss function: Mean Squared Error (MSE)

### 🔹 LSTM Model

* Two `LSTM` layers
* Dropout layers
* Dense output layer
* Optimizer: Adam
* Loss function: Mean Squared Error (MSE)

---

## 📐 Evaluation Metrics

Both models were evaluated using:

* **MSE (Mean Squared Error)**
* **RMSE (Root Mean Squared Error)**
* **MAE (Mean Absolute Error)**

Predicted values were inverse-transformed to compare results in the original price scale.

---

## 📈 Results & Visualization

* Line plot comparing:

  * Actual Close Prices
  * RNN Predictions
  * LSTM Predictions
* Bar charts comparing:

  * MSE (RNN vs LSTM)
  * RMSE (RNN vs LSTM)
  * MAE (RNN vs LSTM)

### 🔍 Key Observation

The **LSTM model consistently achieved lower error values** compared to the RNN model, indicating better performance in capturing long-term dependencies in stock price data.

---

## 🏁 Conclusion

* Both RNN and LSTM models can predict stock price trends reasonably well.
* **LSTM outperformed RNN** in terms of accuracy and stability.
* LSTM is more suitable for complex time-series forecasting tasks like stock price prediction.

---

## 🛠 Technologies Used

* Python
* NumPy
* Pandas
* Matplotlib
* Scikit-learn
* TensorFlow / Keras
* Jupyter Notebook / Kaggle

---


---

## 👤 Author

* **Amirhoseein Kargarfard**
* MCI Bootcamp Project

---

اگر خواستی:

* README رو فارسی کنم
* یا نسخه حرفه‌ای‌تر برای رزومه / پورتفولیو بنویسم
* یا badge و لینک Kaggle اضافه کنم

بگو 👌
