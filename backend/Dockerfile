# Create image based on the official Node 6 image from dockerhub
FROM node:latest

# Create a directory where our app will be placed
RUN mkdir -p /usr/src/app

# Change directory so that our commands run inside this new directory
WORKDIR /usr/src/app

# Pull backend code
RUN git clone https://github.com/pbatleyGH/express-backend ##pull again

# Change directory into pulled repository containing API and package.json
WORKDIR express-backend

# Install dependecies
RUN npm install

# Expose the port the app runs in
EXPOSE 3000

# Serve the app
CMD ["npm", "start"]
