FROM node:16.13.1-alpine

WORKDIR /usr/src/app

COPY . .

RUN npm i -g npm; npm i; npm run build

CMD npm start