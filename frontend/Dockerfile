# Create image based on the official Node 6 image from dockerhub
FROM node:latest

# Create a directory where our app will be placed
RUN mkdir -p /usr/src/app

# Change directory so that our commands run inside this new directory
WORKDIR /usr/src/app

# Git pull step
RUN git clone https://github.com/pbatleyGH/sweet-frontend #repull

# Change directory into pulled repo containing app and package.json file
WORKDIR sweet-frontend

# Install dependecies
RUN npm install

# Expose the port the app runs in
EXPOSE 4200

# Serve the app
CMD ["npm", "start"]
