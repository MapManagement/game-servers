FROM steamcmd/steamcmd:latest
WORKDIR /necessse
COPY steamcmd_script.txt /necesse/steamcmd_script.txt
RUN steamcmd +runscript /necesse/steamcmd_script.txt
VOLUME /necesse
EXPOSE 14159-14159:14159-14159/udp
ENTRYPOINT ["./StartServer-nogui.sh", "-world", "ServerWorld"]
