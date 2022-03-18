FROM node:17.7.1-slim
LABEL MAINTAINER "Madhu Akula" INFO="Kubernetes Goat"

WORKDIR /app

COPY code .

RUN apt update && apt install wget iputils-ping -y \
    && npm install

EXPOSE 80

CMD ["npm", "start"]
