# Movie recommendations.
## Introduction:
For this project, we will use the "small" dataset from [GroupLens](https://grouplens.org/datasets/movielens/latest/). This dataset includes four main files:

- **movies.csv**: Contains information about each movie, including its ID, title, and genres.  
- **ratings.csv**: Records user ratings, with fields for user ID, movie ID, rating, and timestamp.  
- **tags.csv**: Aggregates user-generated keywords associated with movies.  
- **links.csv**: Provides mappings between MovieLens IDs and external databases such as IMDb and TMDB.

Since good recommendations play an important role in client satisfaction we will make of Our objective to develop a recommendation system that can automatically suggest the top 5 movies to a given user. These recommendations will be based on the user's past ratings and those of similar users.
 ## Methodology
 #### **Exploratory data Analysis**
 - dataset overview & cleaning
 - dataset description
 - data/ business understanding
 #### **Major questions**
 this part will sharpen our understanding of the data and the business task.
 Major questions will be answered.
 they will help us grasp the data.

#### **Modelisation**
- data preparation for modelisation
- building Matrix
- collaborative filtering
- training/ optimisation of SVD model

#### **Contact information**
- name
- email
- phone number
- LinkedIn
##  Exploratory data Analysis
#### **Dataset overview & cleaning**
the datasets movies_csv and ratings.csv that we will use are already cleaned which simplifies the process
#### **Dataset Description**
Some description have been provided in the introduction of this project. For more description of the data you may wanna read this:
The dataset is composed of four main files:
movies.csv: contains information about the movies (ID, title, genres). ratings.csv: contains user ratings (userId, movieId, rating, timestamp). tags.csv: gathers keywords associated with movies by users. links.csv: provides mappings between MovieLens IDs, IMDb, and TMDB.
For this project, we will focus on movies.csv and ratings.csv, as they form the foundation of collaborative filtering:
ratings.csv allows us to build the user–movie matrix based on the ratings given.
#### **business understanding**
Video streaming platforms face a major challenge: delivering relevant content to each user from an immense catalog. Without personalized recommendations, users may feel lost and leave the platform, leading to lower retention.
Our goal is to build a recommendation system capable of automatically suggesting the top 5 movies to a user, based on their past ratings and those of similar users.
This collaborative filtering model will analyze shared behaviors among users to predict future preferences. By integrating such a solution, a streaming company can enhance the user experience, increase engagement, and reduce churn.
The key idea behind collaborative filtering is that similar users share similar interests, and users tend to like items that others with similar tastes also enjoy.
## Major Questions
#### What does the distribution of ratings reveal?
**Answer** : most ratings fall between 3 and 5, suggesting a generally positive trend.
#### What does the distribution of ratings per user reveal about user activity levels?
**Answer**
some users are highly active while others contribute very few ratings, highlighting the imbalance.
