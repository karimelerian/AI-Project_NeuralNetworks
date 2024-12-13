# Stock Price Prediction using LSTM

This project leverages an LSTM (Long Short-Term Memory) neural network to predict stock prices based on historical market data.

## Dataset

The project uses the "Stock Exchange Data" dataset from Kaggle, including daily stock data:

- **Columns**: Date, Open, High, Low, Close, Adj Close, Volume.
- **Key file**: `indexData.csv`.

## Methodology

### Preprocessing
- Handle missing values.
- Normalize features with `MinMaxScaler`.
- Split data into training and testing sets.

### LSTM Model
- Single LSTM layer, dropout, and dense output layer.
- Trained with the Adam optimizer and Mean Squared Error loss.
- Early stopping to prevent overfitting.

### Evaluation
- **Metrics**: RMSE, MAE, R-squared, and Directional Accuracy.
- Visualization of actual vs. predicted prices.

## Features and Techniques

- Sliding window approach (60 days) for feature creation.
- Focus on 'Close' and 'Volume' data.
- Correlation analysis and data distribution exploration.
