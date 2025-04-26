# 1. Use Node.js 14 base image
FROM node:14

# 2. Set the working directory inside the container
WORKDIR /app

# 3. Copy package.json and package-lock.json first
COPY package*.json ./

# 4. Install dependencies
RUN npm install

# 5. Copy the rest of the application code
COPY . .

# 6. Expose a port (optional, e.g., if your app runs on 3000)
EXPOSE 3000

# 7. Start the application
CMD ["npm", "start"]
