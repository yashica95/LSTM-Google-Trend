# Time series Prediction on Google Trend data using LSTM
![](https://github.com/yashica95/LSTM-Google-Trend/blob/master/images/google_trend.png)
### Overview:
This project sought to use LSTM to predict Google Trends data for the keyword -'data science course'. The inspiration for this project is to understand the increasing interest in learning data science and see if we can predict the future trend using LSTM model.

### Data Source:
Data has been collected from Google Trends using [pytrends API](https://github.com/GeneralMills/pytrends)

### Techniques used:
1. Downloading data using pytrends API
2. pandas and numpy for datetime, data preparation 
3. Tensorflow for LSTM modeling

### Results:
- Best Train RMSE: 10.59
- Best Test RMSE: 6.38
![](https://github.com/yashica95/LSTM-Google-Trend/blob/master/images/predictions.png)
