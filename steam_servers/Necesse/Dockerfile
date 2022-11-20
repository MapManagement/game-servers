FROM steamcmd/steamcmd:latest
ENV WORLD_NAME=MainWorld
WORKDIR /necesse
COPY steamcmd_script.txt /necesse/steamcmd_script.txt
RUN steamcmd +runscript /necesse/steamcmd_script.txt
EXPOSE 14159-14159:14159-14159/udp
ENTRYPOINT ./StartServer-nogui.sh -world $WORLD_NAME
