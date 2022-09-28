# Project 1
## Investigate TMDB-Movie Data
## by Ajoke Yusuf
### Table of content
- Introduction
- Questions for analysis
- Data Wrangling
- Conclusions
- Limittation

## Introduction
In this project,I will be analysizing a movie dataset named "TMDb Movie Data".
This data set contains information about 10,000 movies collected fromThe Movie Database (TMDb) and it was gotten from @Kaggle

### Question(s) for Analysis
1) Which genre of movie made the highest profit? 1b) Which genres of movie is most popular?

2) Which Production Company made the highest profit?

3) In what year was the highest profit recorded?

4) What's the average runtime in year 2015

## Data Wrangling
The following are the preliminary wrangling steps I did in this analysis:
1. I imported the package I intend to use in my anlysis.
2. I dropped some columns that won't be needed for analysis.
3. I replaced the value 0 to np.nan
4. I dropped null values found in some columns
5. I extracted the first words in cast and genre columns since its contain multiple values

## Conclusions
From the analysis below are the key insight gotten from the questions asked during the analysis:
1. **Action movies** made the highest profit across all genres of movies. The top 5 genre of movies that makes high profit include: Action, Adventure, Comedy, Drama, Animation so if the sole propose of the movie is to make profit then most movies produced should be centered around the top 5 movies.
2. 'Steven Spielberg' is the director with most movies that made high profit.
3. In year 2015,the highest profit was made across all year, in which "Star Wars: The Force Awakens" was the title of the movie and hence it's an action movie produced by Lucas film.
4. The top five production companies of the high profit movies: are Universal Pictures,Paramount Pictures,Walt Disney Pictures,Twentieth Century Fox Film Corporation,Columbia Pictures.
5. Popularity, production companies, director, genre of movies are criteria to be considered to make high profitable movies. In order to make high profit in movies, most movies should advertised in all advertizing platform and the snapshot of the movies should be with a catching scenes that attract the audience. Also, the movie should be centered on action, adventure, comedy, drama, animation movies. Production companies like Universal Pictures,Paramount Pictures,Walt Disney Pictures,Twentieth Century Fox Film Corporation,Columbia Pictures should be the one in charged of production.
## Limitations
After a thorough exploratory analysis, I realized the analysis is biased due to the insufficient dataset provided.During the cleaning process, I observed that more than 50% values in revenue_adj and budget_adj contain zero values which was assumed to be null because in reality, revenue and budget can never be zero. All the entries that has zeros value was replaced with NaN and dropped. The significance removal of >50% makes interpretation bias.

The entries in the: cast, genre and directors fields has >1 values joined together with '|' so i had to split the values by extracting only the first entires in each of the three columns






