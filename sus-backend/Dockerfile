FROM node:16

WORKDIR /app

COPY package*.json ./
COPY tsconfig.json ./
RUN ls -a

COPY src /app/src


RUN npm install

RUN npm run build


EXPOSE 8080

CMD [ "node", "build/index.js" ]
