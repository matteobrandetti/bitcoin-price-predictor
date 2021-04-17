# bitcoin-price-predictor
Neural Network models to forecast bitcoin price with distinct granularities (Timeserie forecasting)
This repository includes four different Jupyter Notebooks with distinct DL-based models for the prediction of the closing price of Bitcoin.
- ***1 Minute Single Step Networks***: it trains two different NN models, LSTM and Convolutional 1D-based, respectevely. Both take a 20 minutes window of samples (Open Price, Closing Price, ecc.) and predicts the Bitcoin closing price of the following minute.
- ***1 hour Single Step Networks***: it trains an LSTM based model, which takes in input a 24 hours window of samples (Open Price, Closing Price, ecc.) and predicts the Bitcoin closing price of the next hour.
- ***10 Mins Multiple Step Networks***: it trains two different NN models, LSTM and Convolutional 1D-based, respectevely. Both take a window of 30 samples (Open Price, Closing Price, ecc.) that occur every 10 mins and and predicts the Bitcoin closing price of the next 100 mins as 10 distinct outputs (a prediction every 10 mins). 
- ***60 Mins Multiple Step Networks***: it trains three different NN models, LSTM, Convolutional 1D-based, and a Multihead Convolutional Network. They all take as input a window of 6 samples occurring every 10 mins (1h) and forecast the price for the next hour as 6 distict predictions of the closing price every 10 mins.
