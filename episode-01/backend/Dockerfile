# Use an appropriate Node.js base image
FROM node:18

# Set the working directory inside the container
WORKDIR /app

# Copy package.json and package-lock.json
COPY package.json package-lock.json ./ 

# Install dependencies
RUN npm install

# Copy all files to the working directory
COPY . .

# Set the working directory to the src directory
WORKDIR /app/src

# Expose the port your app runs on
EXPOSE 8000

# Define the startup command
CMD ["node", "server.js"]
