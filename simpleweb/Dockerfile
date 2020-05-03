# Specify a base image
# Alpine does not come with nodejs
# Check supported for node: hub.docker.com
# node:alpine is a version where node works
FROM node:alpine

# Set the root work directory inside container
# ./ will be this
WORKDIR /usr/app

# Install some dependencies
# COPY {path on machine} {path inside the container}
# Avoid unnecessary re-installs by copying only the package.json before install
COPY ./package.json ./
RUN npm install
COPY ./ ./

# Default command
CMD ["npm", "start"]