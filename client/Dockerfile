# Dockerfile
FROM node:lts-alpine

RUN mkdir /app
WORKDIR /app
COPY package*.json ./
RUN npm i
COPY src src
COPY public public

ENV CHOKIDAR_USEPOLLING=true
ENV WATCHPACK_POLLING=true

CMD npm start