# zillow-housing-price-prediction
## Goal:
The goal of this project is to use the California Zillow housing dataset to do the time series analysis of the median sale prices to see if there is any trend/seasonality in the housing sale prices and to find the best model to predict the future sale price. 

## Dataset:
The Zillow dataset (modified) recorded Feb 2008- Dec 2015 monthly median sold price for housing in California, Feb 2008-Dec 2016 monthly median mortgage rate, and Feb 2008-Dec2016 monthly unemployment rate. This dataset has 3 variables: MedianSoldPrice_AllHomes, MedianMortageRate, UnemploymentRate

## Models tested:
The data has been split into training and validation set and the metric used to compare the performance of different models is  RMSE - Root mean square error

1. Seasonal Autoregressive Integrated Moving Average( SARIMA)
2. Exponential Smoothing
3. Univariate Prophet
4. Multivariate Prophet
5. Seasonal Autoregressive Integrated Moving Average with external variables( SARIMAX)
6. Long short-term memory(LSTM)

### Approach followed to find the best model:
For each category of models we tried 2,3 different parameters with a train and validation set which gave us 2-3 different models for each algorithm. From these we selected the ones with lowest RMSE. This gave us different candidate models. So we had 6 different candidate models, one from each algorithm. From these we then selected the one with the lowest RMSE as our final model. We then used this final model to check for the RMSE on the test set.

#### For the details of the preprocessing done and in-depth analysis of each of these model, please refer to the final report in the repo.
