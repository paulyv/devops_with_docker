FROM ubuntu:18.04

COPY ./script.sh ./

RUN chmod +x ./script.sh
RUN apt-get update
RUN apt-get install curl -y

CMD ./script.sh
