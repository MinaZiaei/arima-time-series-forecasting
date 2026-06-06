# Time Series Forecasting with ARIMA (Stock Data)

## Business Problem

Forecasting stock prices is a challenging problem due to market volatility and randomness. This project uses ARIMA, a traditional time series model, to predict stock prices and evaluate its effectiveness.

---

## Data

- Source: Yahoo Finance
- Stock: AAPL
- Features: Close price time series

---

## Approach

### Stationarity Testing

- Applied Augmented Dickey-Fuller (ADF) test
- Original series was not stationary (p-value ≈ 0.99)
- Applied first-order differencing
- After differencing: p-value ≈ 0 → stationary ✅

---

### ARIMA Model

- Used ARIMA(p,d,q) model
- Selected d = 1 based on stationarity results
- Initial configuration: ARIMA(5,1,0)

---

### Forecasting

- Generated predictions on test dataset
- Compared predicted values with actual prices

---

## Results

- Forecast produced nearly constant predictions
- Model failed to capture volatility of stock prices

---

## Key Insights

- Stock prices behave like a random walk
- ARIMA struggles with highly volatile financial data
- Traditional models capture trends but fail in dynamic environments

---

## Limitations

- ARIMA assumes linear relationships
- Cannot capture non-linear patterns in financial markets

---

## Future Improvements

- Combine ARIMA with machine learning models
- Explore hybrid models (ARIMA + LSTM)
- Add exogenous variables (economic indicators)

---

## Author

Mina Ziaei  
Data Analyst | Aspiring Data Scientist (Finance & AI)
