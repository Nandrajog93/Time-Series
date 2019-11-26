# Time-Series-Forecasting
This repository conatins Time-Series Analysis on Bombay Stock Exchange using 3 methods:

What is Time-Series?

A time series is a sequence where a metric is recorded over regular time intervals.

Depending on the frequency, a time series can be of yearly (ex: annual budget), quarterly (ex: expenses), monthly (ex: air traffic), weekly (ex: sales qty), daily (ex: weather), hourly (ex: stocks price), minutes (ex: inbound calls in a call canter) and even seconds wise (ex: web traffic).


Now forecasting a time series can be broadly divided into two types.

If you use only the previous values of the time series to predict its future values, it is called Univariate Time Series Forecasting.

And if you use predictors other than the series (a.k.a exogenous variables) to forecast it is called Multi Variate Time Series Forecasting.

Methods:

1) ARIMA (Auto Regressive Integrated Moving Average)
2) Prophet
3) LSTM Neural Network

Method 1.

What is ARIMA?

ARIMA projects the future values of a series based entirely on it's own intertia. It perfrom best when your data exhibts a stable or consist patter over a time.

Basic concept:
Step1 : Check the Stationarity [Data remain at a fairly constant level over time]

[When we Talk about stock market data keeps ob fluctuating therefore, data is not stationary, so ARIMA is not useful.
ARIMA is good for predicting seasonlable goods or market]

Ques) How to predict stock price using ARIMA?

Ans) convert the non stationarity data in stationary by subtracting the observation in current period from thr previous one this technique is called defferencing.

Here We are using Mixed model which build on the combination of AR(autoregressive) & MA(Moving average).

Non-sesional ARIMA(p,d,q) --> P: The no. of time lags., d: Degree of differencing., q: Is the order of moving avg.

P (Autoregressive) : It checks the last 3 values of model. Let's say if it is warm then next day is also be warm.

d (Integrated part of the model) : It is like the difference of previous temprature with current temprature

q (Moving average): It allow us to set the error of the model as the linear combination of the error values observed at the previous point in the past.


Method 2.

What is Prophet?

Prophet is a procedure for forecasting time series data based on an additive model where non-linear trends are fit with yearly, weekly, and daily seasonality, plus holiday effects. It works best with time series that have strong seasonal effects and several seasons of historical data. Prophet is robust to missing data and shifts in the trend, and typically handles outliers well.

Method 3.

What is LSTM

https://colah.github.io/posts/2015-08-Understanding-LSTMs/



