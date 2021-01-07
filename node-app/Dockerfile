# base image - below contains npm, node
FROM node:alpine

# Any following commands will be executed here
WORKDIR /usr/app

# copy everything from this file into the container directory (/usr/app)
COPY ./package.json ./ 
RUN npm i
COPY ./ ./

# default command
CMD ["npm", "start"]
