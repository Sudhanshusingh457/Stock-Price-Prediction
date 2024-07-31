# Stock-Price-Prediction
Stock Price Prediction

This project is a sophisticated web application designed to predict future stock prices by leveraging historical data and advanced machine learning techniques. At its core, the application utilizes a Long Short-Term Memory (LSTM) neural network, a type of Recurrent Neural Network (RNN) known for its effectiveness in handling time-series data.The application is built to fetch real-time stock data from Yahoo Finance, which serves as the foundation for predictions.
It collects minute-by-minute data for the past day, ensuring that the predictions are based on the most current information available. The data is then processed through a series of preprocessing steps, including normalization and transformation, to prepare it for analysis.
Users can enter a stock symbol of their choice and specify the number of days they wish to predict. The application then processes the request, performs the necessary computations, and displays the predicted stock price.

# Features:

Real-Time Data Retrieval: Fetches the latest stock price data using the Yahoo Finance API.
Data Preprocessing: Normalizes stock price data to prepare it for the LSTM model.
LSTM Model: Utilizes a Long Short-Term Memory neural network to predict future stock prices based on historical data.
Streamlit Interface: Provides an interactive web interface where users can input stock symbols and specify the number of days for prediction.


# Prerequisites:

Ensure you have the following Python packages installed:
>streamlit

>numpy

>pandas

>yfinance

>scikit-learn

>tensorflow

You can install the required packages using pip:
pip install streamlit numpy pandas yfinance scikit-learn tensorflow

How to Use:

1.Clone the Repository:
git clone <repository-url>
cd <repository-directory>

2.Run the Streamlit App:
Copy code
streamlit run <script-name>.py
Replace <script-name>.py with the name of your Python file.

3.Interact with the Web App:
i.Enter the stock symbol (e.g., AAPL for Apple) in the input field.
ii.Use the slider to select the number of days for which you want to predict the stock price.
iii.Click the "Predict" button to see the forecasted stock price.

# Code Overview:

i.predict_price(ticker, days): The main function that performs stock price prediction. It includes sub-functions for data retrieval, preprocessing, model creation, and prediction.

ii.get_realtime_data(ticker, interval='1m', range='1d'): Fetches real-time stock data from Yahoo Finance.
iii.preprocess_data(data): Normalizes the stock price data.

iv.create_dataset(dataset, look_back=1, days=1): Creates datasets for training the LSTM model.
v.create_model(): Defines and compiles the LSTM neural network.

vi.predict_prices(model, data, scaler): Uses the trained model to predict future stock prices.

# Contributing:

Contributions are welcome! Please submit a pull request with your proposed changes or improvements.
