# Movie Recommender Model in R using Machine Learning

This project is built on R using machine learning libraries. In order to build this recommendation system, I have used the MovieLens Dataset. You can find the movies.csv and ratings.csv file that I have used in our Recommendation System Project here. This data consists of 105339 ratings applied over 10329 movies.

This recommender model uses Collaborative Filtering system to recommend the movie. Utilizing preferences gathered from numerous other users, collaborative filtering involves recommending movies to consumers.For instance, if user A and user B both enjoy action movies, then A will be recommended the movies that B will watch in the future, and vice versa. Therefore, establishing a commonality between the two consumers is necessary for making movie recommendations. 
I calculated similarities using a variety of operators, including cosine and pearson with the aid of recommenderlab.

### Packages used for this recommender model
- recommenderlab
- ggplot2
- reshape2
- data.table
