#I'am using official node image as a base image
FROM node:22

# Set the working directory inside the container
WORKDIR /usr/src/app

# Copy the required fles, package.json and package-lock.json
COPY package*.json ./

# Install dependencies mentioned in the package.json
RUN npm install

# Copy app source code
COPY . .

# Expose port
EXPOSE 8080

# Run the app
CMD ["node", "index.js"]

