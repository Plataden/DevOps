FROM node:16.13.1-alpine

WORKDIR /usr/src/app

COPY . .

RUN npm i -g npm; npm i; npm run build

CMD npm start

# FROM nginx AS final

# WORKDIR /usr/share/nginx/html

# COPY --from=build /tmp/build/build .