# Base image
FROM node:20.14.0

# Set the working directory inside the container
WORKDIR /app

# Copy package.json and package-lock.json
COPY package.json package-lock.json ./

# Install dependencies
RUN npm install

# Copy the source code
COPY . .

# Expose the port on which the server will run
EXPOSE 3000

# Start the server
CMD ["npm", "run", "dev"]
