# Node.js runtime as the base image
FROM node:16

# Set the working directory in the container
WORKDIR /app

# Copy the package.json and package-lock.json files
COPY package.json package*.json ./

# Install the dependencies
RUN npm install

# Copy the rest of the application code
COPY . .

# Copy the lib-p3 directory from the parent directory (../lib-p3) to the container
COPY ../lib-p3 /app/lib-p3

# Specify the command to run the application
CMD [ "npm", "start" ]
