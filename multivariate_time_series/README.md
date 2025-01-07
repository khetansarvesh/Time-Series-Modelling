# <ins> Multivariate Time-Series-Forecasting (>1 feature dataset) </ins>
Like Univariate Analysis here also we can have algorithms for different types of trend, we will look more closely at finding out <ins> overall trend </ins> in the data. There are many algorithms which can help you decode overall trend present in the time series data :
- Multiple Linear Regression
  
- [most used model] Vector AutoRegression (VAR)
    - [Blog 1](https://www.analyticsvidhya.com/blog/2018/09/multivariate-time-series-guide-forecasting-modeling-python-codes/)
    - [Blog 2](https://towardsdatascience.com/prediction-task-with-multivariate-timeseries-and-var-model-47003f629f9)
    - [Blog 3](https://towardsdatascience.com/multivariate-time-series-forecasting-653372b3db36)
- VARX
    - Same as var but in var we had only single order of  lag but here we can specify our own order of lags.No of lags is decided by acf and pacf plot
- Vector Autoregression Moving-Average (VARMA)
- [Vector Autoregression Moving-Average with Exogenous Regressors (VARMAX)](https://www.statsmodels.org/dev/examples/notebooks/generated/statespace_varmax.html)
- VMA
- ARIMAX
- Deep Learning
    - FFNN
    - RNN
    - [LSTM](https://www.youtube.com/watch?v=tepxdcepTbY)
    - GRU
    - Transformers
