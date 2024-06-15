# kafka-aiflow-playground
A small pet project to play around with Kafka and Airflow

# Technical Requirements 
You will need: Python3, Postgres, Airflow, Docker, Docker-compose, Kafka, Kafka-python and Zookeeper.

# Details - Kafka
The following project uses Zookeeper to manage a Kafka Cluster to create a new topic called Toll Plaza which keeps track of incoming cars at different Plazas.

We use a Kafka producer to produce incoming traffic, a consumer to read the traffic, and post relevent information into a Postgres Database. 

# Replication:

1. Run the `docker-compose up` command in the project directory to run the Zookeeper and Kafkaserver on a connected dockerized network
2. Create a new topic called toll:
   `docker exec -it mykafkaserver /opt/kafka/bin/kafka-topics.sh --create --topic toll --bootstrap-server localhost:9092`
3. 
