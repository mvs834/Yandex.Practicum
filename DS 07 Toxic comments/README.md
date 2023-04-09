# Toxic Comments Identification

[ipynb](https://github.com/mvs834/Yandex.Practicum/blob/3aa4bea6c1e42ac87a4f471651cbefc30ebf6d9f/DS%2007%20Toxic%20comments/Toxic_Comments_Predictions.ipynb)

## Project Description

The project involves identifying toxic comments based on a dataset with labeled toxicity.

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
- The data is provided in the form of textual comments.
- There are no missing or duplicate values.
- The target variable is imbalanced.

### Text Cleaning and Lemmatization
- Cleaning the text by removing punctuation marks, digits, symbols, and others except letters and converting to lowercase.
- Lemmatization of the text using two methods: NLTK (faster) and Spacy (slower).

### Model Training
- Text vectorization using the TF-IDF method.
- Training models using logistic regression, decision tree, random forest, gradient boosting, and CatBoost.
- The logistic regression model showed the best performance.

### Lemmatization Evaluation
- Lemmatization using Spacy showed better results.

### Testing
- The logistic regression model showed the best performance with Spacy-lemmatized data.

## Conclusion

The text was loaded and did not require preprocessing. Data preparation involved cleaning the text by removing punctuation marks, digits, symbols, and others except letters and converting to lowercase. Lemmatization was performed using two methods: NLTK (faster) and Spacy (slower). Text data was vectorized using the TF-IDF method for training logistic regression and decision tree models. The logistic regression model showed the best performance, and Spacy-lemmatized data achieved better results. To improve the metric further, tokenization, gradient boosting, and neural network-based vectorization with BERT can be implemented as next steps.
