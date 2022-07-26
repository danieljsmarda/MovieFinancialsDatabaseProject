# Elements of Databases - The University of Texas at Austin
Hi, welcome to the repo for the full-course project of the University of Texas at Austin Elements of Databases course. The course was a comprehensive data engineering course discussing both theory and implementation of relational databases and ETL/big data processing using AWS -- EMR, S3, Athena, RDS (Postgres), Quicksight -- and PySpark. 

In the "Labs" section, a basic IMDB database is created and a schema is designed and implemented. The database is queried and important information visualized with Quicksight. In the "Final Project" section, additional information is ingested from two other online data soucres to result in a comprehensive movie database with title, actor, tag (content), and financial (box office) information of both Hollywood and Bollywood movies.

Descriptions of the deliverable tasks associated with each assignment are explained below. Further detail can be found in the assignment instructions pdfs in the folder for each assignment. All assignments were split equally with my partner, Peter Yi.

## Labs
### Lab 1
Execution of table creation (DDL) statements. Execution of basic SQL queries on an IMDB dataset stored in Amazon S3 buckets and analysis of resulting data using Amazon Quicksight. ERD (Entity Relation Diagram) creation for IMDB database schema.

### Lab 2
Creation of a PostgreSQL instance of Amazon RDS. Population of the instance with the IMDB dataset. Query execution on movie rating information. Design of a star schema for movie rating analysis.

### Lab 3
**Part 1**: Execution of intermediate-level queries (aggregate queries) and creation of corresponding virtual and/or materialized views of various sections of the IMDB dataset. Amazon Quicksight visualization of the results of these queries. 
**Part 2**: Implementation of the star schema designed in Part 1. Aggregate query execution and Amazon Quicksight visualization of meaningful movie rating data from this schema. 

## Final Project
The final project was divided into four milestones. Lab 1, Lab 2, and Lab 3 used exclusively a common IMDB dataset. The final project outlines an ETL process for ingesting data from two other common movie databases: Cinemalytics (a Bollywood equivalent of IMDB) and Movielens (an academia-based movie recommendation website). All .py files are PySpark scripts. 
#### Milestone 1:
Exploration of the Movielens dataset and ingestion into our previously-configured IMDB database. Configuring of an Amazon EMR (Elastic MapReduce) cluster for Spark job processing.
#### Milestone 2:
Further ingestion (ETL) of Movielens data (specifically, tag data).
#### Milestone 3:
Ingestion of online financial box office data into our database. Query optimization using indices.
#### Milestone 4: 
Full ingestion and cleaning of Cinemalytics dataset. Final ERD of complete database with IMDB, Movielens, box office, and Cinemalytics data.
