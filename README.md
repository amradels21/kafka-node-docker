# kafka-node-docker

A kafka producer/consumer proof of concept using node.

![Screen Shot 2021-04-20 at 09 56 47](https://user-images.githubusercontent.com/17026751/115368228-cbcd0000-a1be-11eb-9d17-6ada1ad5ff98.png)

## Prerequisites

* `node`
* `docker`

## Running locally

* `npm install` - installs npm dependencies.
* `docker-compose up` - starts kafka inside docker container.
* `docker exec -it kafka /opt/bitnami/kafka/bin/kafka-topics.sh \
    --create \
    --zookeeper zookeeper:2181 \
    --replication-factor 1 \
    --partitions 1 \
    --topic test` - creates kafka topic.
* `npm run start:producer` - starts producer.
* `npm run start:consumer` - starts consumer.
