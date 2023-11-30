# Cryptomatter-project

### Data Overview

- Bitcoin tweets from 01.01.2017 to 26.11.2022
     (Username, Handle, Date, Text, Reply_cnt,Retweet_cnt, Like_cnt)
- Bitcoin data from Binance
     (first_currency, second_currency, UNIX timestamp, open, high, low, close,    volume)
- BTC trading data 
    (Date, MarketCap, TradeVolume, ClosePrice)

### Parsing tweets from Twitter

- Selenium web parses was used to get all Bitcoin related Tweets.
- As a parameters for proper data capturing we used:
- Minimum # of tweets
- Data range corresponding our BTC data
- Optionally (Retweets, Shares, etc)

### Data Understanding: Sentiments for Tweets

- Our aim is to know what was the mood of people about  Bitcoin on a specific day.
- We derived sentiment intensity of each tweet and grouped it by a Date

### Our dataset:
- 4 exogenous variables (positive, neutral, negative, block reward)
- 1 time series variable – closing price
- Since the value tn−1 is required to predict tn, and tn−1 is unknown, a recursive process is applied in which, each new prediction, is based on the previous one. This process is known as recursive forecasting or recursive multi-step forecasting

