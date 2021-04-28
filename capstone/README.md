# Problem Statement
One of the famous quotes from Warren Buffet on investing, “Rule No. 1: Never lose money. Rule No. 2: Never forget rule No.1”. Investment in the stock market can be daunting for the novice investor and when people invest based on emotion, it could be the main reason why people are selling when the price are at it's bottom due to the fear or losing more or buying at a higher price as they are hoping to ride the up trend.

In 2020, algorithmic trading account for [60-73%](https://www.mordorintelligence.com/industry-reports/algorithmic-trading-market#:~:text=Algorithmic%20trading%20is%20accounted%20for,overall%20United%20States%20equity%20trading.) of the overall United State Equity Trading. Hence, the main objective on this project is to enable decisions to be made based on different machine learning models that will enable us to bring emotion out of the equation. Additionally, we are trying to build a machine learning model that will be able to generate return higher than inflation and never forget about Rule No. 1

## Executive Summary
There will be 2 notebook for this project

### Data Collection
In this notebook, we will be scrapping stock price of companies from the Standard and Poor's 500(S&P500). S&P500 is made up of the 500 large companies listed on the stock exchanges in the United States. This will provide us information of companies of large market capitalization.

#### Content
- [Stock Price Scrapping](#Stock-Price-Scrapping)
- [Fundamental Data Scrapping](#Fundamental-Data-Scrapping)
- [KMeans Unsupervised Clustering](#KMeans-Unsupervised-Clustering)

### Model
In this notebook, we will be building a variation of LSTM model for forecasting of future prices
#### Content
- [Simple LSTM model](#Simple-LSTM-model)
- [Encoder-Decoder LSTM model Single Output](#Encoder-Decoder-LSTM-model-Single-Output)
- [Sequence to Sequence Prediction](#Sequence-to-Sequence-Prediction)
- [Sequence to Sequence Prediction (With Attention Layer)](#Sequence-to-Sequence-Prediction-(With-Attention-Layer))
- [Sequence to Sequence and Signal Prediction](Sequenceto-Sequence-and-Signal-Prediction)

## Conclusion

From this project, there are a few learning points that we could take away.

Firstly, while doing sequences to sequences prediction, there is bound to be a slight lack in the prediction reaction time of the furthest output prediction as it is based on previous trends and predicted values of the pass few days. Hence, when there is a sudden shock to price, it will take time for the model to react. Hence, when we are using these model, we should be looking for a longer term investment.

Secondly, LSTM is a slow model which would take up a lot of computational capability if feeding in large amount of data and having more complicated layers. For further development, we could consider using embedding of time to vector. This will allow more modern GPU to execute the model much more efficiently. It is hard to tune an LSTM model and despite the memory cell, it will still lose some long term memory. With the use of transformer and attention layer, it will help to retain long term dependence.

Lastly, multiple feature engineering such as Relative Strength Index (RSI), Simple Moving Average (SMA) was initially introduce but was later remove as it does not give our model any better results. However, we could try to introduce more variables to fit the model with more epochs and deeper layer. This might help us to have a better prediction. It is also difficult to tune an LSTM model as the validation loss is fluctuating a lot and EarlyStop are hard to introduce.
