Time series modelling usually deals with regression task on time series based dataset, below we will see algorithms to do this!!

# <ins> Univariate Time-Series-Forecasting (1 feature dataset) </ins>
There are many types of trend that you can figure out from the data, namely Overall Trend / Seasonal Trend / Cyclical Trend / Irregular Trend
### 1. Overall Trend



In my notes I have given a detailed explaination of how one can solve the univariate time series problem using even a FFNN but since there exists a problem in solving with FFNN it motivated the idea of RNN, what is this problem?? Read my notes to understand same. Now there exists a problem with RNN i.e. vanishing and exploding gradients which motivates the idea of LSTMs and since these exists a problem with LSTMs it motivated the idea of GRUs. To solve the parallel computation problem with GRUs the idea of transformer based models poped up.


LSTM => 4 hidden layer stacked LSTM RNN architecture to solve the univariate time series forcasting problem of google stock price prediction using pytorch deep learning library.



### 2. Seasonal Trend : Decoding short term trends in univariate time series data
These include algorithms like 
- [Method of Simple Average](https://github.com/khetansarvesh/Time-Series-Modelling/blob/main/seasonal_trend/Simple%20Average.pdf)
- [Ratio to Trend Method](https://github.com/khetansarvesh/Time-Series-Modelling/blob/main/seasonal_trend/Ratio%20To%20Trend.pdf)
- Ratio To Moving Average Method
- Link Relatives Method
- SARIMA (Seasonal Arima)



# <ins> Multivariate Time-Series-Forecasting (>1 feature dataset) </ins>
Like Univariate Analysis here also we can have algorithms for different types of trend, we will look more closely at finding out <ins> overall trend </ins> in the data. There are many algorithms which can help you decode overall trend present in the time series data :
- Multiple Linear Regression
- Vector AutoRegression (VAR)
- VARX - (same as var but in var we had only single order of  lag but here we can specify our own order of lags.No of lags is decided by acf and pacf plot)
- VARMAX
- VMA
- ARIMAX
- Deep Learning
    - FFNN
    - RNN
    - LSTM
    - GRU
    - Transformers



