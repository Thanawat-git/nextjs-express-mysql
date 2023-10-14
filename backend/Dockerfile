# Use an official Node.js runtime as the base image
FROM node:14

# Set the working directory in the container
WORKDIR /app

# Copy package.json and package-lock.json to the working directory
COPY package*.json ./

# Install dependencies
RUN npm install

# Copy the rest of the backend application code
COPY . .

# Expose a port (e.g., 3000) on which your Express.js app will listen
EXPOSE 3000

# Use nodemon to start your Express.js application in development mode
CMD ["npx", "nodemon", "index.js"]
