FROM node:12.16.1-alpine3.11

EXPOSE 8080

WORKDIR "/app"

COPY package*.json ./

RUN npm install && npm cache clean --force

COPY . .

CMD [ "node", "index.js" ]