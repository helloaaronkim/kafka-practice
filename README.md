# kafka-practice

## Run Zookeper & Kafka

- Zookeeper
```
bin/zookeeper-server-start.sh config/zookeeper.properties
```

- Kafka
```
bin/kafka-server-start.sh config/server.properties
```

## Create Topic & Consumer
- Topic
```
bin/kafka-console-producer.sh --topic new-topic --bootstrap-server localhost:9092
```

- Consumer
```
bin/kafka-console-consumer.sh --topic new-topic --from-beginning --bootstrap-server localhost:9092
```

## Kafka UI
```
docker run -it -p 8080:8080 -e DYNAMIC_CONFIG_ENABLED=true provectuslabs/kafka-ui
```
