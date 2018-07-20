# Kafka-producer-consumer
Kafka producer and consumer example

# Zookeeper
## Start Zookeeper using below command in windows
zookeeper-server-start.bat ../../config/zookeeper.properties


Note: For windows we have a separate windows folder having batch files.



# Kafka
## Start Kafka server using below command in windows
 kafka-server-start.bat ../../config/server.properties
 
 
 # Kafka topic
 ## Create Kafka topic using the below command
  kafka-topics.bat --create --zookeeper localhost:2181 --replication-factor 1 --partitions 1 --topic Kafka_Example
 
 kafka-console-consumer.bar --bootstrap-server localhost:9092 --topic Kafka_Example --from-beginning