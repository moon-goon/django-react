FROM node:14.4.0-alpine3.10

WORKDIR /app/frontend

COPY package*.json /app/frontend/
RUN npm i
COPY . /app/frontend
RUN npm run build
EXPOSE 3000