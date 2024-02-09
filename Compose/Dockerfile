# Use the official Node.js  LTS (Long Term Support) image
FROM node:lts

RUN apt-get update && apt-get install -y wget

WORKDIR /usr/src/app

COPY package*.json ./
# Copy package.json and package-lock.json to the working directory
RUN npm install

COPY . .

EXPOSE 3000

CMD node server.js