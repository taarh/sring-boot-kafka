# Spring Boot avec Kafka Producer

## Démarrage de Zookeeper
- `zookeeper-server-start.bat config/zookeeper.properties`

## Démarrage de Kafka Server
- `kafka-server-start.bat config/server.properties`

## Création de Kafka Topic
- `bin/kafka-topics.bat --create --zookeeper localhost:2181 --replication-factor 1 --partitions 1 --topic Kafka_Example`

## Consommation des données depuis le Kafka Topic via le Console
- `bin/kafka-console-consumer.bat --bootstrap-server localhost:9092 --topic Kafka_Example --from-beginning`

## Publier le message via WebService
- `http://localhost:8081/kafka/publish/Sam`
- `http://localhost:8081/kafka/publish/Peter`
