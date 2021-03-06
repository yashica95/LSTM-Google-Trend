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
### Method 1: Using Moving Average
![](https://github.com/yashica95/LSTM-Google-Trend/blob/master/images/predictions.png)

### Method 2: Using Differencing
![](https://github.com/yashica95/LSTM-Google-Trend/blob/master/images/prediction_differencing.png)

The code has been highly inspired from https://github.com/mborysiak/Time-Series-Forecasting-with-ARIMA-and-LSTM repository. Thank you. 

### Method 3: Facebook Prophet ( For curiosity) 
![](https://github.com/yashica95/LSTM-Google-Trend/blob/master/images/facebook_prophet_prediction.png)

**Trends detected by Facebook Prophet**
![](https://github.com/yashica95/LSTM-Google-Trend/blob/master/images/facebook_prophet.png)

**Key Observations** :

1. The trend is upwards therefore suggesting an increasing trend in learning data science courses
2. Interestingly, Mondays have the highest search trend whereas the search trend falls on weekends
3. July to September are the top months for searches, which coincides well with the summer holidays in most parts of the world
