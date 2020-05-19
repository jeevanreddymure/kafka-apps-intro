# kafka-apps-intro
## Commands for Kafka:
All the commands should be executed using powershell opened in kafaka directory
- Running Zookeeper service (Run in its own window): `.\bin\windows\zookeeper-server-start.bat .\config\zookeeper.properties`
- Running Kafka service (Run in its own window): `.\bin\windows\kafka-server-start.bat .\config\server.properties`
- Creating a topic: `.\bin\windows\kafka-topics.bat --zookeeper localhost:2181 --replication-factor 1 --partitions 1 --create --topic {insert name of topic here}`
- Prompting to write a message to a topic: `.\bin\windows\kafka-console-producer.bat --broker-list localhost:9092 --topic {insert name of topic here}`
- Deleting a topic: `.\bin\windows\kafka-topics.bat --zookeeper localhost:2181 --replication-factor 1 --partitions 1 --delete --topic {insert name of topic here}`
- Listing the contents of a topic: `.\bin\windows\kafka-topics.bat --zookeeper localhost:2181 --list`
- Listing a message within a topic: `.\bin\windows\kafka-console-consumer.bat --bootstrap-server localhost:9092 --topic {insert name of topic here} --from-beginning`
## My unique commands are as follows
- `.\bin\windows\zookeeper-server-start.bat .\config\zookeeper.properties` to run Zookeeper sevice
- `.\bin\windows\kafka-server-start.bat .\config\server.properties` to run kafka service
- `.\bin\windows\kafka-topics.bat --zookeeper localhost:2181 --replication-factor 1 --partitions 1 --create --topic COVID` for creating       topic
- `.\bin\windows\kafka-topics.bat --zookeeper localhost:2181 --list` for list of toipcs
- `.\bin\windows\kafka-console-producer.bat --broker-list localhost:9092 --topic COVID` creating messages
- `.\bin\windows\kafka-console-consumer.bat --bootstrap-server localhost:9092 --topic COVID --from-beginning` for listing messages
