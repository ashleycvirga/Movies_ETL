# Movies_ETL
Extract, Transform and Load Movie Data for Amazing Prime

# Overview & Purpose of the Project 

The goal of this project is to provide Amazing Prime with an automated ETL pipeline so that they may keep their movie data updated on a daily basis. 

I have refactored code from the module to create a singular function that takes in new data from the three files—Wikipedia data, Kaggle metadata, and the MovieLens rating data—performs the appropriate transformations and is completed by loading the data into existing tables in a PostgreSQL database.

## Deliverables

### 1: Write an ETL Function to Read Three Data Files

[ETL_function_test.ipynb](https://github.com/ashleycvirga/Movies_ETL/blob/1c5b516f62ce1054698c7bc57843e11b65c137f9/ETL_function_test.ipynb)

### 2: Extract and Transform the Wikipedia Data

[ETL_clean_wiki_movies.ipynb](https://github.com/ashleycvirga/Movies_ETL/blob/1c5b516f62ce1054698c7bc57843e11b65c137f9/ETL_clean_wiki_movies.ipynb)

### 3: Extract and Transform the Kaggle Data

[ETL_clean_kaggle_data.ipynb](https://github.com/ashleycvirga/Movies_ETL/blob/c12c6b598e89873383b006d8283ad6ef045836aa/ETL_clean_kaggle_data.ipynb)

### 4: Create the Movie Database

[ETL_create_database.ipynb](https://github.com/ashleycvirga/Movies_ETL/blob/71533002262359b3af77c249b5306929f64d6e86/ETL_create_database.ipynb)

Confirmed the 'movies' table has 6,052 rows.

![movies_query.png](Resources/movies_query.png)

Confirmed the 'ratings' table has 26,024,289 rows.

![ratings_query.png](Resources/ratings_query.png)

## Notes

I would like to note that for Deliverable 2 & 3, my clean DataFrame "wiki_movies_df" has dropped the original uncleaned columns for 'Box Office', , 'Release date', and 'Running time' as they were replaced with the new clean data columns 'box_office', 'budget', 'release_date', and 'running_time' respectively.

This was done in an effort to remove superlative/uncleaned data and improve readability.

The module examples retained 'Release date' along with 'release_date' and 'Budget' along with 'budget' in their version of "wiki_movies_df".

## Software Used

Python v. 3.7.13
  Pandas v. 1.3.5
  Numpy v. 1.21.5
  JSON
  Sqlalchemy v. 1.4.39
  Psycopg2 v. 2.9.4
  
Jupyter Notebook v. 6.4.11

PgAdmin4 v. 6.12
  PostgreSQL 11
