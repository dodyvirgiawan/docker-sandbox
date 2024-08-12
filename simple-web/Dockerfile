# Specify a base image
## We use this version of base image that is preconfigured to has node installed
FROM node:14-alpine

# Create a new folder inside the container
WORKDIR /usr/app

# Install some deps
# Copy package json inside the working directory, copy into container
# We cache the build process so that for consequent build, it happen faster because of cached version.
COPY ./package.json ./
RUN npm install
COPY ./ ./

# Default command to run
CMD ["npm", "start"]