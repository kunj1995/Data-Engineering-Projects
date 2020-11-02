# Project 3: Data Lakes

### Introduction:
A music streaming startup, Sparkify, has grown their user base and song database even more and want to move their data warehouse to a data lake. Their data resides in S3, in a directory of JSON logs on user activity on the app, as well as a directory with JSON metadata on the songs in their app.

### Porject goal:
In this project we will build an ETL pipeline that extracts their data from the data lake hosted on S3, processes them using Spark which will be deployed on an EMR cluster using AWS, and load the data back into S3 as a set of dimensional tables in parquet format.

### Database Schema:

#### Fact Table
songplays - records in event data associated with song plays (records with page = NextSong)
start_time, userId, level, sessionId, location, userAgent, song_id, artist_id, songplay_id  

#### Dimension Tables
users - users in the app
songs - songs in music database
artists - artists in music database
time - timestamps of records in songplays
  
   
### ETL Pipeline
Load credentials
Read data from S3
Process data using spark
Load it back to S3

### How to run the project
   1) Add appropriate AWS IAM Credentials in dl.cfg.
   2) Specify desired output data path in the main function of etl.py and run etl.py.
