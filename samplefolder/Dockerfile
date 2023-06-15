# Use an official Node.js runtime as the base image
FROM node:14

# Set the working directory in the container
WORKDIR /app

# Copy package.json and package-lock.json to the working directory
COPY package*.json ./

# Install application dependencies
RUN npm install

# Copy the entire application to the working directory
COPY . .

# Expose the port that the application listens on
EXPOSE 3000

# Define the command to run the application
CMD [ "npm", "start" ]