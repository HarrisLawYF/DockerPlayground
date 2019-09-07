FROM node:9-slim
# WORKDIR specifies the directory our
# application's code will live within
WORKDIR /app
# We copy our package.json file to our
# app directory
COPY package.json /app
# We then run npm install to install
# express for our application
RUN npm install
# We then copy the rest of our application
# to the app direcoty
COPY . /app
# We start our application by calling
# npm start.
CMD ["npm", "start"]


#Note: Docker automatically caches the results of each individual command so that they don’t have to be fully run each time you wish to build a Docker image