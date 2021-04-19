# Movie Analysis- Extract Transform Load

## Project Overview

Amazing Prime, a video streaming company is sponsoring a hackathon, where participants are tasked with predicting which low budget movies being released will become the most popular.  In order to build the predictive models we must build an ETL pipeline for further analysis.

The purpose of this project is to create a refactorable ETL pipeline that will automate the processing of large datasets into a SQL database.

## Resources
- Data Sourced from [IMDB](https://developer.imdb.com/?ref=ft_ds), [Kaggle](https://www.kaggle.com/):
  -  [ratings.csv](https://github.com/agregorash/Movies-ETL/blob/main/Resources/.gitignore) 
  -  [movies_metadata.csv](https://github.com/agregorash/Movies-ETL/blob/main/Resources/movies_metadata.csv) 
  -  [wikipedia-movies.json](https://github.com/agregorash/Movies-ETL/blob/main/Resources/wikipedia-movies.json)
               
 - Software: Python 3.8.3, Jupyter Notebooks, Anaconda 3, pgAdmin 4

## Stages of the Pipeline

-**Extract**- Data is read into the python environment using Pandas from two differing formats; csv and json.  

-**Transform**- Data is transformed into a usable dataset that can be loaded into the database.  Data cleaning included assessing missing values, null values, handling corrupt data, and formatting.  Then data was filtered, formatted, classified into understandable categories, and finally merged.

-**Load**- Created a connection to the database from the python environment and loaded in the final dataset.

## Results
The result of this project is a [single function](https://github.com/agregorash/Movies-ETL/blob/main/ETL_create_database.ipynb) that can be called to clean and transform any movie data from the given data sources and load it into SQL where further analyses can be performed.  
