# Docker

## Docker Commands

  To get the running containers
  
    docker ps

  To get the list of all containers including stopped ones

    docker ps -a

  To list the images

    docker images

  To pull an image or registry from the dockerhub

    docker pull <name>:<version>
      Ex: docker pull nginx:1.23

  To create a container from an image

    docker run <image-name>:<version>
      Ex: docker run nginx:1.23

  To run the container in detached mode

    docker run -d <image>:<version>
      Ex: docker run -d nginx:1.23

  To get the logs from a container

    docker logs <container_name_or_id>

  To stop a container

    docker stop <container_name_or_id>

  To start a container

    docker start <container_name_or_id>

  To restart a running container

    docker restart <container_name_or_id>

  To remove a container

    docker rm <container_name_or_id>

  To remove an image from a container

    docker rmi <image_id_or_name>

  To port bind a container while creation

    docker run -d -p 9000:80 nginx:1.23

  To port bind a container while creation with a name

    docker run --name web-app -d -p 80:80 nginx:1.23

    