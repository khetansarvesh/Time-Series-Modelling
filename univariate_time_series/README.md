# <ins> Univariate Time-Series-Forecasting (1 feature dataset) </ins>

There are many types of trend that you can figure out from the data, namely Overall Trend / Seasonal Trend / Cyclical Trend / Irregular Trend

# 1. Overall Trend

These are also called sequential models because we are using them to solve a sequential problem. Whichever algorithm gives the best predictive results is considered and evaluation metrics remain the same as what we discussed in the cross sectional data regression problem. 

<ins> Temporal Dependence Models </ins> : We can make forecast of tomorrow’s weather by observing the weather of past few days. If the weather was sunny for last 4–5 days then there is high chance for weather to be sunny tomorrow. This is an intuitive way of understanding temporal dependence model. The correlation between past and present values shows temporal dependence. In this model, we give heavy weights to recent data than the older data points

- Least Squares
- Auto Regression (AR)
- Moving Average (MA)
- Auto Regressive Moving Average (ARMA)
- Auto Regressive integrated Moving Average (ARIMA)
- AUTO ARIMA
- SARIMA
- Deep Learning (DL)
    - FFNN
    - RNN
    - LSTM => 4 hidden layer stacked LSTM RNN architecture to solve the univariate time series forcasting problem of google stock price prediction using pytorch deep learning library.
    - GRU
    - Transformers 

<ins> General Additive Model (GAM) </ins> : Instead of using correlation between values from similar time stamps, we can train our model on overall trends and add some seasonal effect to it. The principle behind GAM is similar to that of regression model. Unlike regression which uses individual predictor for outcome, GAM uses sum of smooth function to predict the outcome. The smooth functions here includes functions describing trend component, seasonal component, holiday component and so on. As GAM comprises of functions, we can isolate the individual function and evaluate its effect in prediction, which makes GAM more interpretable.

- FBProphet




# 2. Seasonal Trend : Decoding short term trends in univariate time series data
These include algorithms like 
- [Method of Simple Average](https://github.com/khetansarvesh/Time-Series-Modelling/blob/main/seasonal_trend/Simple%20Average.pdf)
- [Ratio to Trend Method](https://github.com/khetansarvesh/Time-Series-Modelling/blob/main/seasonal_trend/Ratio%20To%20Trend.pdf)
- Ratio To Moving Average Method
- Link Relatives Method
- SARIMA (Seasonal Arima)