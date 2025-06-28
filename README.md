# 📈 Stock Price Prediction using LSTM in Python

This project uses a Long Short-Term Memory (LSTM) neural network to predict stock prices based on historical data fetched using Yahoo Finance. It demonstrates data preprocessing, model training, and visualizing predicted vs. actual prices.

## 🔍 Overview

- **Data Source:** Yahoo Finance (`yfinance`)
- **Target Feature:** `Close` price of a stock
- **Model:** LSTM neural network
- **Frameworks:** TensorFlow / Keras, scikit-learn, pandas, matplotlib

## 🧠 Model Architecture

- `LSTM` (100 units) with `return_sequences=True`
- `Dropout` (20%)
- `LSTM` (100 units)
- `Dropout` (20%)
- `Dense` output layer (1 unit)

The model uses the previous 60 days of closing prices to predict the next day's price.

## 📊 Example Used

- **Stock Ticker:** AAPL (Apple Inc.)
- **Date Range:** 2015-01-01 to 2021-01-01

You can modify the `stock_symbol` in the script to predict other tickers like `TSLA`, `GOOGL`, etc.

## 📁 File Structure

stock-price-prediction-lstm/
├── stock_lstm_prediction.py # Main script (or .ipynb for Jupyter/Colab)
├── README.md # Project documentation


## 🚀 How to Run the Project

### ✅ Prerequisites

Ensure the following Python libraries are installed:

```bash
pip install numpy pandas matplotlib yfinance scikit-learn tensorflow


python stock_lstm_prediction.py


📉 Output
The model plots and compares:

🔴 Actual Stock Prices

🔵 Predicted Stock Prices

It also prints the Mean Squared Error (MSE) for model evaluation.

🧪 Evaluation Metric
Mean Squared Error (MSE) is used to evaluate prediction accuracy.

🛠 Future Improvements
Tune LSTM hyperparameters for better performance

Use additional features like Open, High, Low, Volume

Deploy the model as a web app (using Flask or Streamlit)

Integrate live prediction with real-time stock APIs

