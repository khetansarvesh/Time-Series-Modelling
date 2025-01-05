# <ins> Univariate Time-Series-Forecasting (1 feature dataset) </ins>

There are many types of trend that you can figure out from the data, namely Overall Trend / Seasonal Trend / Cyclical Trend / Irregular Trend

# 1. Overall Trend

### [1.1] <ins> Temporal Dependence Models </ins>
We can make forecast of tomorrow’s weather by observing the weather of past few days. If the weather was sunny for last 4–5 days then there is high chance for weather to be sunny tomorrow. This is an intuitive way of understanding temporal dependence model. The correlation between past and present values shows temporal dependence. In this model, we give heavy weights to recent data than the older data points

- [Method of Semi Averages](https://github.com/khetansarvesh/Time-Series-Modelling/blob/main/univariate_time_series/Semi%20Average%20Model.pdf)
- [Moving Average (MA) Model](https://github.com/khetansarvesh/Time-Series-Modelling/blob/main/univariate_time_series/MA.pdf)
- [Least Squares Model](https://github.com/khetansarvesh/Time-Series-Modelling/blob/main/univariate_time_series/Least%20Squares%20Model.pdf)
- [Auto Regression (AR) Model](https://www.youtube.com/watch?v=Ia9irWcWt8s)
- [Auto Regressive Moving Average (ARMA) Model](https://www.youtube.com/watch?v=8t11SmVD8dU)
- [Auto Regressive integrated Moving Average (ARIMA) Model](https://www.youtube.com/watch?v=8FCDpFhd1zk)
  - ARIMA requires data to have constant mean and variance with no seasonality.
  - If data doesn’t satisfy the above conditions, lets say, if we have a data points that has a upward trend, then to use ARIMA we first need to apply transformation on it, and make it stationary 
- AUTO ARIMA Model
- SARIMA Model
- Deep Learning (DL) Models
    - FFNN Model
    - 1D CNN Model
    - Hidden Markov Models (HMM)
    - Conditional Random Fields (CRF)
    - Recursive Neural Network (RvNN) Model
    - [1990s] Recurrent Neural Network (RNN) Model - Unidirectional
    - Bidirectional RNN Model - Bidirectional
    - [1997] LSTM RNN Model - Unidirectional
    - Bidirectional LSTM RNN Model - Bidirectional
      - LSTM => 4 hidden layer stacked LSTM RNN architecture to solve the univariate time series forcasting problem of google stock price prediction using pytorch deep learning library.
    - [2014] Gated RNN Model - Unidirectional
    - Bidirectional Gated RNN Model - Bidirectional 
    - Transformer Encoder Model - Bidirectional 
    - Transformer Decoder Model - Unidirectional


In my notes I have given a detailed explaination of how one can solve the univariate time series problem using even a FFNN but since there exists a problem in solving with FFNN it motivated the idea of RNN, what is this problem?? Read my notes to understand same. Now there exists a problem with RNN i.e. vanishing and exploding gradients which motivates the idea of LSTMs and since these exists a problem with LSTMs it motivated the idea of GRUs. To solve the parallel computation problem with GRUs the idea of transformer based models poped up.










### [1.2] <ins> General Additive Model (GAM) </ins>
Instead of using correlation between values from similar time stamps, we can train our model on overall trends and add some seasonal effect to it. The principle behind GAM is similar to that of regression model. Unlike regression which uses individual predictor for outcome, GAM uses sum of smooth function to predict the outcome. The smooth functions here includes functions describing trend component, seasonal component, holiday component and so on. As GAM comprises of functions, we can isolate the individual function and evaluate its effect in prediction, which makes GAM more interpretable.

- [FBProphet](https://www.youtube.com/watch?v=09tg5fU4T6A)




# 2. Seasonal Trend : Decoding short term trends in univariate time series data
These include algorithms like 
- [Method of Simple Average](https://github.com/khetansarvesh/Time-Series-Modelling/blob/main/univariate_time_series/seasonal_trend/Simple%20Average.pdf)
- [Ratio to Trend Method](https://github.com/khetansarvesh/Time-Series-Modelling/blob/main/univariate_time_series/seasonal_trend/Ratio%20To%20Trend.pdf)
- Ratio To Moving Average Method
- Link Relatives Method
- SARIMA (Seasonal Arima)
