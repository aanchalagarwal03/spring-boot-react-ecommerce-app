# Base Package
FROM node:14

MAINTAINER Ujjaval Desai

# Create app directory
WORKDIR /usr/src/app

# Install app dependencies
# A wildcard is used to ensure both package.json AND package-lock.json are copied
# where available (npm@5+)
 COPY ./client/package*.json ./
# COPY package*.json ./

RUN npm install
#run npm install -g npm

# Bundle app source
COPY . .

#RUN yarn install

#Aanchal change
EXPOSE 80

# Initiate npm start
CMD [ "npm", "run-script", "start_docker_dev" ]
