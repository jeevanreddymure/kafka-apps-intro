# kafka-apps-intro
## Commands for Kafka:
All the commands should be executed using powershell opened in kafaka directory
- Command to run a zookeeper service

  `.\bin\windows\zookeeper-server-start.bat .\config\zookeeper.properties`  
- Command for Running Kafka service  

  `.\bin\windows\kafka-server-start.bat .\config\server.properties`
- command for Creating a topic 

  `.\bin\windows\kafka-topics.bat --zookeeper localhost:2181 --replication-factor 1 --partitions 1 --create --topic {insert your unique      name here}`
- command for deleting a topic

   `.\bin\windows\kafka-topics.bat --zookeeper localhost:2181 --replication-factor 1 --partitions 1 --delete --topic {insert your unique      name here}`
-  command for Listing a message within a topic

   `.\bin\windows\kafka-console-consumer.bat --bootstrap-server localhost:9092 --topic {insert your unique name here} --from-beginning`
## My unique commands are as follows
- `.\bin\windows\zookeeper-server-start.bat .\config\zookeeper.properties` to run Zookeeper sevice
- `.\bin\windows\kafka-server-start.bat .\config\server.properties` to run kafka service
- `.\bin\windows\kafka-topics.bat --zookeeper localhost:2181 --replication-factor 1 --partitions 1 --create --topic COVID` for creating       topic
- `.\bin\windows\kafka-topics.bat --zookeeper localhost:2181 --list` for list of toipcs
- `.\bin\windows\kafka-console-producer.bat --broker-list localhost:9092 --topic COVID` creating messages
- `.\bin\windows\kafka-console-consumer.bat --bootstrap-server localhost:9092 --topic COVID --from-beginning` for listing messages
## References 
- [eli Ross](https://github.com/eliross84/kafka-apps-intro/blob/master/README.md)
