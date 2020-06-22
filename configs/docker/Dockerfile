FROM ubuntu:18.10

# copy and configuration of interscity-dana project
COPY ./dana ./home/marciopsa/dana 
COPY ./interscity_dana_project ./home/marciopsa/interscity_dana_project
COPY start.sh /home/marciopsa/interscity_dana_project/pal/start.sh
COPY assembly.sh /home/marciopsa/interscity_dana_project/pal/assembly.sh
ENV DANA_HOME=/home/marciopsa/dana/
ENV PATH="${PATH}:/home/marciopsa/dana/"
WORKDIR /home/marciopsa/interscity_dana_project/pal/

ENTRYPOINT ["/bin/bash", "./assembly.sh"]
