# Use Node.js version 18.19-alpine
FROM node:18.19-alpine

# Set working directory
WORKDIR /app

# Copy package.json and package-lock.json
COPY package.json package-lock.json ./

# Install Angular CLI globally and install project dependencies
RUN npm install -g @angular/cli && npm install

# Copy the rest of the application code
COPY . .

# Expose the frontend port
EXPOSE 4200

# Start the Angular development server
CMD ["ng", "serve", "--host", "0.0.0.0"]
