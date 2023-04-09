# Time Series. Forecasting the number of taxi clients.

[ipynb](https://github.com/mvs834/Yandex.Practicum/blob/3aa4bea6c1e42ac87a4f471651cbefc30ebf6d9f/DS%2006%20Taxi%20clients%20prediction/Time_Series_Taxi_Clients_Prediction_RMSE_6.9.ipynb)

## Project Description
The goal of this project is to analyze historical data on taxi orders at airports and forecast the number of taxi orders for the next hour based on this data.

## Skills and Tools

- **python**
- **pandas**
- **numpy**
- matplotlib.**pyplot**
- **seaborn**
- statsmodels.tsa.seasonal.**seasonal_decompose**
- sklearn.model_selection.**TimeSeriesSplit**
- sklearn.pipeline.**make_pipeline**
- sklearn.linear_model.**LinearRegression**
- sklearn.tree.**DecisionTreeRegressor**
- sklearn.ensemble.**RandomForestRegressor**
- **lightgbm**
- **xgboost**
- catboost.**CatBoostRegressor**

## Project Execution
### Data Upload and Overview
- The data is represented as a time series with hourly intervals
- The data contains outliers
- The data is monotonous

### Data Analysis
- The data exhibits a trend and daily seasonality

### Model Training
- A feature for the day of the week was created to train the models
- Models were trained using linear regression, decision tree, random forest, gradient boosting, and CatBoost
- The best result was achieved with the random forest model

### Model Testing
- On the test dataset, the random forest model achieved an RMSE score of 6.9

## Conclusion

In this project, the data was preprocessed (outliers removal, checking for missing values and duplicates, checking for monotonicity, rescaling), an exploratory data analysis was performed to identify seasonality, and a model was trained and selected to forecast the number of taxi clients for the next hour. The best model was the decision tree model with max_depth=4. At this hyperparameter value, the RMSE score on the test dataset is 6.9.