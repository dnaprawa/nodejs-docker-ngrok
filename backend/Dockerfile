FROM node:14.4.0-buster-slim

ARG NODE_ENV=production
ENV NODE_ENV $NODE_ENV

WORKDIR /app

ARG PORT=8080
ENV PORT $PORT

COPY package.json package-lock.json ./

RUN npm ci

COPY . /app

USER node

CMD [ "node", "src/server.js" ]

