# Use an official Node.js runtime as the base image
FROM node:14

# Set the working directory in the container
WORKDIR /usr/src/app

# Copy package.json and package-lock.json to the working directory
COPY package*.json ./

# Install the dependencies
RUN npm install

# Copy the application source code to the working directory
COPY . .

# Copy the index.html file to a public directory
COPY index.html public/

# Expose a port for the application to listen on (if necessary)
EXPOSE 3000

# Specify the command to run when the container starts
CMD [ "npm", "start" ]
