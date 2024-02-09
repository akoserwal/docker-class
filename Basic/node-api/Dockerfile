# Use the official Node.js  LTS (Long Term Support) image
FROM node:lts

ARG TARGETPLATFORM
ARG TARGETARCH
ARG TARGETVARIANT

# Create and set the working directory in the container
WORKDIR /usr/src/app

# Copy package.json and package-lock.json to the working directory
COPY package*.json ./

# Install the dependencies
RUN npm install

# Copy the rest of the application code to the working directory
COPY . .

# Expose port 3000
EXPOSE 3000

# Command to run the application
CMD ["node", "index.js"]
