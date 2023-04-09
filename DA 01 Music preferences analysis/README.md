# Music Preferences Analysis

[ipynb](https://github.com/mvs834/Yandex.Practicum/blob/3aa4bea6c1e42ac87a4f471651cbefc30ebf6d9f/DA%2001%20Music%20preferences%20analysis/Music_preferences_analysis.ipynb)

## Project Description

It is necessary to test three hypotheses:

- User activity depends on the day of the week. Moreover, this manifests itself differently in Moscow and St. Petersburg.
- In Moscow, certain genres prevail on Monday mornings, while in St. Petersburg, others do. The same goes for Friday evenings — the prevailing genres depend on the city.
- Moscow and St. Petersburg prefer different genres of music. Pop music is more frequently listened to in Moscow, while Russian rap is more popular in St. Petersburg.

## Skills and Tools

- **python**
- **pandas**

## Project Execution

### Data Upload and Overview
The data describes tracks and contains information about the track, such as its title, artist, and genre, as well as information about the user, such as their city and when they listened to the music. There are missing values, and the header style is inconsistent.

### Data Preprocessing
- Missing values were replaced with "unknown".
- Obvious and implicit duplicates were identified and removed.
- Headers were converted to "snake case" format.

### Hypothesis Testing

#### Activity vs. Days of the Week
The hypothesis was confirmed:

- In Moscow, the peak of listening activity falls on Monday and Friday, with a noticeable decline on Wednesday.
- In St. Petersburg, on the other hand, people listen to more music on Wednesdays. Activity on Monday and Friday is almost equally lower than on Wednesday.

#### Beginning vs. End of the Week
The hypothesis was only partially confirmed:

- Users listen to similar music at the beginning and end of the week.
- The difference between Moscow and St. Petersburg is not too pronounced. In Moscow, Russian popular music is more frequently listened to, while in St. Petersburg, jazz is more popular.
- However, missing data call this result into question. In Moscow, there are so many missing values that the top 10 ranking of genres could have looked different if the data on genres had not been lost.

#### Genre Preferences in Moscow and St. Petersburg
The hypothesis was partially confirmed:

- Pop music is the most popular genre in Moscow, as the hypothesis suggested. Moreover, a similar genre—Russian popular music—appears in the top 10 genres.
- Contrary to expectations, rap is equally popular in Moscow and St. Petersburg.

## Conclusion

The hypotheses have been tested, and the following has been established:

1. The day of the week affects user activity differently in Moscow and St. Petersburg.
The first hypothesis was fully confirmed.

2. Musical preferences do not change much over the course of the week, whether in Moscow or St. Petersburg. Minor differences are noticeable at the beginning of the week, but they are not significant.

3. Moscow and St. Petersburg have different genre preferences. Pop music is more popular in Moscow, while Russian rap is more popular in St. Petersburg.

The third hypothesis was not confirmed. If there are differences in preferences, they are imperceptible to the majority of users.