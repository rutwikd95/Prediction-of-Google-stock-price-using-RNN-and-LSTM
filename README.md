# Prediction-of-Google-stock-price-using-RNN-and-LSTM
This is a Recurrent Neural Network (RNN) that predicts the Google stock prices and the trend in stock prices using the LSTM units (using Keras).

### About LSTMS:

The Long Short-Term Memory (LSTM) cell can process data sequentially and keep its hidden state through time.
Long short-term memory (LSTM) units are units of a recurrent neural network (RNN). An RNN composed of LSTM units is often called an LSTM network. A common LSTM unit is composed of a cell, an input gate, an output gate and a forget gate. The cell remembers values over arbitrary time intervals and the three gates regulate the flow of information into and out of the cell.

LSTM networks are well-suited to classifying, processing and making predictions based on time series data, since there can be lags of unknown duration between important events in a time series. LSTMs were developed to deal with the exploding and vanishing gradient problems that can be encountered when training traditional RNNs. Relative insensitivity to gap length is an advantage of LSTM over RNNs, hidden Markov models and other sequence learning methods in numerous applications

![lstm 2](https://user-images.githubusercontent.com/33639642/45781401-d9e4c980-bc2d-11e8-85a5-bc6bdac9692b.png)


### How it works?  
The RNN takes in the training data (Google_Stock_Price_Train.csv) as input and trains on the previous 120 rows to predict the next value.
For this project, I have used 6 LSTM layers along with Dropout Regularization on each layer.
The RNN is compiled using the "Adam" Optimizer along with the "Mean_Squared_Error" as the Loss Function.

After the RNN is trained, the predicted values are compared with the Real Stock Price Values (Google_Stock_Price_Test.csv).
From Visualization (Plot), we can see that the predicted values follow the same upward and downward trend as the Real Stock values.
