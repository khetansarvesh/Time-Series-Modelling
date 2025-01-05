# Time-Series-Modelling

# <ins> Univariate Time Series Analysis </ins>
### 1. Overall Trend
### 2. Seasonal Trend
### 3. Cyclic Trend
### 4. Irregular Trend

# <ins> Multivariate Time Series Analysis </ins>

### 1. Overall Trend
There are many algorithms which can help you decode overall trend present in the time series data 
a. Multiple Linear Regression
b. Vector AutoRegression (VAR)
c. VARX - (same as var but in var we had only single order of  lag but here we can specify our own order of lags.No of lags is decided by acf and pacf plot)
d. VARMAX
e. VMA
f. ARIMAX
g. Deep Learning 
    - FFNN
    - RNN
    - LSTM
    - GRU
    - Transformers


### 2. Seasonal Trend
### 3. Cyclic Trend
### 4. Irregular Trend



In my notes I have given a detailed explaination of how one can solve the univariate time series problem using even a FFNN but since there exists a problem in solving with FFNN it motivated the idea of RNN, what is this problem?? Read my notes to understand same. Now there exists a problem with RNN i.e. vanishing and exploding gradients which motivates the idea of LSTMs and since these exists a problem with LSTMs it motivated the idea of GRUs. To solve the parallel computation problem with GRUs the idea of transformer based models poped up.


# LSTM

4 hidden layer stacked LSTM RNN architecture to solve the univariate time series forcasting problem of google stock price prediction using pytorch deep learning library.


# Transformer-Encoder


