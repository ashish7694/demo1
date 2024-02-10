# Use an official Node.js runtime as a parent image
FROM node:20

# Set the working directory in the container
WORKDIR /myapp/frontend



# Copy the app source code to the working directory
COPY . ./

# Install app dependencies
RUN npm install


# Install nano
RUN apt-get update && \
    apt-get install -y nano && \
    rm -rf /var/lib/apt/lists/*

# Build the app
#RUN npm run build
#VOLUME /myapp/data


# Expose the port the app runs on
EXPOSE 3000

# Define the command to run your app
CMD ["npm", "start"]
