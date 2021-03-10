## Project Documentation

1. Discuss the purpose of this database in the context of the startup, Sparkify, and their analytical goals.
    - The NoSQL keyspace *sparktifydb* is constructed where Sparkify requests can be easily accessed and is curated to what song users are listening to.
    - They specifically are looking for answers to the following three requests:
      1. Give me the artist, song title and song's length in the music app history that was heard during sessionId = 338, and itemInSession = 4
      2. Give me only the following: name of artist, song (sorted by itemInSession) and user (first and last name) for userid = 10, sessionid = 182
      3. Give me every user name (first and last) in my music app history who listened to the song 'All Hands Against His Own'


2. State and justify your data model schema design and ETL pipeline.
    - By having exact specifications of what the end-users want, a NoSQL data model supplies them answers without needing to aggregate, filter, or join.
    - A couple of benefits of this data model are the ability to work with large data sets, having fast reads and writes (high throughput), and high availability.


### Jupyter notebook, NoSQL_Apache_Cassandra_ETL, process
  - Execute ETL pipeline for pre-processing files
  - Create an Apache Cassandra cluster
  - Create a NoSQL keyspace *sparktifydb*
  - Create tables and queries to align with each requst stated above.
  - Verifiy the results align with expectation
  - Drop the tables
  - Close the session and cluster connection
