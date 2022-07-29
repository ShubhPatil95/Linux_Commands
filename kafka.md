Kafka_Commands

##### 1. Check log of by group name
```ruby
cd /usr/local/kafka
bin/kafka-consumer-groups.sh --bootstrap-server localhost:9092 --describe --group GROUP_NAME
```
##### 2. Increase kafka message size for topic
```ruby
cd /usr/local/kafka
bin/kafka-configs.sh --bootstrap-server localhost:9092 --entity-type topics --entity-name TOPIC_NAME --alter --add-config max.message.bytes=5000000
```
##### 3. Increase kafka message size for topic
```ruby
cd /usr/local/kafka
bin/kafka-configs.sh --bootstrap-server localhost:9092 --entity-type topics --entity-name TOPIC_NAME --alter --add-config max.message.bytes=5000000
```
