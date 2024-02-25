# Use the latest Node.js version
FROM node:latest AS development

WORKDIR /app

# Install dependencies
COPY package.json package-lock.json ./
RUN npm install

# Copy your app files
COPY . .

# Expose necessary ports
EXPOSE ${PORT}

# Set up environment variables
ENV NODE_ENV=development

# Start the development server
CMD ["npm", "start"]
