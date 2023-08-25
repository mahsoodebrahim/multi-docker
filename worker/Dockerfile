FROM node:16-alpine as builder
# Use an official Node.js runtime as the base image
FROM node:14.14.0-alpine

# Set the working directory inside the container
WORKDIR /app

# Copy package.json and package-lock.json to the working directory
COPY ./package*.json ./

# Install app dependencies
RUN npm install

# Copy the rest of the application code
COPY ./ ./

# Define the command to run your application
CMD ["npm", "run", "start"]