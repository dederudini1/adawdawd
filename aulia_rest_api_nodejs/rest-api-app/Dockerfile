FROM node:14

ADD ./database/data.sql /docker-entrypoint-initdb.d

WORKDIR /rest-api-app
COPY package.json .
RUN npm install
COPY . .
CMD npm start
