## List Docker CLI commands
docker
docker container --help

## Display Docker version and info
docker --version
docker version
docker info

## Excecute Docker image
docker run hello-world

## List Docker images
docker image ls

## Docker containers
docker container ls
docker container ls -all
docker container ls -a -q
docker ps -a : List all containers docker ps : list all running containers
docker stop $(docker ps -a -q) :  stop all running containers docker
rm $(docker ps -a -q) : remove all running containers docker
rm container_name : remove a container

# Mapping your machine’s port 4000 to the container’s published port 80 using -p
docker run -p 4000:80 <image_name>
# Run app(image) in background with detached mode
docker run -d -p 4000:80 <image/app>
