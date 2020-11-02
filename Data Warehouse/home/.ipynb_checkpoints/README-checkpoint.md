# Project 3: Data Warehouse

### Porject goal:
This project is for music streaming startup Sparkify. Project goal is to build an ETL pipeline pipeline that extracts data from AWS S3, stage tables on Redshift and execute SQL queries to create tables from the staging tables. This data will be furthur used by analytics team at Sparkify.

### Database Schema

There are two staging tables which copies the JSON file inside the S3 buckets.

#### Staging Table
   staging_songs - info about songs and artists
   staging_events - users' actions. i.e. which song they are listening

Created a star schema optimized for queries on song play analysis. Star schema includes following tables.
Fact Table
songplays - records in event data associated with song plays i.e. records with page NextSong
Dimension Tables
users - users in the app
songs - songs in music database
artists - artists in music database
time - timestamps of records in songplays broken down into specific units
The database schema is shown as follows

