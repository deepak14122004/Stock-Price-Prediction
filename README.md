**Stock Price Prediction using Bidirectional LSTM**

This project focuses on predicting stock prices using a Bidirectional Long Short-Term Memory (LSTM) model. The model leverages historical stock data, including moving averages, to predict future stock prices. The repository contains code, data preprocessing steps, and evaluation metrics for the predictive model.

**Project Overview**

This project utilizes a Bidirectional LSTM model to predict future stock prices based on historical data. Moving averages of different periods are used to capture trends, and the model is trained to forecast the closing prices. The project aims to demonstrate the effectiveness of deep learning in time series forecasting.

**Dataset**

The dataset consists of historical stock prices for a company, which includes the following columns:

Date: The date of the stock price
Open: The opening price
High: The highest price for the day
Low: The lowest price for the day
Close: The closing price of the stock
Volume: The volume of stocks traded
Additional features were created:

MA_10: 10-day moving average
MA_50: 50-day moving average
MA_100: 100-day moving average

**Features**

The model uses the following features for prediction:

Close: The actual closing price
MA_10: 10-day moving average
MA_50: 50-day moving average
MA_100: 100-day moving average

**Model Architecture**

The model is built using a Bidirectional LSTM with the following structure:

Layer 1: Bidirectional LSTM (50 units) with return sequences
Dropout: 20% to prevent overfitting

Layer 2: Bidirectional LSTM (50 units) without return sequences
Dropout: 20%

Output Layer: Dense layer with 1 unit to predict the closing price
The model is trained using the Adam optimizer and the mean squared error loss function.

