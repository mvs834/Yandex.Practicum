# Gold Recovery Prediction

[ipynb](https://github.com/mvs834/Yandex.Practicum/blob/933ecc24c96cc99ef951753285712c67b565ad0c/DS%2003%20Oil%20region%20profit%20estimation/Oil_region_profit_estimation.ipynb)

## Project Description

The goal of this project is to predict the gold recovery rate from gold-containing ore based on mining and refining parameters.

## Project Execution
### Data Upload and Preparation
- The test dataset is missing 34 features that are present in the training dataset.
- The efficiency of enrichment calculations was verified, and the calculation was found to be correct.
- The test dataset is missing the target features, final.output.recovery and rougher.output.recovery.

### Data Preprocessing
- Missing values were filled with the previous values.
- Target features were added to the test dataset.

### Data Analysis
- Distribution plots of the features at different refining stages were constructed.
- The sizes of the raw material granules in the training and test datasets are the same.
- The total concentration of metals (Au, Ag, Pb) increases after enrichment and is concentrated (distribution narrows) at the end of the technological process.

### Model Building
- Functions were written to calculate the final sMAPE.
- Linear regression, decision tree, and random forest models were trained.

## Skills and Tools

- **python**
- **pandas**
- **numpy**
- matplotlib.**pyplot**
- **seaborn**
- sklearn.linear_model.**LinearRegression**
- sklearn.tree.**DecisionTreeRegressor**
- sklearn.ensemble.**RandomForestRegressor**



## Conclusion

The best model is the random forest model, which was found to be adequate as it has a lower sMAPE error compared to the constant dummy model.