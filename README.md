# Movies-ETL
Extract, Transform, Load

## Purpose
1. Create an ETL pipeline from raw data to a SQL database.
2. Extract data from disparate sources using Python.
3. Clean and transform data using Pandas.
4. Use regular expressions (Regex) to parse data and to transform text into numbers.
5. Load data with PostgreSQL and verify in PgAdmin.

The project included extracting a large data set from Kaggle, then transforming the data into a usable dataset for a "hacking competition."  Once the data was transformed and narrowed in scope for the hack-a-thon, the DataFrames were loaded into PostgresSQL.  

## Extracting
Wikipedia Movies JSON file, starting with 193 Columns:
![Pic 1](https://github.com/Baylex/Movies-ETL/blob/main/Resources/d1_1wiki_movies.PNG)

Kaggle Movie Metadata, 24 columns
![Pic 2](https://github.com/Baylex/Movies-ETL/blob/main/Resources/d1_2kaggle_metadata.PNG)

Kaggle Ratings data, 2602489 rows by 4 columns

![Pic 3](https://github.com/Baylex/Movies-ETL/blob/main/Resources/d1_3ratings.PNG)

## Transforming 
### Wikipedia Data
Wikipedia Movies transformed, 22 columns
![Pic 4](https://github.com/Baylex/Movies-ETL/blob/main/Resources/d2_1wiki_movies.PNG)

Wikipedia Movies, making the column names more succinct and uniform, 7033 rows of data.
![Pic 5](https://github.com/Baylex/Movies-ETL/blob/main/Resources/d2_2wiki_movie_counts.PNG)

### Kaggle Data
Wikipedia Movies merged with Kaggle Movies data, all column names and row counts, 6052 rows.
![Pic 8](https://github.com/Baylex/Movies-ETL/blob/main/Resources/d3_6movies.PNG)

Merged Movies with Kaggle ratings, all of the column names and row counts, 6052 rows.

![Pic 9](https://github.com/Baylex/Movies-ETL/blob/main/Resources/d3_5movies_ratings.PNG)

## Loading
### Creating the Movie Database
Sending the data to PostgresSQL
![Pic 10](https://github.com/Baylex/Movies-ETL/blob/main/Resources/d4_final_send.PNG)

### Verifying the data in PgAdmin
Movies Query

![Pic 11](https://github.com/Baylex/Movies-ETL/blob/main/Resources/movies_query.PNG)

Ratings Query

![Pic 12](https://github.com/Baylex/Movies-ETL/blob/main/Resources/ratings_query.PNG)

## Summary

A JSON file and 2 Kaggle files were extracted, then transformed, and joined.  A movies and ratings file were loaded into a database for the hack-a-thon event.
