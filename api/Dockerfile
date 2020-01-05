FROM mhart/alpine-node:latest as builder

RUN apk update && apk add bash curl

WORKDIR /api

COPY package*.json ./

RUN npm install

COPY . ./

EXPOSE 3000

CMD node src/bin/www
