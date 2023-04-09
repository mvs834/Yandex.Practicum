# Analysis of telecom company tariffs

[ipynb](https://github.com/mvs834/Yandex.Practicum/blob/3aa4bea6c1e42ac87a4f471651cbefc30ebf6d9f/DA%2004%20Telecom%20tariff%20analysis/Telecom_tariff_analysis.ipynb)

## Project description

The aim of the project is to analyze the behavior of telecom company customers and determine which tariff is more profitable for the company.

## Project workflow
### Data upload

The data has been loaded and does not have any missing values. Since the task requires studying slices by months, dates should be converted to the appropriate format.

### Data preparation
- Column names have been renamed.
- Data types have been changed.
- Dates have been rounded to months.
- Dates have been converted to a consistent format.
- Seconds have been rounded to minutes.
- New columns have been calculated: revenue from calls, SMS and Internet, as well as total revenue including subscription fees.

### Data analysis
- The mean value of the "Ultra" tariff plan in the sample is higher than that of the "Smart" plan.
- The standard deviation of the "Ultra" tariff plan in the sample is higher than that of the "Smart" plan.
- The distributions are similar, but the sample for the "Ultra" plan has a greater positive skewness, although the value of the first quartile is lower than that of the "Smart" plan.

### Hypothesis testing

- Revenue by tariff plans:
Null hypothesis: The average revenue of users on the "Ultra" and "Smart" tariff plans is the same.
Alternative hypothesis: The average revenue of users on the "Ultra" and "Smart" tariff plans is different.

- Revenue by cities:
Null hypothesis: The average revenue of users from Moscow is not different from the revenue of users from other regions.
Alternative hypothesis: The average revenue of users from Moscow is different from the revenue of users from other regions.

## Skills and tools

- **python**
- **pandas**
- **numpy**
- scipy.**stats**



## Summary

The input data for "duration" and "mb_used" have a left-skewed distribution that approximates a Poisson distribution. This is an expected distribution for data reflecting the duration of events.

Data preprocessing included column renaming, data type conversion, rounding dates to months, standardizing date format, and rounding seconds to minutes.

Columns for revenue by service were calculated based on the tariff plans, usage volumes were analyzed, and statistical hypotheses were formulated and tested.

On average, "Smart" tariff plan users spend 419 minutes on calls per month (with a standard deviation of 189), while "Ultra" users spend 548 (with a standard deviation of 305). "Smart" plan users send an average of 39 messages per month (with a standard deviation of 27), while "Ultra" plan users send 61 (with a standard deviation of 46). "Smart" plan users use an average of 16 GB of internet per month (with a standard deviation of 6), while "Ultra" plan users use 20 GB (with a standard deviation of 10). The distribution of services used differs between the two tariff plans, with "Ultra" having a greater left skew, reflecting greater usage volumes by customers of this plan.

The "Smart" tariff plan generates revenue from calls, internet, and messages, while the "Ultra" plan generates revenue primarily from internet usage. "Ultra" plan users do not exceed their limits and mainly generate revenue from their subscription fees.

The average revenue from the two tariff plans differs, with the "Smart" plan generating more revenue than the "Ultra" plan. The average revenue from users in Moscow does not differ significantly from that of users in other regions.