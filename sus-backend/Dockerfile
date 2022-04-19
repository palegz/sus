FROM node:16

WORKDIR /usr/src/app

COPY package*.json ./

RUN npm install

RUN tsc

COPY . .

EXPOSE 8080

CMD [ "node", "build/index.js" ]
