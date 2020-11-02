# Project 1: Data modeling with Postgres

### Porject goal:

To create a ETL pipeline and Postgres database to optimize queries for anaytics team at Sparkify.

### Database:

The database in based on a star schema.
one fact table: songplays contains columns songplay_id,start_time, user_id, 
Dimension tables: users contains columns user_id,first_name,last_name,level
                  songs contains columns song_id,title,artist_id,year,duration
                  artists contains columns artist_id,name,location,latitude,longitude
                  time contains columns start_time,hour,day,week,month,year,weekday
                  
                  
### Files in Repository:
1. Data: This folder contains all the required JSON data.
2. sql_queries.py: It containes the python script to Create, Insert, Drop tables.
3. create_tables.py: It containes the python script to connect with database and run queries of the sql_queries.
4. etl.ipynb: It contains python code to create ETL pipeline, to insert data into tables and close the connection with databse.
5. test.ipync: It contains python code to verify that the tables are created and/or data has been entered. 
6. etl.py: It contains python code to run ETL pipeline code.

### ETL Pipelines:
song_data ETL
log_data ETL

### How to run:
1. Run create_tables.py from terminal to set up the database and tables.
2. Run etl.py from terminal to process and load data into the database.
3. Launch test.ipynb to run validation and example queries.






