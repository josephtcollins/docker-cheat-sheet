# Useful docker commands

(container is busybox for all below, replace with container_id or name)

docker run busybox // run container (create + start)
docker run busybox echo hello there // commands can follow the container name
docker run -it busybox sh // run and enter root dir in shell

docker ps // list active containers
docker ps -a // list all containers in history

docker stop busybox // exit gracefully, will kill after 10 secs
docker kill busybox // kill container immediately