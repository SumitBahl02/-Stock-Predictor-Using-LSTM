# Stock Price Prediction Using LSTM

This project predicts stock prices using a Long Short-Term Memory (LSTM) neural network. The dataset used is for TATA Global stock prices.

## Project Overview

The goal of this project is to predict future stock prices based on historical data. The model is trained on historical stock prices and then used to predict future prices.

## Key Steps

1. **Data Preprocessing:**
   - Load the dataset.
   - Scale the features using `MinMaxScaler`.
   - Create sequences of 60 time steps for training.

2. **Model Building:**
   - Construct an LSTM model with four LSTM layers and dropout regularization.
   - Compile the model with the 'adam' optimizer and 'mean_squared_error' loss function.
   - Train the model on the training data.

3. **Prediction:**
   - Load the test dataset.
   - Prepare the input data for prediction.
   - Use the trained model to predict stock prices.
   - Plot the real vs. predicted stock prices.

## Files

- `NSE-TATAGLOBAL.csv`: Contains historical stock prices for training.
- `tatatest.csv`: Contains stock prices for testing the model.
- `stock_prediction.py`: The main script for preprocessing, training the model, and predicting stock prices.

## Dependencies

- NumPy
- Matplotlib
- Pandas
- Scikit-learn
- Keras

## How to Run

1. Clone this repository.
2. Ensure you have all the dependencies installed.
3. Run the `stock_prediction.py` script.

```bash
python stock_prediction.py
