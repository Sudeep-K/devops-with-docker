FROM ubuntu:22.04

WORKDIR /usr/src/app

COPY script.sh .

RUN apt -y update

RUN apt install -y curl 

RUN chmod 777 ./script.sh

CMD ./script.sh
