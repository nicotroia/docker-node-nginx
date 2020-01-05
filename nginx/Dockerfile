FROM nginx:alpine

RUN apk update && apk add bash

WORKDIR /nginx

COPY . ./

EXPOSE 80

CMD nginx -g 'daemon off;'
