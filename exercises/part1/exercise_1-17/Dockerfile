FROM ubuntu:latest


RUN apt-get update --fix-missing
RUN apt-get install -y curl
RUN ap-get install -y mongodb
RUN curl -sL https://deb.nodesource.com/setup_15.x | bash -
RUN apt-get install -y nodejs

WORKDIR /App

RUN npm init -y
RUN npm install --save express
RUN npm install -g nodemon

COPY ./app/app.js ./ 

CMD ["nodemon", "app.js"]
