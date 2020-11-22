FROM node:10.23.0-alpine3.10
WORKDIR /app
ADD package*.json ./
RUN npm install
ADD . .
CMD node index.js