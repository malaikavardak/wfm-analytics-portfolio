# Project 01 – Forecasting Volume

This project simulates hourly support volume over 14 days and builds a simple forecasting model to predict future staffing needs.

## Objective
Use historical hourly volume data to forecast staffing needs for future days — a key component of Workforce Management (WFM).

## Tools
- Python (Pandas, NumPy, Matplotlib)
- Excel (for data sharing and analysis)

## Method
1. Simulated 14 days of hourly volume between 8 AM and 8 PM.
2. Modeled daily traffic pattern using a sinusoidal function + random noise.
3. Averaged volume per hour over the 14 days.
4. Used the average to forecast demand for a future day.
5. Visualized historical data, average trend, and forecast.

## Files
- `demand_forecast.xlsx`: Excel with raw data, hourly averages, and forecast
- `forecasting_model.ipynb`: Python notebook used to generate the simulation and forecast
- `README.md`: This file

## Visualization
The output plot shows:
- Gray: Historical volume for each day
- Blue: Average hourly volume
- Red dashed: Forecasted volume for next day
<img width="1891" height="964" alt="image" src="https://github.com/user-attachments/assets/12348fd9-5402-4a46-b868-ae210b359f0e" />
<img width="1822" height="858" alt="image" src="https://github.com/user-attachments/assets/59c53c47-ebe3-4a32-976a-d24af69791ec" />

---

## WFM Relevance
Forecasting is essential for:
- Accurate staffing
- Cost control
- Meeting SLAs

This project demonstrates a simple yet practical approach to demand prediction in operations and remote support environments.

## Conclusion
The forecasting model leverages Holt-Winters Exponential Smoothing to predict hourly volume for the next day based on historical data. The analysis reveals a strong daily seasonality, with low activity during early morning hours and peak volumes occurring between mid-morning and early afternoon. The model, using additive trend and seasonality with a 24-hour cycle, effectively captures these patterns and provides reliable short-term forecasts. This makes it valuable for operational planning tasks such as staffing, system load management, and demand forecasting. However, its accuracy may be limited in the presence of anomalies or sudden behavioral shifts, suggesting potential for enhancement through the inclusion of external variables.



