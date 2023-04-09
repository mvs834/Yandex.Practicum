# Сhoosing the most profitable region for drilling wells

[ipynb](https://github.com/mvs834/Yandex.Practicum/blob/3aa4bea6c1e42ac87a4f471651cbefc30ebf6d9f/DS%2003%20Oil%20region%20profit%20estimation/Oil_region_profit_estimation.ipynb)

## Project Description

The objective of this project is to determine the most profitable and least risky region for drilling a new well based on data about the quality of oil and the volume of reserves.

## Project Execution Steps
### Data Upload and Preparation

Since there are no missing values, duplicates or problematic values in the data, no preprocessing is required.

### Model Training and Validation

- A high correlation was found between feature f2 and the target feature for region 1.
- A function was written to split the data into training and validation sets, and to train a linear regression model.
- A function was written for a dummy model.
- Comparison of the results of the linear regression model with the dummy model showed that the models are adequately trained as they show a lower RMSE error.

### Profit and Risk Calculation

- A function was written to calculate the profit.
- A function was written to evaluate the prospects using Bootstrap.

## Skills and Tools

- **python**
- **pandas**
- **numpy**
- Bootstrap
- matplotlib.**pyplot**
- **seaborn**
- sklearn.linear_model.**LinearRegression**



## Conclusion

As a suggestion, attention should be given to Region 1 due to its relatively high average predicted profit and low probability of incurring losses. However, it is important to note that feature f2 is highly correlated with the target variable in this region. There may be an error and the evaluation may be incorrect.

Regions 0 and 2 have similar indicators, and the choice between them should be based on risk tolerance: Region 2 has a higher probability of losses but also a slightly higher predicted profit, while Region 0 is more conservative in this regard.