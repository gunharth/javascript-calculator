# Use an official Node.js runtime as a parent image 
FROM node:lts-buster-slim

# Set the working directory
WORKDIR /usr/src/app

# Copy package.json and package-lock.json
COPY package.json package-lock.json ./

# Install dependencies
RUN npm ci

# Copy the rest of the application code
COPY . .

# Expose the port the app runs on
EXPOSE 3001

# The default command is to serve the API
CMD ["npm", "run", "start"]
