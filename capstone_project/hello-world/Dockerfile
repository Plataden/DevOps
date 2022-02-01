FROM node:16.13.1-alpine AS build

EXPOSE 3000

WORKDIR /tmp/build

COPY . .

RUN npm i -g npm; npm i; npm run build

FROM nginx AS final

WORKDIR /usr/share/nginx/html

COPY --from=build /tmp/build/build .