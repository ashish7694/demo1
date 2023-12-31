# Use an official Node.js runtime as a parent image
FROM node:20

# Set the working directory in the container
WORKDIR /myapp

# Copy the app source code to the working directory
COPY . .

# Install app dependencies
RUN npm install


# Build the app
#RUN npm run build

# Expose the port the app runs on
EXPOSE 3000

# Define the command to run your app
CMD ["npm", "start"]
