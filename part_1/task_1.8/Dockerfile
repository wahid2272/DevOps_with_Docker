FROM ubuntu:20.04

RUN apt-get update; apt-get install -y curl;

WORKDIR /usr/src/path

COPY index.sh .

CMD ./index.sh