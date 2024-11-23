# Stock Analysis and Visualization

# Overview:
This project involves analyzing and visualizing financial data for various stocks in different sectors, such as Apple (AAPL), Amazon (AMZN), Google (GOOG), and Microsoft (MSFT) from the technology sector. It combines traditional stock analysis techniques with machine learning methods, such as LSTM (Long Short-Term Memory) networks for next-value prediction and Particle Swarm Optimization (PSO) for hyperparameter tuning. The goal is to study stock trends and predict future stock prices.

# Features:
1. Data Loading and Preprocessing:
   - Historical stock prices are loaded from CSV files for multiple companies.
   - Daily closing prices are extracted and cleaned for analysis.

2. Moving Averages:
   - Moving averages (10-day, 20-day, and 50-day) are calculated to smooth fluctuations and identify trends.

3. Risk vs. Return Analysis:
   - Daily percentage returns are computed.
   - Expected return (average daily return) and risk (standard deviation of returns) are calculated.
   - A scatter plot visualizes the tradeoff between risk and return.

4. Correlation Analysis:
   - Correlation between stocks is calculated to understand their relationships.
   - A heatmap visualizes these correlations.

5. Next Value Prediction (LSTM):
   - LSTM networks are implemented to predict the next day's stock price based on historical data.
   - The LSTM model uses past sequences of stock prices as input and predicts future prices.
   - Feature scaling and supervised learning transformation are applied to preprocess the data for LSTM.

6. Hyperparameter Optimization (PSO):
   - Particle Swarm Optimization (PSO) is used to optimize the `sequence_length` hyperparameter of the LSTM model.
   - PSO helps find the optimal size of sliding window for feature engineering by minimizing prediction errors (MSE).

7. Visualization:
   - Subplots show trends for individual stocks, including their moving averages.
   - Risk-return scatter plots and correlation heatmaps summarize the analysis visually.
   - Predicted vs. actual stock prices are plotted to evaluate the performance of the LSTM model.

# How to Run:
1. Requirements:
   - Python 3.x
   - Libraries: pandas, numpy, matplotlib, seaborn, tensorflow/keras, pyswarm (for PSO)

2. Steps:
   - Place the stock price CSV files in a folder.
   - Run the preprocessing script to clean and prepare the data.
   - Execute the analysis script to calculate moving averages, risk, and correlations.
   - Train the LSTM model for the next value prediction using historical data.
   - Use PSO to optimize the LSTM hyperparameters.
   - Visualize the analysis results, including predicted vs. actual prices.

3. Outputs:
   - Subplots for stocks showing closing prices and moving averages.
   - Scatter plot of risk vs. return with annotated stock labels.
   - Heatmap showing stock correlations.
   - Predicted vs. actual stock price plots from the LSTM model.

# Insights:
- Moving averages highlight short-term, intermediate, and long-term trends.
- Risk-return analysis compares the volatility and returns of different stocks.
- Correlation analysis reveals relationships between stocks, guiding diversification.
- LSTM predictions provide insights into future stock movements based on historical patterns.
- PSO enhances the LSTM model by finding optimal sequence lengths for improved prediction accuracy.
