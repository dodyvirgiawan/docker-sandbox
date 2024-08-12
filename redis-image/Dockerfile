# Use an existing docker image as a base image to run on
# Alpine Image -> Docker Image based on Alpine Linux with complete package index.
FROM alpine

# Download and install a dependency
# 1. Will create a temporary image (FROM ALPINE)
# 2. And execute this command below specified in RUN
RUN apk add --update redis

# Tell the image what to do when it starts as a container
CMD ["redis-server"]