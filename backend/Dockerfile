# Base image
FROM node:20

# Set the working directory in the container
WORKDIR /app

# Copy package.json and package-lock.json
COPY package*.json ./

# Install dependencies
RUN npm install 

# Copy the rest of the backend source code into the container
COPY . .

# Expose the port the server is running on
EXPOSE 5000

# Command to run the app using nodemon
CMD ["npm", "start"]