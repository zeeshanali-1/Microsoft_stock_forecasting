Microsoft Stock Forecasting with LSTM

Stock forecasting is a challenging task that involves forecasting future stock prices based on historical data. As, the future trends depend upon the past data, one effective approach that we are going to use is Long Short-Term Memory (LSTM) neural networks, a type of recurrent neural network (RNN) well-suited for time series data. LSTM models can capture long-term dependencies in stock prices, making them useful for predicting future trends.
Here, we first try to predict the stocks of Microsoft, and we used their historical data. We used the data starting from 1st January 2000 till the current date which is 1st August 2024. 

The process typically involves these steps:

1.	Data Acquisition:
	
o	The dataset is downloaded from Yahoo Finance, focusing on Microsoft's stock prices.

o	The data is cleaned and prepared, keeping only relevant columns such as the date and closing prices.

2.	Data Preprocessing:

o	The date column is converted from a string to a datetime object for easier manipulation.

o	The closing prices are prepared in a format that the LSTM model can use for training.

o	A windowing function is created to structure the data into sequences that the LSTM can learn from.

3.	Model Setup:

o	TensorFlow and Keras are used to create a sequential model.

o	The model consists of an input layer, an LSTM layer with 64 neurons, and dense layers.

o	The model is trained on the preprocessed data.

4.	Training and Testing:

o	The data is split into training, validation, and testing sets.

o	The model is trained using the training set, validated during training using the validation set, and finally tested on unseen data to evaluate its performance.

5.	Model Evaluation:

o	The model's performance is evaluated based on its ability to predict the stock price using the testing dataset.

o	Visualizations using Matplotlib help in understanding the model's predictions compared to the actual stock prices.

In the end we concluded that predicting stocks is incredibly difficult. There is of course the trend we can analyze. We saw that the graph really started to go up and that would indicate that it's a good stock to buy, but that doesn't guarantee that.

