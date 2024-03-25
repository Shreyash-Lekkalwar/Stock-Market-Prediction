Stock Market Trend Prediction with Random Forest Classifier

This project aims to predict the trend of the S&P 500 stock market index using historical data. It utilizes the yfinance library to fetch historical stock market data and then trains a Random Forest Classifier model to predict whether the market will go up or down on the next trading day.
Installation

Before running the code, make sure to install the required dependencies:

bash

pip install yfinance

Data Collection

The historical data of the S&P 500 index is fetched using the yfinance library. If the data is already saved as "sp500.csv", it is loaded; otherwise, the data is fetched from Yahoo Finance and saved for future use.
Data Preprocessing

The fetched data is preprocessed, including converting the index to datetime format and removing unnecessary columns such as Dividends and Stock Splits.
Model Training

A Random Forest Classifier model is trained using historical data features such as Close price, Volume, Open price, High price, and Low price. The model is trained to predict whether the market will go up or down on the next trading day based on these features.
Model Evaluation

The trained model's performance is evaluated using precision score, which measures the ratio of correctly predicted upward trends to the total predicted upward trends.
Feature Engineering

Additional features are engineered from the historical data, including rolling averages and trend indicators over different time horizons. These features aim to capture more complex patterns in the data and improve the model's predictive performance.
Improved Model Training

The Random Forest Classifier model is retrained using the newly engineered features. Predictions are made using this improved model, and the model's performance is evaluated again.
Conclusion

This project demonstrates how machine learning techniques can be applied to predict stock market trends using historical data. By leveraging Random Forest Classifier and feature engineering techniques, it aims to provide insights into the potential future direction of the market.
