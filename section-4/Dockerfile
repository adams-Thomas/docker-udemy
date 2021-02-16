# Alpine is a basic linux image for docker containers. node:alpine stands for an alpine image with Node installed
FROM node:alpine

WORKDIR /usr/app

# Only copy package.json so that when changes are made to Index.js the dependencies don't get reinstalled
COPY ./package.json ./
RUN npm install

# This copy then brings across everything else
COPY ./ ./

CMD ["npm", "start"]