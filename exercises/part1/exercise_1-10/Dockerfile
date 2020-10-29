FROM node:10-alpine

WORKDIR /app

ADD ./frontend-example-docker-master ./

RUN npm install && npm run build

CMD ["npm", "start"]
