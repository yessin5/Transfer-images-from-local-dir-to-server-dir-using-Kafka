The goal of this project is to transfer images from local directory named "local_dir" to a server directory named "server" using Kafka and Kafka-python.

The project consists of 2  python scripts:

producteur.py : It's job is to send the images

comsommateur.py : It's job is to read the images 

To start this project you have to:
- Start Zookeeper using these commands:
  
C:\Users\hp>cd C:\kafka_2.12-3.7.0

C:\kafka_2.12-3.7.0>start bin\windows\zookeeper-server-start.bat config\zookeeper.properties

- Start a kafka server using this command:
  
C:\kafka_2.12-3.7.0>start bin\windows\kafka-server-start.bat config\server.properties

- Open your Python IDE and run these commands on separated Terminal windows:
bin/zookeeper-server-start.sh config/zookeeper.properties 
bin/kafka-server-start.sh config/server.properties


Requirements:
- Apache Kafka: https://kafka.apache.org/downloads
- Kafka library on python: https://pypi.org/project/kafka-python/
