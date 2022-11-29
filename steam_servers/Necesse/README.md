# Necesse

Game ID: 1169370  
Port: 14159  
Login: Anonymous  

## Variables

- ``WORLD_NAME`` - name of the world that will be created

## Start

Container solely:

```
docker container run --name NecesseServer \
-p 14159-14159:14159-14159/udp \
-v ./necesse_data:/necesse \
-e WORLD_NAME="WorldName" \
necesse_server
```

Docker Compose:

```sh
docker-compose up -d
```

## Source

https://necessewiki.com/Multiplayer-Linux
