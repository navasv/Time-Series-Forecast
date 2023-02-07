# Time-Series-Forecast
Time series forecast for the daily minimum temperature in Melbourne, Australia

The objective of this project is to create a time series forecast for the daily minimum temperature in Melbourne, Australia. Time series forecasting is a method used to predict future values based on historical data. In this case, historical data on daily minimum temperatures in Melbourne is used to predict future minimum temperatures.

A time series decomposition method was used to identify any trends, seasonality, and residuals in the data. The data was then split into training and testing sets. The forecasting model used in this project is the SARIMA (Seasonal Autoregressive Integrated Moving Average) model. This model is a combination of the seasonal and non-seasonal components of the data, and it uses both past values and past errors to make predictions. The model was trained on the training data and its performance was evaluated using the testing data.
As the original data was taking indefinite time to build model, data was resampled to monthly data.
The ARIMA model was fit to the data using the auto_arima() function in the pmdarima library in Python. The auto_arima() function automatically selects the best combination of AR, I, and MA parameters for the model based on the data.
The model was then used to make predictions for the daily minimum temperature in Melbourne for the period from January 1, 1989 to December 31, 1990. The predictions were compared to the actual test data to evaluate the accuracy of the model.
