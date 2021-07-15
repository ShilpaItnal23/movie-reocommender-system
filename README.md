# movie-reocommender-system
Movie Recommendation System

# Dataset Link:
https://www.kaggle.com/tmdb/tmdb-movie-metadata?select=tmdb_5000_movies.csv

# Steps to build Movie Recommeder System

1. Import all necessary libraries.
2. Import datasets. Here in this system, 2 data sets are being used i) tmdb_5000_movies.csv ii) tmdb_5000_credits.csv.  Since both the data sets are giving the same movie information, it is going to be combined.
3. This recommendation system is based on content based. Based on that, it is necessary to identify, which attributes are not necessary and drop those all attributes which are not contributing.
4. Concatenate overview, generes, keywords, cast and crew,  make new column called tags(newly created dataset has columns as movie_id, title, tags).
5. Recommendation is based on similarity score. Convert text to vector and apply vectorization, not considering stop words, using stemming similarity score can be calculated.
6. Each movie is compared with all other movies, the distance between them is calculated using cosine angle(angle between two vecotrs) not with Euclidian distance(distance betweenn two vectors). Thus 5 movies will be recommended.

#  Steps to create website.
1. Web app is built using stremlit
2. Fetch 5 movies
3. Fetch 5 posters. To do go to TMDB API. Get details, try it out, copy paste the link. In that link, copy paste the api along with movie id. Once that is done, you will get movie information.
4. Using JSON reader, you can view the data properly. Fetch poster path. Using which you are going to fetch the posters.
5. In your localhost, you are going to see the Movie-Recommendation-System as shown below.



