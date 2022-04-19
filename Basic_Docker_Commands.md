# Basic Docker Commands

**Description:** All stop shop for referencing Docker commands that may be useful when executing these scripts or interacting with Docker.

## Containers

Show all containers (default shows just running) \
```bash
docker ps -a
```

Stop all Docker containers \
```bash
docker kill $(docker ps -q)
```

## Cleaning Up

Remove all Docker containers \
```bash
docker rm $(docker ps -a -q)
```

Remove all Docker images \
```bash
docker rmi $(docker images -q)
```

## Persistent Data

Named volume for saving data \
```bash
docker container run -v [LOCALDIR]:[CONTAINER LOCATION[ [CONTAINER]
```

Copy data locally \
```bash
docker cp [CONTAINERNAME]:/PATH] [LOCAL]
```
