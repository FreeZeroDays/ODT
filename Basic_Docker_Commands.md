# Basic Docker Commands

**Description:** All stop shop for referencing Docker commands that may be useful when executing these scripts or interacting with Docker.

## Containers

Show all containers (default shows just running) \
```docker ps -a```

Stop all Docker containers \
```docker kill $(docker ps -q)```

## Cleaning Up

Remove all Docker containers \
```docker rm $(docker ps -a -q)```

Remove all Docker images \
```docker rmi $(docker images -q)```

## Persistent Data

Named volume for saving data \
```docker container run -v [LOCALDIR]:[CONTAINER LOCATION[ [CONTAINER]```
