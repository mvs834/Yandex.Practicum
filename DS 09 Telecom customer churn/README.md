# Customer Churn Prediction for a Telecommunications Company

[ipynb](https://github.com/mvs834/Yandex.Practicum/blob/bff7a30c0b9fb9cd09551ec9d79578344f975552/DS%2009%20Telecom%20customer%20churn/Telecom_Customer_Churn_LGBM_0,89.ipynb)

## Project Description

The goal of this project is to analyze customer data, including their connected services and expenses, and predict potential customer churn.

## Project Execution
### Data Upload and Preprocessing
- Column names are converted to lowercase.
- No missing values were found.
- Data types were converted to their appropriate types.
- Feature distributions were analyzed.
- New features were created.

### Feature Selection
- Feature correlations were analyzed.

### Exploratory Data Analysis
- Churned customers had higher monthly service expenses and did not have additional services.

### Data Preparation for Training
- Data was split into training and testing sets.
- Categorical features were encoded.
- Quantitative features were scaled.
- Significant features were selected based on logistic regression and random forest models.

### Model Training
- Logistic regression, decision tree, random forest, and gradient boosting models were trained with consideration for class imbalance using LGBM, XGBoost, and CatBoost classifiers.
- The LGBM model with the best performance was selected.

### Model Evaluation on Test Set
- The LGBM model achieved an ROC-AUC score of 0.89 on the test set.


## Skills and Tools

- **python**
- **pandas**
- **numpy**
- matplotlib.**pyplot**
- **seaborn**
- sklearn.feature_selection.**SequentialFeatureSelector**
- sklearn.inspection.**permutation_importance**
- sklearn.linear_model.**LogisticRegression**
- sklearn.tree.**DecisionTreeClassifier**
- sklearn.ensemble.**RandomForestClassifier**
- **lightgbm**
- **xgboost**
- catboost.**CatBoostClassifier**



## Conclusion

This project involved data preprocessing, exploratory analysis to identify significant features, creation of new features, and training and selection of a model for customer churn prediction. The LGBM model was selected with an ROC-AUC score of 0.89.