# movie-reocommender-system
Movie Recommendation System

#Dataset Link:
https://www.kaggle.com/tmdb/tmdb-movie-metadata?select=tmdb_5000_movies.csv

#Steps to build Movie Recommeder System
1. Import all necessary libraries.
2. Import datasets. Here in this system, 2 data sets are being used i) tmdb_5000_movies.csv ii) tmdb_5000_credits.csv.  Since both the data sets are giving the same movie information, it is going to be combined.
3. This recommendation system is based on content based. Based on that, it is necessary to identify, which attributes are not necessary and drop those all attributes which are not contributing.
4. Concatenate overview, generes, keywords, cast and crew,  make new column called tags(newly created dataset has columns as movie_id, title, tags).
5. Recommendation is based on similarity score. Convert text to vector and apply vectorization, not considering stop words, using stemming similarity score can be calculated. 

