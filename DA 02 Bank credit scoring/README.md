# Borrowers' Solvency Analysis

[ipynb](https://github.com/mvs834/Yandex.Practicum/blob/3aa4bea6c1e42ac87a4f471651cbefc30ebf6d9f/DA%2002%20Bank%20credit%20scoring/Bank_credit_scoring.ipynb)

## Project Description

It is necessary to assess the impact of the marital status and the presence and number of children of the client on the repayment of the loan on time based on statistics on the solvency of clients.


## Skills and Tools

- **python**
- **pandas**
- **numpy**
- matplotlib.**pyplot**
- **seaborn**
- nltk.stem.**SnowballStemmer**
- pymystem3.**Mystem**

## Project Execution

### Data Upload and Overview
- missing values were detected in two columns (days_employed and total_income)
- it is necessary to change the data type in the days_employed column
- incorrect values were identified, including the presence of negative (days_employed) and ultra-high values, m.b. discharge error (days_employed), different spelling of the same categories, i.e. lowercase and uppercase letters (education)
- implicit duplicates were detected in the purpose column (car deal, car purchase, buying your own car, etc.)

### Data Preprocessing
- missing values in total_income are replaced with median ones in the entire sample
- missing values in days_employed are replaced depending on the age of the client
- incorrect days_employed values have been changed: negative values have been converted to positive, and ultra-high values have been divided by 100
- floating-point values in the days_employed and total_income columns have been replaced with an integer data type
- duplicates in children were replaced based on assumptions about the incorrect introduction of values 20 (zero on the nampad could be located under a deuce) and -1 (minus could be written as a dash)
- in the client_age column, problematic duplicates are only zero values that were deleted based on their insignificant number
- in the education column, duplicates are associated with different spelling of categories, which may be due to a different approach to the initial input of information. All values were given to be written in lowercase letters
- lemmatization of the purpose column was carried out: 1) stems were selected, 2) sorted by frequency of occurrence, 3) the necessary ones were selected for the purposes of the loan and 4) lemmatization was carried out using the function in each row of the column
- to answer the question "is there a relationship between having children and repayment of the loan on time?" The childfree column has been added for borrowers without children (True) and with children (False). Borrowers without children are about 2 times more than borrowers with children

### Answers to Questions
- "Is there a relationship between having children and repayment of the loan on time?" - it is impossible to make an unambiguous conclusion about the dependence between the presence of children and the repayment of the loan on time
- "Does the number of the client's children affect the fact of repayment of the loan on time?" - the largest number of debtors is in the category of borrowers with 4 children, and the smallest is among borrowers without children. This may indicate dependence - the more children the borrower has, the less likely it is to repay the loan on time - children eat up all the money
- "Is there a relationship between marital status and repayment of the loan on time?" - the largest number of debtors in the category "not married", which may be explained by the lack of obligations to the spouse. The smallest number of debtors in the "widower / widow" category, which can be explained by the repayment of debt at the expense of inheritance
- "Is there a relationship between the level of income and repayment of the loan on time?" - there is a relationship between the income level and the repayment of the loan on time - the higher the income, the more loan repayments on time
- "How do the different purposes of the loan affect its repayment on time?" - the largest percentage of debtors is observed in the category of loan purposes "car", the smallest - in the category "housing" (even if you combine the categories "real estate" and "housing")

## Conclusion

The initial data consisted of 21525 rows, after preprocessing they remained 21424. The sample is sufficient to conduct the study.

Data preprocessing consisted of filling in missing values, correcting incorrect values, processing duplicates, categorization and lemmatization.

The following dependencies have been identified:

- with an increase in the number of children from 0 to 4, the number of debtors increases
- with an increase in income, the number of debtors decreases
- the objectives of the loan affect the timely repayment of the loan: the largest number of debtors take a loan for a car, then - for education, for a wedding and the smallest number of debtors take a loan for housing.