FROM node:22.8.0-alpine3.20
LABEL MAINTAINER="Madhu Akula" INFO="Kubernetes Goat"

WORKDIR /usr/src/app

COPY code/package*.json ./

RUN npm install \
    && apk add --no-cache curl

COPY code/* ./

EXPOSE 3000

CMD [ "npm", "start" ]
