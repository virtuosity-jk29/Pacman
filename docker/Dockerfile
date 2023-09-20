# FROM node:boron

# # Create app directory
# RUN mkdir -p /usr/src/app
# WORKDIR /usr/src/app

# # Clone game source code
# RUN git clone https://github.com/font/pacman.git .

# # Install app dependencies
# RUN npm install

# # Expose port 8080
# EXPOSE 8080

# # Run container
# CMD ["npm", "start"]
FROM node:boron

ENV MONGO_DB_USERNAME=admin \
    MONGO_DB_PWD=password

RUN mkdir -p /home/app

COPY ./app /home/app

# set default dir so that next commands executes in /home/app dir
WORKDIR /home/app

# will execute npm install in /home/app because of WORKDIR
RUN npm install

# no need for /home/app/server.js because of WORKDIR
CMD ["node", "start"]
