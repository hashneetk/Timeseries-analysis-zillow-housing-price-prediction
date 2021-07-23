# zillow-housing-price-prediction
## Goal:
The goal of this project is to use the California Zillow housing dataset to do the time series analysis of the median sale prices to see if there is any trend/seasonality in the housing sale prices and to find the best model to predict the future sale price. 

## Dataset:
The Zillow dataset (modified) recorded Feb 2008- Dec 2015 monthly median sold price forhousing in California, Feb 2008-Dec 2016 monthly median mortgage rate, and Feb 2008-Dec2016 monthly unemployment rate. This dataset has 3 variables: MedianSoldPrice_AllHomes,MedianMortageRate,UnemploymentRate

## Models tested:
The data has been split into training and validation set for finding the best model that can predict the future median selling price. Different models have been trained using cross validation and the metric used to compare different model is  RMSE - Root mean square error

1. Seasonal Autoregressive Integrated Moving Average( SARIMA)
2. Exponential Smoothing
3. Univariate Prophet
4. Multivariate Prophet
5. Seasonal Autoregressive Integrated Moving Average with external variables( SARIMAX)
6. Long short-term memory(LSTM)
