##Project Data Modeling with Postgres


#Introduction

A startup called Sparkify wants to analyze the data they've been collecting on songs and user activity on their new music streaming app. The analytics team is particularly interested in understanding what songs users are listening to. Currently, they don't have an easy way to query their data, which resides in a directory of JSON logs on user activity on the app, as well as a directory with JSON metadata on the songs in their app.

They'd like a data engineer to create a Postgres database with tables designed to optimize queries on song play analysis, and bring you on the project. Your role is to create a database schema and ETL pipeline for this analysis. You'll be able to test your database and ETL pipeline by running queries given to you by the analytics team from Sparkify and compare your results with their expected results.


#Project Goal
The aim of the project is to build a Postgres Database Schema and ETL pipeline for a fictional startup music streaming company called 'Sparkify'. This database allows data engineer to aggregate all songs by using SQL and the star scheme, joins and aggregation


#Database Schema
In order to enable Sparkify to analyze their data, a star schema was created, which can be filled with an ETL pipeline.

To fill the relational database, an ETL pipeline is used, which makes it possible to extract the necessary information from the log files of the user behaviour as well as the corresponding master data of the songs and convert it into the schema.

Fact Table: songplays
Dimension Tables: users, songs, artists and time.

#How to run the python scripts 

* Ensure all file in the same folder 
* Run the script to generate the database and tables by writing 'python create_tables.py' command in terminal console
* Load and Insert data to the database by writing 'python etl.py'command in terminal console
* Open 'test.ipynb' and run all the code to verify the result. 

#Files in repository 
* **[data](data)**: Folder containing data of songs and logs 
* **[create_tables.py](create_tables.py)**: Python script to perform SQL-Statements for creating database and tables
* **[sql_queries.py](sql_queries.py)**: Python script containing SQL queries used by create_tables.py and etl.py
* **[etl.py](etl.py)**: Python script to reads and processes files from song_data and log_data and loads them into your tables
* **[test.ipynb](test.ipynb)**: Verify created tables and confirm the data is stored correctly.
