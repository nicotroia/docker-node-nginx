FROM mhart/alpine-node:latest as builder

RUN apk update && apk add bash curl

WORKDIR /node

COPY package*.json ./

RUN npm install

COPY . ./

EXPOSE ${NODE_PORT}

CMD node src/bin/www
