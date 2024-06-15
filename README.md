# kafka-playground
A small pet project to play around with Kafka 

# Technical Requirements 
You will need: Python3, Postgres, Airflow, Docker, Docker-compose, Kafka, Kafka-python and Zookeeper.

# Details - Kafka Project
The following project uses Zookeeper to manage a Kafka Cluster to create a new topic called Toll Plaza which keeps track of incoming cars at different Plazas.

We use a Kafka producer to produce incoming traffic, a consumer to read the traffic, and post relevent information into a Postgres Database. 

# Details - Airflow Project

Setup Airflow DAG such that it preforms ETL ona daily basis. 
We setup a dag which downloads public vehicle data, transforms the data (Cleaning, filtering, etc.) and then loads it up to a Postgres DB. 
