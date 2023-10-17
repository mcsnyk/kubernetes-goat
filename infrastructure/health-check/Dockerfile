FROM node:20.8-bookworm-slim
LABEL MAINTAINER "Madhu Akula" INFO="Kubernetes Goat"

WORKDIR /app

COPY code .

RUN apt update && apt install wget iputils-ping -y \
    && npm install

EXPOSE 80

CMD ["npm", "start"]
