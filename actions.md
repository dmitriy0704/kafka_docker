***Создать топик
```shell
docker compose exec [SERVICE_NAME] kafka-topics.sh --create --topic baeldung_linux --partitions 1 --replication-factor 1 --bootstrap-server kafka:9092
```

***Список топиков
```shell
docker compose exec [SERVICE_NAME] kafka-topics.sh --list --bootstrap-server kafka:9092
docker exec -it [CONTAINER_NAME] kafka-topics.sh --list --bootstrap-server kafka:9092
```

***Отправить сообщение
```shell
docker exec -it [CONTAINER_NAME] kafka-console-producer.sh --topic [TOPIC_NAME] --bootstrap-server kafka:9092
```

***Получить сообщения из топика
```shell
docker exec -it [CONTAINER_NAME] kafka-console-consumer.sh --topic [TOPIC_NAME] --bootstrap-server kafka:9092
```