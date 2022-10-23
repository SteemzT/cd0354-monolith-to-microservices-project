# Use NodeJS base image
FROM node:12

# Create app directory
WORKDIR /usr/src/app

# Install app dependencies by copying
# package.json and package-lock.json
COPY package*.json ./

# Install dependencies
RUN npm ci

# Bundle app source
COPY . .
EXPOSE 8080
CMD [ "npm", "run", "dev" ]