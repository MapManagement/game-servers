# Necesse

Game ID: 1169370  
Port: 14159  
Login: Anonymous  

## Configuration

- ``WORLD_NAME`` - name of the world that will be created
- ``SLOTS`` - number of players that can play on the server
- ``PASSWORD`` - password which is needed to join the server, empty if not needed
- ``PAUSE_WHEN_EMPTY`` - pauses the server if no player is connected to it
- ``GIVE_CLIENTS_POWER`` - enables the players to adjust some settings for themselves
- ``LOGGING`` - enables logging
- ``ZIP_SAVES`` - enables zip-compressed saves
- ``MOTD`` - sets the message of the day

## Start

Container solely:

```
docker container run --name NecesseServer \
-p 14159-14159:14159-14159/udp \
-v necesse_data:/root/.config/Necesse \
--env-file env \
necesse-server
```

Docker Compose:

```sh
docker-compose up -d
```

## Source

https://necessewiki.com/Multiplayer-Linux
