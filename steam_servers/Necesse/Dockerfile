FROM steamcmd/steamcmd:latest
WORKDIR /dst
COPY steamcmd_script.txt /dst/steamcmd_script.txt
RUN steamcmd +runscript /dst/steamcmd_script.txt
VOLUME /dst
EXPOSE 14159/udp
EXPOSE 14159/tcp
ENTRYPOINT ["./StartServer-nogui.sh", "-world", "ServerWorld"]
