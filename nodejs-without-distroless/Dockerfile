FROM node:18-alpine
# set working  directory
WORKDIR /app

# COPY all package.json and install dependencies
COPY package.json* ./
RUN npm install --production

# Copy the rest of app
COPY . .

# EXPOSE port 3000
EXPOSE 3000

# start app
CMD ["npm", "start"]