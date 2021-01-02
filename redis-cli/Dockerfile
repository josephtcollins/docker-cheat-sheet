# use existing docker image as a base
FROM alpine

# Download and install a dependency
RUN apk add --update redis

# Tell the image what to do when it starts i.e. run this command
CMD ["redis-server"]

# docker build .
# docker run {id}