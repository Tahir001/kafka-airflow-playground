# kafka-playground
A small pet project to play around with Kafka 

# Technical Requirements 
You will need: Python3, Postgres, Docker, Docker-compose, Kafka, Kafka-python and Zookeeper.

# Details 
The following project uses Zookeeper to manage a Kafka Cluster to create a new topic called Toll Plaza which keeps track of incoming cars. 

We use a kafka producer to produce incoming traffic

Which then gets taken by a Kafka consumer, and ingested into a Postgres Database. 

