# Stock price analysis, prediction, and visualization

# Overview:
This project involves analyzing and visualizing financial data for various stocks in different sectors, such as Apple (AAPL), Amazon (AMZN), Google (GOOG), and Microsoft (MSFT) from the technology sector. In this repo, there are three different models: Baseline model(4 stocks, LSTM, no tuning), Optimized model(4 stocks,Deep LSTM, Optuna) and Extended optimized model (Extended version of Optimised model with 13 stocks).

# Data Explotary:
1. Moving Averages:
   - Moving averages (10-day, 20-day, and 50-day) are calculated to smooth fluctuations and identify trends.

2. Correlation Analysis:
   - Correlation between stocks is calculated to understand their relationships.
   - A heatmap visualizes these correlations.
  

# Model Prediction
1. Data Loading and Preprocessing:
   - Historical stock prices are loaded from CSV files for multiple companies.
   - Daily closing prices are extracted and cleaned for analysis.
   - Normalization
   - Encoding stock indices using LableEncoding()

2. Hyperparameter Optimization using Optuna

5. Next Value Prediction (LSTM):
   - LSTM networks are implemented to predict the next day's stock price based on historical data.
   - The LSTM model uses past sequences of stock prices as input and predicts future prices.

7. Visualization:
   - Exploratory data.
   - Training and validation loss plots.
   - Predicted vs. actual stock prices are plotted to evaluate the performance of the LSTM model.


   # Requirements:
   - Python 3.x
   - Libraries: pandas, numpy, matplotlib, tensorflow/keras
