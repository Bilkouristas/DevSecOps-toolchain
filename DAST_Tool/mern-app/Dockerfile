#  Dockerfile for Node Express Backend api (development)

FROM node:14.15.1-alpine

# ARG NODE_ENV=development

# Create App Directory
RUN mkdir -p /usr/src/app
WORKDIR /usr/src/app

# Install Dependencies
COPY package*.json ./

RUN npm i

# Copy app source code
COPY . .

# Exports
EXPOSE 3001

CMD ["npm","start"]