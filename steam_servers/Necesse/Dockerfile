FROM steamcmd/steamcmd:latest

ENV WORLD_NAME=MainWorld
ENV SLOTS = 10
ENV PASSWORD = ""
ENV PAUSE_WHEN_EMPTY = 1
ENV GIVE_CLIENTS_POWER = 1
ENV LOGGING = 1
ENV ZIP_SAVES = 1
ENV MOTD = "Awesome Necesse Server"

WORKDIR /necesse
VOLUME ~/.config/Necesse

COPY steamcmd_script.txt /necesse/steamcmd_script.txt
RUN steamcmd +runscript /necesse/steamcmd_script.txt

EXPOSE 14159-14159:14159-14159/udp

ENTRYPOINT ./jre/bin/java -jar Server.jar \
        -nogui \
        -world ${WORLD_NAME} \
        -slots ${SLOTS} \
        -password ${PASSWORD} \
        -pausewhenempty ${PAUSE_WHEN_EMPTY} \
        -giveclientspower ${GIVE_CLIENTS_POWER} \
        -logging ${LOGGING} \
        -zipsave ${ZIP_SAVES} \
        -motd ${MOTD}
~
