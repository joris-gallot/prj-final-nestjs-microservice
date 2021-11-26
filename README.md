# Prerequisites

## Rabbitmq

Install rabbitmq with docker:

```bash
docker run -d -e RABBITMQ_DEFAULT_USER=rmq-user -e RABBITMQ_DEFAULT_PASS=rmq-pwd --hostname prj-final --name prj-final-rabbit -p 5672:5672 rabbitmq:3
```

## Autentication microservice

### Postgresql

Install Postgresql with docker:

```bash
docker run --name authentication-ms-pg -e POSTGRES_PASSWORD=pg-pwd -e POSTGRES_USER=pg-user -e POSTGRES-DB=authentication-db -p 5430:5432 -d postgres
```

## Game microservice

### Postgresql

Install Postgresql with docker:

```bash
docker run --name game-ms-pg -e POSTGRES_PASSWORD=pg-pwd -e POSTGRES_USER=pg-user -e POSTGRES-DB=game-db -p 5431:5432 -d postgres
```

## Question microservice

### Mongon

Install Mongo with docker:

```bash
docker run --name question-ms-mongo -d -e MONGO_INITDB_ROOT_USERNAME=mongo-user -e MONGO_INITDB_ROOT_PASSWORD=mongo-pwd -p 27017:27017 mongo
```
