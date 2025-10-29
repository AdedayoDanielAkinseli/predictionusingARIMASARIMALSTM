# predictionusingARIMASARIMALSTM
This repository contains a Jupyter Notebook titled “Predicting UK Average House Prices Using ARIMA, SARIMA, and LSTM Models”, developed as part of a postgraduate dissertation. The project evaluates and compares traditional time series models with deep learning methods for forecasting average UK house prices.
# INTRODUCTION
The main objective of this dissertation was to evaluate the predictive performance of ARIMA (Autoregressive Integrated Moving Average), SARIMA (Seasonal Autoregressive Integrated Moving Average), and LSTM (Long-Short Term Memory) models in forecasting the average house price in the United Kingdom using Government data. Using this univariate dataset, the models were trained on 80% data, and the remaining 20% was tested. Results show the ARIMA model performed poorly by failing to capture the non-linear and seasonal dynamics in the housing market, yielding high errors and a negative R-squared value. SARIMA model improved its accuracy by incorporating seasonality, yielding an R-squared value of 0.8574, though it struggles with long-term dependencies. LSTM outperformed both models, achieving the highest accuracy with R-squared values of 0.8827 and having lower error metrics. LSTM demonstrates its ability to capture non-linear and long-term dependencies. However, LSTM model limitations, which include its reliance on historical data, lack of external economic factors, high computational costs, and restricted interpretability, challenge its forecasting ability. This study highlights the potential of deep learning models like LSTM in offering a reliable framework for forecasting long-term UK housing prices and recommends integrating a multivariate model for future research.
# METHODOLOGY
The dataset was downloaded from the United Kingdom government website, whose main source is the HM Land Registry for England and Wales, Registers of Scotland, and His Majesty’s Revenue and Customs Stamp Duty Land Tax data for the Northern Ireland House Price Index. The Dataset has been assessed against the Quality Assurance of Administrative Data (QAAD) toolkit.
The dataset consists of over 100,000 entries of data ranging over a period of 59years(1965 - 2024). It includes multiple columns, which are : 
Datetime
Region Name, e.g, United Kingdom, England, Scotland, Wales, and Northern Ireland, Belfast, Mid Ulster, Derry City and Strabane, East Midlands, etc.
Area code
Average price 
Price Index
Property Type – detached, semi-detached, terraced, flat, or all property types
Buyer status – first-time buyers  or former owner-occupiers
Funding status – cash and mortgage
Property status – new builds and existing builds

# RESULT AND ANALYSIS FOR ARIMA AND SARIMA MODEL
The table demonstrates how well the ARIMA and SARIMA models predicted UK average house prices. Four evaluation metrics were utilized: The Root Mean Squared Error (RMSE), Mean Squared Error (MSE), Mean Absolute Error (MAE), and R-squared 
Mean Squared Error (MSE): average of squared differences between predicted and actual values
The Root Mean Squared Error (RMSE): the square root of MSE, easily interpretable because it directly compares to the actual values
Mean Absolute Error (MAE): average of absolute differences between predicted and actual values
R-SQUARED: measures how well the model performed

# RESULTS AND ANALYSIS OF LSTM MODEL
The LSTM model with two layers of 64 neurons, a dropout rate of 0.1, and early stopping has an RMSE of 7,470.14, an MSE of 55803119.05, and  R- SQUARED of 0.8827, indicating high prediction performance. The combination of the network size, low dropout, and early stopping is effective in balancing learning capacity with overfitting control, yielding a dependable LSTM model for forecasting UK average house prices.

# CONCLUSION 
The Long Short-Term Memory (LSTM) model accurately captures long-term trends and temporal relationships in historical housing price data. However, it shows limitations when confronted with external shocks such as policy interventions, interest rate increases, or general economic downturns.

