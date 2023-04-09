# Detecting Factors Affecting Real Estate Prices

[ipynb](https://github.com/mvs834/Yandex.Practicum/blob/3aa4bea6c1e42ac87a4f471651cbefc30ebf6d9f/DA%2003%20Real%20estate%20price%20analysis/Real_estate_price_analysis.ipynb)

## Project Description
The objective is to identify the parameters that affect the market value of real estate based on advertisement data and mapping. This will enable the creation of an automated system that can detect anomalies and fraudulent activities.

## Skills and Tools

- **python**
- **pandas**
- **numpy**
- matplotlib.**pyplot**
- **seaborn**

## Project Execution
### Data Upload and Overview
Necessary actions have been identified:

- Renaming columns
- Changing data types
- Handling missing values and incorrect data

It is possible that the price will be primarily determined by the living space.

### Data Preprocessing
Missing values have been handled:

- The balcony column: missing values have been filled with the absence of balconies, which did not affect the distribution. The number of balconies has a significant effect on the price of housing with 0-2 balconies and increases the price with 3 or more balconies. Thus, three groups are distinguished - without balconies, with 1-2 balconies, and with 3 or more balconies.
- The ceiling_height column: incorrect values have been removed, and missing values have been filled based on the initial distribution, without disrupting it.
- The days_exposition column: missing values have been filled without changing the original distribution.


Data type has been changed:

- Last_price - to int, as the accuracy of price in kopeks does not matter; it is also more convenient to convert values to millions.
- Days_exposition - to int - half-day accuracy is not important.
- First_day_exposition - in time format, as it is difficult to work with this data otherwise.


### New Features Creation

- Price per square meter
- Advertisement publication date
- Sale date
- Categorization of apartment floors
- Ratio of total area to living area

### Exploratory Data Analysis

- Filtered out rows likely covering predominantly small settlements.
- The price is directly dependent on the area of the property.
- Price does not depend on the distance from the center, but there is an area with high housing prices within 0-8 km from the center.
- The price depends on the floor category.
- Price does not depend on the day of publication, but maximum prices are on Thursdays and Sundays.
- Price weakly depends on the month - it is minimum in October and maximum at the beginning of the year and in the middle of summer.
- The price depends on the year - it fell from 2014 to 2017 and then began to rise.
- Maximum cost is in Saint Petersburg, minimum - either in Vyborg or Krasnoye Selo (depending on the filter).
- All basic parameters of housing (total area, price, ceiling height, number of rooms) are higher on average in the city center than in the surrounding areas and suburbs.
- In the center of Saint Petersburg, the price is influenced by fewer factors because the key factor is the fact that the property is located in the center. In the surrounding areas, only the total area of the property has an impact on the price. On the suburbs, the number of rooms also begins to affect the price of housing. The ceiling height has no significant impact on the price of housing regardless of its location.

## Conclusion
The following parameters that affect the market value of real estate have been established:

- Number of photos: a small quantity may be a sign of fraud.
- Total area and derivatives (living space, kitchen area, number of rooms) are the main parameters that determine the price of housing.
- In large cities, the distance from the center is important because there is a clear division into zones that determine the basic parameters of housing.
- Floor: housing on the first floor is generally cheaper for many reasons, while housing on the top floor is usually more expensive.
- Publication time generally does not determine the price, but there are months and days of the week when prices differ.
- Prices can change from year to year, and in large cities, they may have different directions of change depending on the zone.