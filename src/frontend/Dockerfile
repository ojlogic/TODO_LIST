# // _____________ stage 1 ____________ // #
FROM node:17 AS build

WORKDIR /app

COPY ./todo-list/package.json ./package.json

RUN npm install

COPY ./todo-list ./

RUN npm run build


# // _____________ stage 2 ____________ // #
FROM nginx

COPY --from=build /app/dist/index.html /nginx/static/index.html
COPY --from=build /app/dist/static/css /nginx/static
COPY --from=build /app/dist/static/js /nginx/static

