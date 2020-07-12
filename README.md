# IMBD-movie-data

It all started pretty inocuous, talking about our likes and dislikes, but when we started talking about movies, everything when from 0 to 200mph in 3 seconds. How do you decide what to watch? Is there that much of a difference between the critics reviews and the people? Which one is more harsh? Also, can that be considered successful? What about the money? Is it relevant the director or the budget if a movie is successful? Those are some of the questions we are trying to answer with this project.

![Image retrived from Panorama Audiovisual](https://www.panoramaaudiovisual.com/wp-content/uploads/2019/06/IMDB.jpg)

## Data

The data was retrived from Kaggle and it was updated by Stefano Leone, you can find the original [here](https://www.kaggle.com/stefanoleone992/imdb-extensive-dataset). This Dataset was scraped from IMDb, which is the most popular movie website. This site combines movie plot description, Metasore ratings, critic and user ratings and reviews, release dates, list of actors, general information about them, and many other aspects.

It contains 4 csv files, dividing the data into 4 aspects:

* Movies: contains 81,273 movies with 22 attributes
* Names (cast members): contains 175,719 cast members with 20 attributes
* Ratings: contains 81,273 movies with 49 attributes
* Title Principals (cast members roles): contains 377,848 cast members roles in movies with 6 attributes

Since our interests relied on the ratings and the movies, we only end up using those two csv files.

## Process

We decided to divide the project into two sections:

1. One dedicated to the reviews of the movies, to analize who, between the critic and the viewer, is harsher when they rate the movies.
2. The second, to review the success of a movie in terms of revenue per director and the user ratings vs the budget.

### Critic Scores vs. Viewer Ratings (information extracted from [this repository](https://github.com/patelpurvip/IMDB_ratings_analysis))

#### Cleaning

For this process, we decided to delete movies without reviews from both critics and viewers.