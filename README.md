# Gold-price-prediction
Predicting the first hour of US regular market hours based on pre market data analysis.

First, I will be using Ensemble method using LSTM + XGboost.
In my LSTM model, I will be using an averaged LSTM model using 5min,10min, and 15min timeframes as a sequential input, adding candlestick geometry features, patterns features, and technical indicators features, as well as OHLCV data.
In addition, I am adding a static vector as dense layer where it includes: candlestick geometry features, patterns features, technical indicators features, and support/resistance/breakouts features. I may be adding attention layer later after validation and testing.
In my XGboost model, the results will be definitive in predicting the market regime of the upcoming opening session in US market hours. It will be mainly used for clustering market regimes among "bearish","neutral", and "bullish".
The predictions made by this ensemble model will be then inputted in a meta-model: logistic regression, which will provide the final predictions.

For automation purposes, I can later add a rule-based filter and sentiment analysis and news filter to mitigate risk and implicitly, will be reducing profits.

I am still in the process of building the model. I am gonna share what its ready until now and will be regularly updating. 
