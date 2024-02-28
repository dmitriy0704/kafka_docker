***Создать топик
```shell
docker compose exec [SERVICE_NAME] kafka-topics.sh --create --topic baeldung_linux --partitions 1 --replication-factor 1 --bootstrap-server kafka:9092


***Список топиков
```shell
docker compose exec [SERVICE_NAME] kafka-topics.sh --list --bootstrap-server kafka:9092
docker exec [CONTAINER_NAME] kafka-topics.sh --list --bootstrap-server kafka:9092