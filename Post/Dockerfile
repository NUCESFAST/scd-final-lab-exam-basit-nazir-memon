# Use the official Node.js 14 image as the base image
FROM node:14

# Set the working directory in the container
WORKDIR /app

# Copy package.json and package-lock.json to the working directory
COPY package*.json ./

# Install dependencies
RUN npm install

# Copy the rest of the application code to the working directory
COPY . .

# Expose the port that the app runs on

# Considering Roll No + 2000 + microservice number
# 1205+2000+2 = 3207
EXPOSE 3207

# Command to run the application
CMD ["node", "index.js"]
