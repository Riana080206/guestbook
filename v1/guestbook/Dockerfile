# Use the official Node.js image as the base
FROM node:18-alpine

# Set working directory inside the container
WORKDIR /app

# Copy package management files and install dependencies
COPY package*.json ./
RUN npm install --only=production

# Copy all application code into the container
COPY . .

# Expose port 3000 for the Guestbook application
EXPOSE 3000

# Start the application
CMD ["npm", "start"]
