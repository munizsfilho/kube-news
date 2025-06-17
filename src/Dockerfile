FROM node:lts-slim AS builder
LABEL maintainer="Muniz Filho <muniz.filho@gmail.com>"
LABEL description="Kube News - A simple news aggregator for Kubernetes and Cloud Native news."
WORKDIR /app
COPY package*.json .
RUN npm install
COPY . .
EXPOSE 8080
CMD [ "node", "server.js" ]