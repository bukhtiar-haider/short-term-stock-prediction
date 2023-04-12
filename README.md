# Short-Term Stock Prediction with LSTM

This repository contains code for a machine learning-based stock prediction model using stacked time-series encoder-decoder LSTM architecture. The model is trained on the historical stock data of Apple (AAPL) acquired from Yahoo Finance. The purpose of this model is to predict short-term trends in the stock market for moderate frequency trading.

## Requirements

The following packages are required to run the code:
- tensorflow
- pandas
- numpy
- matplotlib
- scikit-learn

## Usage

1. Clone the repository:

git clone https://github.com/username/repo-name.git

2. Download the dataset from Yahoo Finance and save it as `AAPL.csv`.

3. Open the Jupyter notebook `AAPL-Stock-Prediction-LSTM.ipynb`.

4. Run the cells in the notebook to train and test the model.

## Results

The trained model is capable of predicting short-term trends in the stock market for Apple (AAPL) with moderate accuracy. The model architecture consists of two LSTM layers, each with 128 units, followed by a Dense layer. The output layer is a Dense layer with one neuron, which predicts the next day's Close value. The model uses mean squared error as the loss function, and the `mse_penalize_greater` function is used to compute the loss by penalizing overestimation more than underestimation. The model is trained for 1000 epochs with a batch size of 32.

## License

This code is released under the MIT License. See `LICENSE` for more information.
