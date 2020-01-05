FROM nginx:alpine

RUN apk update && apk add bash

ADD . /nginx

WORKDIR /nginx

COPY . ./

EXPOSE 80

CMD nginx -g 'daemon off;'
