# RabTech Task 5: Time-Series Forecasting with ARIMA

## Dataset
This project uses the supplied `daily-demand-series.csv` with columns:
- `date`: daily observation date
- `demand`: demand value to forecast
- `marketing_event`: indicator for a marketing event
- `holiday`: holiday indicator

The provided dataset has only 30 daily observations. Treat forecasts as a demonstration, not a reliable operational forecast.

## Run in VS Code
1. Open this folder in VS Code.
2. Create and activate a virtual environment.
3. Install packages with `python -m pip install -r requirements.txt`.
4. Open `notebooks/task5_time_series_forecasting.ipynb`.
5. Select the `.venv` kernel and choose **Run All**.
6. Save the notebook with Ctrl+S.

## Methods
- Time-series decomposition (weekly period)
- Augmented Dickey-Fuller stationarity test
- Differencing when indicated by ADF
- Small ARIMA grid search using a chronological holdout
- MAPE and RMSE evaluation
- 30-day forecast with a forecast plot

## Limitations
Only 30 observations are available. Weekly decomposition and a short holdout can be unstable with such limited data. Forecasts beyond the observed range are highly uncertain. Do not treat them as a dependable business plan.
