FROM node:boron

RUN mkdir -p /usr/src/app
WORKDIR /usr/src/app

RUN git clone https://github.com/virtuosity-jk29/Pacman.git .

RUN npm install

EXPOSE 8080

CMD npm start
# FROM node:boron
# WORKDIR /usr/src/app
# COPY package*.json .
# RUN npm install
# COPY . .
# CMD npm start