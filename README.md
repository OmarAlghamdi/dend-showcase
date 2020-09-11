# DEND Showcase
Here you can find brief description of the projects I did during my journey through [Udacity's Data Engineering Nanodegree](https://www.udacity.com/course/data-engineer-nanodegree--nd027).

## ETL Process & Relation Modeling
In the first project I implemented an [ETL](https://en.wikipedia.org/wiki/Extract,_transform,_load) process using Python's Pandas to Extract data from JSON files, Transform them into a [Start Schema](https://en.wikipedia.org/wiki/Star_schema#:~:text=The%20star%20schema%20is%20an,it%20representing%20the%20star's%20points.), then Load them into PostgreSQL DB.

You can find full details [here](https://github.com/OmarAlghamdi/Sparkify-relational).

## ETL Process & NoSQL
In the second project I implemented an ETL process using [Apache Cassandra](https://cassandra.apache.org/) be able to answer few question about the data. Each question (query) had its own table.

You can find full details [here](https://github.com/OmarAlghamdi/Sparkify-NoSQL).

## ETL Pipeline In The Cloud
In the third project I implemented similar ETL process to the one I did in the first project. But, I implanted it to scale to handle Big Data. I used an [AWS Redshift](https://aws.amazon.com/redshift/?whats-new-cards.sort-by=item.additionalFields.postDateTime&whats-new-cards.sort-order=desc) cluster to stage (Extract) the Data from [AWS S3](https://aws.amazon.com/s3/) to Redshift, Transform it into Star Schema, then Load it to dimensional tables.

You can find full details [here](https://github.com/OmarAlghamdi/sparkify-cloud-etl).

## Spark & Data Lake
In the fourth project I a [Spark](https://spark.apache.org/) cluster to process data read from AWS S3 (Extract) into dimensional model (Transform). The I Loaded the data back to S3 in [parquet forma](https://parquet.apache.org/documentation/latest/) to allow data to scale in size nicely without paying for always-on Spark cluster (created only during the run time of the ETL process).

You can find full details [here](https://github.com/OmarAlghamdi/sparkify-data-lake-spark).

## Pipeline Scheduling With Airflow
In the fifth project I used [Apache Airflow](https://airflow.apache.org/) to schedule the ETL pipeline I built in the third project. The goal was to make Airflow automate the ETL process and make it run each hour to account for new data.

You can find full details [here](https://github.com/OmarAlghamdi/sparkify-airflow-pipeline).

## Preparing Bike Share Data For Business Analysis
In the capstone project it was time to prove my competent and put what I learned throughout the Nanodegree into practice.

I was free to define the scope of my project and use data I think is useful. I chose to prepare [data from a Bike Sharing service based In the San Francisco, CA (fictional)](https://www.kaggle.com/benhamner/sf-bay-area-bike-share) for business analysis.

I implemented an ETL pipeline using Spark running on [AWS EMR](https://aws.amazon.com/emr/?whats-new-cards.sort-by=item.additionalFields.postDateTime&whats-new-cards.sort-order=desc) cluster. Data is Extracted from and Loaded in S3 to enable data to scale in term of size and concurrent reads.

You can find full details [here](https://github.com/OmarAlghamdi/dend-capstone).
