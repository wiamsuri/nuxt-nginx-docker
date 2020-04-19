FROM node:10.20

ENV APP_ROOT /src

RUN mkdir ${APP_ROOT}
WORKDIR ${APP_ROOT}
ADD . ${APP_ROOT}

RUN npm ci
RUN npm run build

ENV HOST 0.0.0.0
