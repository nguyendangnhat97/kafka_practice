Step 1: Install Kafka
wget https://archive.apache.org/dist/kafka/2.8.0/kafka_2.12-2.8.0.tgz
tar -xzf kafka_2.12-2.8.0.tgz

Step 2: Start Mysql Server
Then create a database named tolldata, create a table named livetolldata(timestamp datetime, vehicle_id int,
vehicle_type char(15), toll_plaza_id smallint)

Step3: Install kafka-python and mysql-connector-python

Step 4: Start Zookeeper and Kafka Server
bin/zookeeper-server-start.sh config/zookeeper.properties
bin/kafka-server-start.sh  config/server.properties

Step 5: Configure toll_traffic_generator.py and streaming_data_reader.py then run
