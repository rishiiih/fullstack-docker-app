# Use Node.js base image
FROM node:14-alpine

# Set working directory inside container
WORKDIR /app

# Copy package.json first (for better build caching)
COPY package.json ./

# Install dependencies
RUN npm install

# Copy rest of the backend files
COPY . .

# Expose backend port
EXPOSE 5000

# Start backend
CMD ["npm", "start"]
