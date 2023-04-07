# Bank customer churn prediction

[ipynb](https://github.com/mvs834/Yandex.Practicum/blob/a58d05259920dddcd70aaf0b1e6c6a3526397949/DS%2002%20Bank%20customers%20churn/Bank_customer_churn.ipynb)

## Project Description

The task is to predict whether a customer will leave the bank based on historical data on customer behavior and termination of contracts with the bank.

## Project Execution
### Data Upload and Preprocessing

- Column names are converted to "snake_case".
- Missing values in the Tenure column are processed.
- The target variable is unbalanced.

### Exploratory Data Analysis on Unbalanced Data
#### Logistic Regression

- Categorical features are converted to numerical using One Hot Encoder.
- Features are independent of each other.
- Quantitative features are scaled.
- Samples are split and the model is trained.

#### Decision Tree, Classification

- Categorical features are converted to numerical using OrdinalEncoder.
- Samples are split and the model is trained.

#### Random Forest, Classification

- Samples are split and the model is trained.

Conclusion: The highest F1 score was achieved when training the Random Forest model compared to Logistic Regression and Decision Tree. Therefore, Random Forest should be used for further analysis.

### Dealing with Imbalanced Data

- Increasing the sample size leads to an increase in the F1 score. Therefore, an increased sample should be used for further analysis.
- The maximum accuracy, recall, and F1 score are achieved at a threshold of 0.4.
- The AUC-ROC metric is high, and the graph is steep enough.

### Model Test
- f1_score: 0.59
- AUC ROC score: 0.8566493552869575

## Skills and Tools

- **python**
- **pandas**
- **numpy**
- matplotlib.**pyplot**
- **seaborn**
- sklearn.linear_model.**LogisticRegression**
- sklearn.tree.**DecisionTreeClassifier**
- sklearn.ensemble.**RandomForestClassifier**



## Conclusion

The input data was processed by retaining only the necessary parameters and eliminating missing values. The analysis of the imbalanced dataset revealed that the Random Forest model performed the best. The best hyperparameters for the Random Forest model were selected using a grid search method. Balancing the initially small sample of the target variable using the upsampling method is preferred because of the high F1 score it yields. Consequently, a model was developed to predict customer churn based on historical data, achieving an F1 score of 0.6.