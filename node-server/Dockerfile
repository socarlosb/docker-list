# Smaler docker image
FROM node:alpine

# Create app folder
RUN mkdir -p /app
WORKDIR /app

# Cache npm dependencies
COPY package*.json /app/

# Copy application files
COPY . /app

# Open port
EXPOSE 3000

# Start server
CMD ["npm", "start"]