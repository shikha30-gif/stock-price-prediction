Stock Price Prediction 
A machine learning app that predicts next-day closing prices for Nifty 50 stocks (the top 50 Indian stock exchange companies) using XGBoost.
Data fetching — pulls 2 years of historical price data for any Nifty 50 stock (e.g., RELIANCE.NS, TCS.NS) via Yahoo Finance
Feature engineering — computes technical indicators: moving averages (5/10/20-day), volatility, price returns, volume change, high-low spread, and RSI (Relative Strength Index)
Model training — trains an XGBoost regression model per stock to predict the next day's closing price, with an 80/20 train-test split
Prediction — loads the trained model, pulls recent data, and forecasts the next close, showing predicted price, expected % change, and a bullish/bearish signal
Interface — wraps everything in a Gradio web app with two tabs: one to predict prices for a selected stock, one to manually train/retrain a model
