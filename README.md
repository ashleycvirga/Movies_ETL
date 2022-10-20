# Movies_ETL
Extract, Transform and Load Movie Data for Amazing Prime

# Overview & Purpose of the Project 

The goal of this project is to provide Amazing Prime with an automated ETL pipeline so that they may keep their movie data updated on a daily basis.  This automated pipeline takes in new data, performs the appropriate transformations, and loads the data into existing tables. I refactored the code from this module to create a singular function that takes in the three files—Wikipedia data, Kaggle metadata, and the MovieLens rating data—performs the ETL process and finally adds the data to a PostgreSQL database.

## Deliverables

### 1: Write an ETL Function to Read Three Data Files

### 2: Extract and Transform the Wikipedia Data

### 3: Extract and Transform the Kaggle Data

### 4: Create the Movie Database

## Notes

I would like to note that for Deliverable 2, my clean DataFrame "wiki_movies_df" has dropped the original uncleaned columns for 'Box Office', 'Budget', 'Release date', and 'Running time' as they were replaced with the new clean data columns 'box_office', 'budget', 'release_date', and 'running_time' respectively.

This was done in an effort to remove superlative data, uncleaned data and improve readability.

This does differ from the Module 8 Challenge Instructions examples. 
