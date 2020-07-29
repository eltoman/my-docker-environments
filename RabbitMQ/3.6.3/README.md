# Clustering RabbitMQ Docker containers

Bassed my enviroment on:
[Set up a RabbitMQ cluster on your laptop using Docker](https://oprea.rocks/blog/set-up-a-rabbitmq-cluster-on-your-laptop-using-docker/)

### running `docker-compose`

1. Create a network shared by all containers
```bash
docker network create rabbitmq-cluster
```

2. Start cluster:
```bash
docker-compose up -d
```

3. View logs for all containers
```bash
docker-compose logs -f
```

## Tools

Very useful tool for simulating message circulation in your RabbitMQ setup.

http://tryrabbitmq.com/