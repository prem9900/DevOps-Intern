# Use the official Node.js version 18 image based on Alpine Linux (lightweight and fast)
FROM node:18-alpine

# Set environment variables used in the application
ENV DOMAIN="http://localhost:3000" \
    PORT=3000 \
    STATIC_DIR="./client" 

    

# Set the working directory inside the container
WORKDIR /usr/src/app

# Copy package.json and package-lock.json for installing dependencies
COPY package*.json ./

# Install project dependencies inside the container
RUN npm install

# Copy the rest of the application source code into the container
COPY . .

# Inform Docker that the app will run on port 3000
EXPOSE 3000

# Start the Node.js server by running server.js
CMD ["node", "server.js"]
