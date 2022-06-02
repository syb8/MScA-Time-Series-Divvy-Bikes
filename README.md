# Divvy Bikes Stock Rebalancing Issues

Use Case:
- Predicting potential station/dock availability using bike-in and bike-out data as proxies

Dataset:
- Divvy Bikes Travel History
- Bike-in and Bike-out
- Weather History

Goals:
- Realtime Hourly Forecast
- Aggregated Daily Forecast

Key Challenges:
- Lumpy/Erratic Data
- Complex seasonality (more than two seasonalities)
- High Variance

Models:
Univariate Forecasting
1. TBATS
2. Double-Seasonal Holt-Winters
3. Auto Arima with Fourier Terms
4. Prophet

Intervention Examination (Covid-19 Effect):
1. Dynamic Regression (incorporating weather to see Covid impact)
2. Causal impact, intervention model

Result:
1. TBATS using two seasonalities (yearly, weekly)
2. Covid-19 impact can be seen by incorporating weather data as weather provides contrast to traffic data (weather not affected by Covid while Divvy traffic was. Covid-19 also impacts various regions differently).
