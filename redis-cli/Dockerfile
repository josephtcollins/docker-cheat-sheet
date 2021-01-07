# use existing docker image (alpine) as a base
FROM alpine

# Download and install a dependency
RUN apk add --update redis
RUN apk add --update gcc

# What the image runs when the container starts
CMD ["redis-server"]

# docker build .
#   in the above step
#   when downloading redis, a temp container is created and it's installed there
#   then a snapshot is take of that container and saved for later
#   This kind of thing happens on every step (FROM, RUN, CMD etc...)
# docker run {id}
# 