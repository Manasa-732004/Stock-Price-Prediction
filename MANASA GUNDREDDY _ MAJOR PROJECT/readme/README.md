# Stock Price Prediction & Market Trend Analysis

## 1. Project Overview

This project focuses on analyzing historical stock market data to understand stock price movements and market trends. A basic machine learning approach is also used to predict the next day's closing price.

For this project, Apple Inc. (AAPL) stock data is used.

## 2. Objectives

- Collect and understand historical stock market data
- Clean and preprocess the dataset
- Perform Exploratory Data Analysis (EDA)
- Analyze stock price movements and trading volume
- Create meaningful visualizations
- Perform feature engineering
- Build machine learning models for stock price prediction
- Evaluate and compare the models
- Analyze the prediction results and identify important insights

## 3. Dataset

The dataset contains historical stock market data for Apple Inc. (AAPL).

The data was collected using the Yahoo Finance source through the `yfinance` Python library.

### Dataset Period

- Start Date: January 1, 2018
- End Date: January 1, 2026

### Main Columns

- Open
- High
- Low
- Close
- Adj Close
- Volume

## 4. Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- yfinance
- Jupyter Notebook

## 5. Data Cleaning and Preprocessing

The dataset was inspected using Pandas.

The following preprocessing steps were performed:

- Checked the data types of columns
- Checked for missing values
- Removed missing values where required
- Checked for duplicate records
- Converted the date index into datetime format
- Adjusted the column structure where required

## 6. Exploratory Data Analysis

Exploratory Data Analysis was performed to understand stock price movements, trading volume, and overall market trends.

The analysis included:

- Closing price over time
- Trading volume over time
- High and Low prices
- Opening and Closing prices
- Daily price changes
- Moving averages
- Correlation between numerical variables

## 7. Feature Engineering

Additional features were created from the historical stock data.

### Features Used

- Open
- High
- Low
- Volume
- MA20
- MA50
- Daily_Change
- Price_Range

### Moving Average

MA20 represents the 20-day moving average.

MA50 represents the 50-day moving average.

These features help identify short-term and longer-term price trends.

### Daily Change

Daily Change represents the change in closing price from the previous trading day.

### Price Range

Price Range is calculated as:

High - Low

## 8. Target Variable

The target variable is the next day's closing price.

The target was created by shifting the Closing Price column by one trading day.

## 9. Train-Test Split

The dataset was divided into training and testing data using an 80:20 split.

Since stock data is time-dependent, the chronological order of the data was maintained instead of randomly shuffling the records.

## 10. Machine Learning Models

Two machine learning models were used:

### Linear Regression

Linear Regression was used as the first prediction model to establish a simple baseline for predicting the next day's closing price.

### Random Forest

Random Forest was used as the second model for comparison.

It combines multiple decision trees to make predictions.

## 11. Model Evaluation

The models were evaluated using:

- Mean Absolute Error (MAE)
- Root Mean Squared Error (RMSE)
- R² Score

The model performance was compared using these evaluation metrics.

## 12. Model Comparison

The performance of Linear Regression and Random Forest was compared based on their evaluation metrics.

Based on the obtained results, Linear Regression performed better than Random Forest for this dataset according to the selected evaluation criteria.

## 13. Actual vs Predicted Prices

An Actual vs Predicted Price visualization was created to compare the actual closing prices with the prices predicted by the Linear Regression model.

This visualization helps understand how closely the predicted values follow the actual stock prices.

## 14. Feature Importance

Feature importance was analyzed using the Random Forest model.

The most important features included:

- MA50
- MA20
- High
- Low
- Open

These features contributed more strongly to the Random Forest predictions compared with the other features.

## 15. Key Insights

- AAPL closing prices showed an overall changing trend during the analyzed period.
- Trading volume varied significantly over time.
- Moving averages helped identify price trends.
- The 20-day and 50-day moving averages were useful engineered features.
- The models were able to learn patterns from historical stock data.
- Linear Regression performed better than Random Forest based on the selected evaluation metrics.
- Historical stock prices alone cannot guarantee accurate future predictions.

## 16. Conclusion

This project demonstrated a complete Data Science workflow using historical AAPL stock data.

The project included data collection, data cleaning, exploratory data analysis, visualization, feature engineering, machine learning model development, evaluation, and model comparison.

Linear Regression and Random Forest were trained and evaluated, and Linear Regression showed better performance for this dataset based on the selected evaluation metrics.

The project is intended for educational purposes and should not be considered financial advice or a guarantee of future stock prices.

