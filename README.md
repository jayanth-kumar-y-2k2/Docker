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

### Executing Commands in a Running Container
- **Command:** `docker exec`
  - **Usage:** `docker exec -it container_id_or_name bash`
  - **Description:** Executes a command in a running container. The `-it` option allows interaction with the container.

### Inspecting Docker Objects
- **Command:** `docker inspect`
  - **Usage:** `docker inspect container_id_or_name`
  - **Description:** Returns low-level information on Docker objects.

### Managing Docker Networks
- **Command:** `docker network ls`
  - **Usage:** `docker network ls`
  - **Description:** Lists all Docker networks.

### Managing Docker Volumes
- **Command:** `docker volume ls`
  - **Usage:** `docker volume ls`
  - **Description:** Lists all Docker volumes.

- **Command:** `docker volume create`
  - **Usage:** `docker volume create my-volume`
  - **Description:** Creates a new Docker volume.

- **Command:** `docker network create`
  - **Usage:** `docker network create my-network`
  - **Description:** Creates a new Docker network.

### Docker Registry Interactions
- **Command:** `docker pull`
  - **Usage:** `docker pull nginx`
  - **Description:** Pulls an image or a repository from a Docker registry.

- **Command:** `docker push`
  - **Usage:** `docker push my-image`
  - **Description:** Pushes an image or a repository to a Docker registry.

- **Command:** `docker tag`
  - **Usage:** `docker tag my-image myrepo/my-image:tag`
  - **Description:** Tags an image into a repository.

- **Command:** `docker login`
  - **Usage:** `docker login`
  - **Description:** Logs into a Docker registry.
