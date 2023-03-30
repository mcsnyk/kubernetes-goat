FROM node:19.8-alpine
LABEL MAINTAINER="Madhu Akula" INFO="Kubernetes Goat"

WORKDIR /usr/src/app

COPY code/package*.json ./

RUN npm install \
    && apk add --no-cache curl

COPY code/* ./

EXPOSE 3000

CMD [ "npm", "start" ]
