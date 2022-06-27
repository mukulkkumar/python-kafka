# Python - Kafka

- **Kafka commands:-**

*To create a topic*
```
./kafka-topics.sh --bootstrap-server localhost:9092 --create --topic registered_user
```

*To list a topic*
```
./kafka-topics.sh --bootstrap-server localhost:9092 --list
```

*To describe a topic*
```
./kafka-topics.sh --bootstrap-server localhost:9092 --describe --topic registered_user
```

*To describe a consumer group*
```
./kafka-consumer-groups.sh --bootstrap-server localhost:9092 --describe --group consumer-group-a
```

**We have to first start the producer to push messages into the topic and then consumer to pull messages from the topic.**

*To start the producer*
- python producer.py

*To start the consumer*
- python consumer.py

*Note:- Before starting the producer and consumer, we need to start zookeeper and kafka server and create a topic registered_user*
