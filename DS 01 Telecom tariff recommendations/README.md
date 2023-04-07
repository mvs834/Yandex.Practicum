# Recommendation of a telecom tariff to a customer

[ipynb](https://github.com/mvs834/Yandex.Practicum/blob/ef7d24f2858f502ecbf13930df9cc0918c0ec7f0/DS%2001%20Telecom%20tariff%20recommendations/Telecom_tariff_recommendations.ipynb)


## Project Description

The goal of this project is to build a classification model that recommends the most suitable telecom tariff for a customer based on their usage of minutes, SMS, and internet traffic.

## Project Execution Workflow
### Data upload

The data does not require any preprocessing.

### Data Splitting
The training set contains 1,928 rows, and the validation set contains 643 rows.

### Model Analysis
The highest accuracy was achieved by the Random Forest model, which had an accuracy of 0.786 on the validation set. The best Decision Tree model had a maximum depth of 5 and achieved an accuracy of 0.784 on the validation set. The Logistic Regression model had an accuracy of 0.684 on the validation set.

## Skills and Tools

- **python**
- **pandas**
- **seaborn**
- sklearn.linear_model.**LogisticRegression**
- sklearn.tree.**DecisionTreeClassifier**
- sklearn.ensemble.**RandomForestClassifier**



## Conclusion

Comparing the built model to a constant model reveals a small difference of only 8%. This indicates that the model requires improvement.