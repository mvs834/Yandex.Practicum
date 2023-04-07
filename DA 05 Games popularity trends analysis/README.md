# Analysis of trends in the popularity of games

[ipynb](https://github.com/mvs834/Yandex.Practicum/blob/1a914a49824195561f514b79a769795e01448633/DA%2005%20Games%20popularity%20trends%20analysis/Games_popularity_trends_analysis.ipynb)

## Project Description

It is necessary to identify patterns that determine the success of the game based on historical data about the games. This will allow you to bet on a potentially popular product and plan advertising campaigns

## Project progress
### Data loading

Data is loaded, needs preprocessing

### Data preprocessing
- column names are reduced to lowercase
- - partial replacement of omissions was made: the rating omissions were partially restored by the names of the games, and the ratings of users and critics have a significant number of omissions, it is better not to fill them in so as not to draw incorrect conclusions when analyzing.

### Exploratory data analysis
- studied data slices: games by year, sales by platform, sales from reviews, games by genre
- a portrait of a user from each region has been compiled: the most popular platforms, genres, the impact of the ESBR rating on sales in the regions

### Hypothesis Testing
- Null hypothesis: the average user ratings of Xbox One and PC platforms are the same.
- Alternative hypothesis: the average user ratings of Xbox One and PC platforms are different.

The statistical hypothesis of the equality of average user ratings of the two platforms is not rejected. Users rate games, not platforms, and in most cases, these ratings are similar. However, as discovered when filling in missing data, some platforms have significantly different ratings, which may be due to technical features of transferring games from one platform to another.

- Null hypothesis: the average user ratings of Action and Sports genres are the same.
- Alternative hypothesis: the average user ratings of Action and Sports genres are different.

The statistical hypothesis of the equality of average user ratings of the two genres is rejected. This is consistent with the results - the study showed that the user profile (genre preferences) differs around the world.


## Skills and tools

- **python**
- **pandas**
- **numpy**
- matplotlib.**pyplot**
- **seaborn**



## Conclusion

To identify the patterns that determine the success of a game, the period from 2014 to 2016 was selected. It is not recommended to take a longer period because the market situation changes. Over time, there is more competition among platforms, and the speed of changing gaming trends has increased. Before 2007, leaders among gaming platforms changed every 5 years, and after that, they changed every 2-3 years. Since the forecast is for 2017, the interval should not exceed 3 years behind the forecast, which means the period of 2014-2016.

Currently, the most popular platforms are PS4 and XOne, but their popularity started to decline in 2015. This means that a new gaming platform will soon appear on the market, and investing in it could pay off in the following years.

User and critic reviews do not influence sales.

The most profitable gaming genres are action and shooter. However, to maximize profits in the shooter genre, a small number of high-quality games should be developed, while in the action genre, a large number of games should be produced.

When choosing the PS4 platform, the market to focus on is not important, while for XOne games, the European or North American markets are preferred. The market is also not crucial when choosing the action genre, whereas the shooter genre may be less in demand in Japan. Ratings affect sales differently in the Western and Eastern worlds. In Europe and North America, games with an M rating have high sales, while in Japan, games with a T rating sell more.