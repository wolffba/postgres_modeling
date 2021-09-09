The goal of this project was to take a subset of data from the "Million Song Dataset" along with an event similator (see github page for a description: https://github.com/Interana/eventsim) and create an Extract, Transform, Load (ETL) file to process the raw data into a star schema relational database.

This process was taken in three main steps which are described below:

1) A python notebook (etl.ipynb) was used created to test the code on a subset of the database to make sure it was working.
2) A test notebook (test.ipynb) was used to ensure that the tables creation and insertion of tables was working properly.
3) After running the elt.ipynb and the test.ipynb and everything functioned properly then code from the etl.ipynb was applied to the main executable file (etl.py) to process files over the entire song and log file directories.

Description of files:

1) 'data' -  This is the location of data from the "Millon Song Dataset" ('song_data' directory) and the event simulator ('log_data' directory).

2) 'create_tables.py' - This file implements the code to create and drop databases in postgreSQL for each time a connection is made to the postgreSQL database

3) 'etl.ipynb' - Notebook with code on a subset of the database

4) 'etl.py' - Final executeable file to run the full ETL process

5) 'sql_queries.py' - Implements the code for creating tables and inserting data into the tables into postgreSQL.

6) 'test.ipynb' - Notebook that excutes the postgresSQL database to ensure the tables and inserted data are correct.