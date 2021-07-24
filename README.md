# zillow-housing-price-prediction
## Goal:
The Zillow dataset recorded Feb 2008 - Dec 2015 monthly median sold price for housing in California, Feb 2018 - Dec 2016 monthly median mortgage rate and Feb 2008 - Dec 2016 monthly unemployment rate. The goal of this project is to predict the monthly median sold price for Jan-Dec 2016. 
There are three features in the dataset are:Date, MedianSoldPrice, MedianMortageRate, UnemploymentRate.

## Models tested:
The data has been split into training and validation set and the metric used to compare the performance of different models is  RMSE - Root mean square error
### Univariate Models: 
1. Seasonal Autoregressive Integrated Moving Average( SARIMA)
2. Exponential Smoothing
3. Univariate Prophet

### Multivariate Models:
1. Multivariate Prophet
2. Seasonal Autoregressive Integrated Moving Average with external variables( SARIMAX)
3. Long short-term memory(LSTM)

### Approach followed to find the best model:
For each category of models we tried 2,3 different parameters with a train and validation set which gave us 2-3 different models for each algorithm. From these we selected the ones with lowest RMSE. This gave us different candidate models. So we had 6 different candidate models, one from each algorithm. From these we then selected the one with the lowest RMSE as our final model. We then used this final model to check for the RMSE on the test set.

#### For the details of the preprocessing done and in-depth analysis of each of these model, please refer to the final report in the repo.
