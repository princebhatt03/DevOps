# Step 1: Use official Node image
FROM node:18

# Step 2: Set working directory
WORKDIR /app

# Step 3: Copy package files and install dependencies
COPY package*.json ./
RUN npm install

# Step 4: Copy rest of the backend code
COPY . .

# Step 5: Expose port (must match server port)
EXPOSE 5000

# Step 6: Run the server
CMD ["npm", "start"]
