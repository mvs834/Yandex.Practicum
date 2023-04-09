# Car Market Price Prediction

[ipynb](https://github.com/mvs834/Yandex.Practicum/blob/0ba08c55408e5f1b47e1ec04d56d6d981c85a8a8/DS%2005%20Car%20Price%20Prediction/Car_Price_Prediction.ipynb)

## Project Description

The goal of this project is to estimate the market value of a car based on historical data, including technical specifications, equipment, and prices of similar cars.

## Skills and Tools

- **python**
- **pandas**
- **numpy**
- matplotlib.**pyplot**
- **seaborn**
- sklearn.preprocessing.**StandardScaler**
- sklearn.preprocessing.**OrdinalEncoder**
- sklearn.**pipeline**
- sklearn.linear_model.**LinearRegression**
- sklearn.tree.**DecisionTreeRegressor**
- sklearn.ensemble.**RandomForestRegressor**
- **lightgbm**
- **xgboost**
- catboost.**CatBoostRegressor**

## Project Execution
### Data Upload and Overview
- Column names are not in the "snake_case" format.
- Columns with dates are not in date format.
- Missing data on timestamps.
- 5 columns contain missing values.
- 4 rows are clear duplicates.
- Strange values in columns with price, registration year, number of images, postal code, mileage, and power.

### Data Preprocessing
- Zero values in the target variable have been removed.
- Prices have been rounded to the nearest 50 euros.
- Incorrect values and outliers in columns with registration year and power have been removed.
- Mileage column has been categorized.
- Missing values in columns with gearbox type, body type, engine type, and model have been removed.
- Column names have been converted to "snake_case".
- Columns with dates have been converted to date format.
- Missing values in the timestamp column have been filled.

### Model Training
- New features have been created.
- Categorical features have been encoded.
- Linear regression, decision tree, random forest, gradient boosting, and catboost models have been trained.
- Model training times have been recorded.

### Model Analysis
- The CatBoost model with the lowest RMSE values and optimal training time was selected.

## Conclusion

Data preprocessing was performed (format changes, handling missing values and outliers), exploratory data analysis was conducted to identify outliers, new features were created, and a model was trained and selected for price prediction. The CatBoost model was selected, which showed the lowest RMSE value of 29.1 in a reasonably short amount of time.