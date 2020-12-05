#Base Image (MMT require node 14.15.1)
FROM node:14.15.1

#Set working directory
RUN mkdir /usr/src/app

#Copy files from current directory to Docker
COPY . /usr/src/app
WORKDIR /usr/src/app

#Set environment variable path
ENV PATH /usr/src/app/node_modules/.bin:$PATH

#Install and cache app dependencies
RUN yarn

#Start app
CMD [ "npm", "start" ]
