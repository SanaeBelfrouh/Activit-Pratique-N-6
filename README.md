# Activit-Pratique-N-6
Activité Pratique N°6 : Systèmes Distribués Asynchrones avec FAFKA  et Spring Cloud Stream
<pre>
1. 
- Télécharger Kafka
- Démarrer Zookeeper
- Démarrer Kafka-server
- Tester avec Kefka-console-producer et kafka-console-consumer
2. Avec Docker (voir https://developer.confluent.io/quickstart/kafka-docker/)
https://www.youtube.com/watch?v=9O1Kuk2xXO8
 - Créer le fichier docker-compose.yml
 - Démarrer les conteneurs docker : zookeeper et kafka-broker
 - Tester avec Kafka-console-producer et kafka-console-consumer
3. 
En Utilisant KAFKA et Stpring Cloud Streams, Créer :
- Un Service Producer KAFKA via un Rest Controler
- Un Service Consumer KAFKA
- Un Service Supplier KAFKA
- Un Service de Data Analytics Real Time Stream Processing avec Kaflka Streams
- Une application Web qui permet d'afficher les résultats du Stream Data Analytics en temps réel
</pre>
## Kafka Server
<pre>
kafka-server-start.bat ..\..\config\server.properties
</pre>
 ![kafka](https://github.com/SanaeBelfrouh/Activit-Pratique-N-6/assets/116807307/930cf206-030d-4ff0-9cdb-d097fe15448e)
## ZooKeeper
<pre>
zookeeper-server-start.bat ..\..\config\zookeeper.properties
</pre>
![zookeeper](https://github.com/SanaeBelfrouh/Activit-Pratique-N-6/assets/116807307/6cd19e58-937f-4a2e-948f-2426d3633da4)
## Tester avec Kefka-console-producer et kafka-console-consumer
[Uploading Video_2023_06_02-2_edit_0.webm…]()

## Producer
<pre>
kafka-console-producer.bat --broker-list localhost:9092 --topic R1
</pre>
![Consolproducer](https://github.com/SanaeBelfrouh/Activit-Pratique-N-6/assets/116807307/29c8f3a0-0f86-4cef-9b1d-6080043dccf1)

## Consumer
<pre>
kafka-console-consumer.bat --bootstrap-server localhost:9092 --topic R1
</pre>
![LOCALLHOSTBLOG](https://github.com/SanaeBelfrouh/Activit-Pratique-N-6/assets/116807307/85c40ef8-e2f6-4aca-97f0-1526c2270da9)

![costumer service](https://github.com/SanaeBelfrouh/Activit-Pratique-N-6/assets/116807307/3a7531b3-6f90-44fc-aa07-a5381b2a10c9)
## Flux de donnée chaque 100 s:
<pre>
kafka-console-consumer.bat --bootstrap-server localhost:9092 --topic R2
</pre>
![R2](https://github.com/SanaeBelfrouh/Activit-Pratique-N-6/assets/116807307/6faf49fa-50c1-44e4-8427-c2145b029193)

## Analytics:
![ANALYS](https://github.com/SanaeBelfrouh/Activit-Pratique-N-6/assets/116807307/e49efdad-3991-4295-9091-a050bc69d0d8)

Graph represenation using js:

[doker.webm](https://github.com/SanaeBelfrouh/Activit-Pratique-N-6/assets/116807307/7a2fc5a2-eb8e-4470-8205-d88ae0020147)
