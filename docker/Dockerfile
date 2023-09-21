FROM node:boron

# Create app directory
RUN mkdir -p /usr/src/app
WORKDIR /usr/src/app

# Copy package.json file
RUN git clone https://github.com/virtuosity-jk29/Pacman.git .

# Install app dependencies
RUN npm install
 
# Expose port 8080
EXPOSE 8080

# Run container
CMD ["npm", "start"]