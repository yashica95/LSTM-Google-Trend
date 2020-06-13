# Time series Prediction on Google Trend data using LSTM
![](https://github.com/yashica95/LSTM-Google-Trend/blob/master/images/google_trend.png)
### Overview:
This project sought to use LSTM to predict Google Trends data for the keyword -'data science course'. The inspiration for this project is to understand the increasing interest in learning data science and see if we can predict the future trend using LSTM model.

### Data Source:
Data has been collected from Google Trends using [pytrends API](https://github.com/GeneralMills/pytrends)

### Techniques used:
1. Downloaded data using pytrends API for past 4 years
2. Used pytrends API to find daily data by overlapping 
3. USed pandas and numpy for datetime, data preparation by converting dataframe to time series using windows, differencing
4. Normalizing data in range of (0,1)
3. Built LSTM model using Tensorflow, Keras 

### Results:
- Best Train RMSE: 10.59
- Best Test RMSE: 6.38
![](https://github.com/yashica95/LSTM-Google-Trend/blob/master/images/predictions.png)


The code has been highly inspired from https://github.com/mborysiak/Time-Series-Forecasting-with-ARIMA-and-LSTM repository. Thank you. 
