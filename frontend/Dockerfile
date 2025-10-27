# Use an official Node.js runtime as a parent image
FROM node:20-alpine

# Set the working directory
WORKDIR /app

# Copy package.json and package-lock.json (if available)
COPY package.json ./

# Install dependencies
RUN npm install

# Copy the rest of the application files
COPY . .

# Expose the port Vite runs on
EXPOSE 5173

# The command to run the dev server will be provided by docker-compose
# CMD ["npm", "run", "dev"]
