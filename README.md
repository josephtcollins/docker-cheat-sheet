# Useful docker commands

(container is busybox for all below, replace with container_id or name)

docker run busybox // run container (create + start)
docker run busybox echo hello there // commands can follow the container name
docker run -it busybox sh // run and enter root dir in shell

docker ps // list active containers
docker ps -a // list all containers in history

docker stop busybox // exit gracefully, will kill after 10 secs
docker kill busybox // kill container immediately



To make hotloader on project

docker run -p 3000:3000 -v /app/node_modules -v $(pwd):/app {container_id}
OR with docker-compose (see frontend docker-compose.yml)
docker compose up
