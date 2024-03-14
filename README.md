STEP 1: GET KAFKA
Download the latest Kafka release and extract it:

$ tar -xzf kafka_2.13-3.7.0.tgz

$ cd kafka_2.13-3.7.0

STEP 2: START THE KAFKA ENVIRONMENT

NOTE: Your local environment must have Java 8+ installed.

Apache Kafka can be started using ZooKeeper or KRaft. To get started with either configuration follow one the sections below but not both.

Kafka with ZooKeeper

Run the following commands in order to start all services in the correct order:

# Start the ZooKeeper service

$ bin/zookeeper-server-start.sh config/zookeeper.properties

Open another terminal session and run:

# Start the Kafka broker service

$ bin/kafka-server-start.sh config/server.properties

Once all services have successfully launched, you will have a basic Kafka environment running and ready to use.

REATE A TOPIC TO STORE YOUR EVENTS

Open another terminal session and run:

$ bin/kafka-topics.sh --create --topic quickstart-events --bootstrap-server localhost:9092

<img width="517" alt="image" src="https://github.com/NavyaTrilok/Spark-Kafka-Streaming/assets/14071348/476ff1cc-d3e0-4a54-b10e-2b6c54f7bd5a">

<img width="328" alt="image" src="https://github.com/NavyaTrilok/Spark-Kafka-Streaming/assets/14071348/849930c4-82b9-4982-8764-fe626843ca5c">

<img width="468" alt="image" src="https://github.com/NavyaTrilok/Spark-Kafka-Streaming/assets/14071348/cf72e65b-6a1a-4bfd-90da-ca811bc4af90">


