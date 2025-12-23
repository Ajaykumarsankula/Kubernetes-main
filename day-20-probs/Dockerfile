# Use official Node.js runtime as base image
FROM node:18-alpine

# Set working directory inside container
WORKDIR /app

# Copy package.json and package-lock.json (if exists)
COPY package*.json ./

# Install dependencies
RUN npm install --production

# Copy application source code
COPY server.js .

# Expose the port the app runs on
EXPOSE 3000

# Start the application
CMD ["node", "server.js"]
