FROM node:14.11-buster-slim

RUN apt-get update

ENV APP_ROOT /src

WORKDIR ${APP_ROOT}
COPY . ${APP_ROOT}

RUN npm ci
RUN npm run build

ENV HOST 0.0.0.0
