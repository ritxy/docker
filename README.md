# Docker

## List of docker commands
docker build . -> Create an image using the Dockerfile in the current directory

docker ps -> List all the running containers
docker ps -a -> List all the containers
docker stop container_name -> Stop a container

docker run -p 3000:80 2ddf2ede7d6c -> Run image in a container and use the port 3000 in the machine that is 80 in the image in attached mode
docker run -p 3000:80 -d 2ddf2ede7d6c -> Run image in a container and use the port 3000 in the machine that is 80 in the image in dettached mode
docker start image_name -> Start a container with the image selected, the container is running in the background
docker start -a image_name -> Start a container in attached mode
docker attach name_container -> Put a container in attached mode

docker logs contaniner_name -> See the logs of a container
docker logs -f container_name -> Put the container in attached mode and see the future logs

docker run -it image_name -> Run an image in an interctive mode, a console will be ready fro your inputs
docker start -ai container_name -> Start a container in an interactive mode, let you input things if your image have an input paramenters

docker rm container_name container_name2 -> Remove the container in the list of parameters
docker prune -> Remove all containers

docker images -> List all images
docker rmi image_name -> Remove an image, only can remove if is not be using by a container that must be stopped and must be removed first
docker image prune -> Remove all images that are not be using
