FROM node:alpine

WORKDIR /app

COPY client/package.json package.json
COPY client/yarn.lock yarn.lock

RUN yarn install

COPY client/ .

ENV CI=true

RUN yarn test
