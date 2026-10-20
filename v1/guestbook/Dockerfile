# Use official Node.js runtime as parent image
FROM node:18-alpine

# Set the working directory in the container
WORKDIR /app

# Copy package.json and package-lock.json
COPY package*.json ./

# Install application dependencies
RUN npm install --only=production

# Copy all project files into the working directory
COPY . .

# Expose port 3000 to allow traffic to the container
EXPOSE 3000

# Command to run the application
CMD ["npm", "start"]
