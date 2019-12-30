# Specify a base image
FROM node:alpine

# Install some dependencies
# COPY {path on machine} {path inside the container}
COPY ./ ./
RUN npm install

# Default command
CMD ["npm", "start"]