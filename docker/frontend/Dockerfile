# docker/frontend/Dockerfile

FROM node:carbon

WORKDIR frontend/package*.json ./
RUN npm install

ENV PATH /app/node_modules/.bin:$PATH

ADD frontend /app/src
WORKdiR /app/src
RUN npm run build
RUN npm run start

