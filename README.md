
# zookeeper
## Build zookeeper

```
docker build -t zookeeper zookeeper
```

## Run zookeeper

```
docker run -d --name zookeeper zookeeper
```

# Kafka
## Build kafka
```
docker build -t kafka kafka
```

## Run zookeeper

```
docker run -d --name kafka --link zookeeper:zookeeper kafka
```

