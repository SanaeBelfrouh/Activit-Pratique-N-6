# Activit-Pratique-N-6
Activité Pratique N°6 : Systèmes Distribués Asynchrones avec FAFKA  et Spring Cloud Stream

1
## Kafka Server
kafka-server-start.bat ..\..\config\server.properties

 ![kafka](https://github.com/SanaeBelfrouh/Activit-Pratique-N-6/assets/116807307/930cf206-030d-4ff0-9cdb-d097fe15448e)
## ZooKeeper
zookeeper-server-start.bat ..\..\config\zookeeper.properties
![zookeeper](https://github.com/SanaeBelfrouh/Activit-Pratique-N-6/assets/116807307/6cd19e58-937f-4a2e-948f-2426d3633da4)
## Tester avec Kefka-console-producer et kafka-console-consumer
[Uploading Video_2023_06_02-2_edit_0.webm…]()

## Producer
kafka-console-producer.bat --broker-list localhost:9092 --topic R1

![Consolproducer](https://github.com/SanaeBelfrouh/Activit-Pratique-N-6/assets/116807307/29c8f3a0-0f86-4cef-9b1d-6080043dccf1)

## Consumer
kafka-console-consumer.bat --bootstrap-server localhost:9092 --topic R1

![LOCALLHOSTBLOG](https://github.com/SanaeBelfrouh/Activit-Pratique-N-6/assets/116807307/85c40ef8-e2f6-4aca-97f0-1526c2270da9)

![costumer service](https://github.com/SanaeBelfrouh/Activit-Pratique-N-6/assets/116807307/3a7531b3-6f90-44fc-aa07-a5381b2a10c9)
## Flux de donnée chaque 100 s:
kafka-console-consumer.bat --bootstrap-server localhost:9092 --topic R2
![R2](https://github.com/SanaeBelfrouh/Activit-Pratique-N-6/assets/116807307/6faf49fa-50c1-44e4-8427-c2145b029193)

## Analytics:
![ANALYS](https://github.com/SanaeBelfrouh/Activit-Pratique-N-6/assets/116807307/e49efdad-3991-4295-9091-a050bc69d0d8)

Graph represenation using js:

[doker.webm](https://github.com/SanaeBelfrouh/Activit-Pratique-N-6/assets/116807307/7a2fc5a2-eb8e-4470-8205-d88ae0020147)
