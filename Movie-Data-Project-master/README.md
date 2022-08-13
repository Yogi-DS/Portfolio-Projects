# Movie-Data-Project

## by Yograj, Luiz and Andrew.

Data Sources:
1. Kaggle
https://data.world/data-society/imdb-5000-movie-dataset
2. PromptCloud (Found in Kaggle though)
https://www.kaggle.com/PromptCloudHQ/imdb-data



Explanation of use for your DB
We want to analyse following:
User Rating vs. Revenue
Content Rating vs. Revenue
Genre vs. Revenue
Facenumber in poster vs. Revenue



Column/Keys used (just a list)
Movie Title
Year
Genre
Actors
Rating
Metascore
Budget
Gross revenue



Which style DB and why? 
SQL because:
Reasonably small database
Easy to read and understand the relational schema
More convenient to use statistics
None to few null values


Transform strategy
Download csv files from the datasource
Import csv into pandas dataframe
Merge the two dataframes on “Movie Title”
Export a new clean csv
Import the new csv into SQL
Create mainly 3 different tables from this database: 
Movie : Title, year, duration, description, genre, director, actors
Social: Voting count, facebook likes, User rating, IMDB Score, metascore
Revenue: Budget, Gross revenue, win/loss amount or percentage
	Unique movie_id for each title will link all these tables.



Extract:
Download csv files from the datasources
1. Kaggle
https://data.world/data-society/imdb-5000-movie-dataset
2. PromptCloud (Found in Kaggle though)
https://www.kaggle.com/PromptCloudHQ/imdb-data

Imported both CSVs into pandas dataframe

Transform:
Set the columns order and dropped all unnecessary columns
Stripped off the extra spaces within the columns in order to merge both CSVs
Renamed all columns
Merged the two dataframes on “Movie Title”
Checked all missing values from the combined dataframe and dropped them
Export a new clean csv as combined_df


Load:
Created a database connection using sqlalchemy
Created a relational database with 8 tables referring to different data of the database
Actor
Actor_movie
Financial
Genre
Genre_movie
Movie
Reviews
Social_media
Ensured column order and column heads matched database schema



Why this database?
We have nice and clean data which presents best in tabular model so chose sql database for the data to load it into. 




Database Schema


