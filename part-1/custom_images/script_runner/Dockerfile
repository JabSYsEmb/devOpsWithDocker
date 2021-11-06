FROM ubuntu:18.04

WORKDIR /home/bin

COPY ./script.sh /home/bin/

RUN chmod +x script.sh

RUN apt-get update

RUN apt-get install -y curl

CMD ./script.sh
