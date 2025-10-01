## 📌 Docker Basics
| Command | Description |
|---------|-------------|
| `docker --version` | Shows the Docker version installed. |
| `docker info` | Displays system-wide information like the number of containers and images. |
| `docker login` | Logs in to a Docker registry (e.g., Docker Hub). |
| `docker logout` | Logs out from a Docker registry. |
| `docker search <image_name>` | Searches for an image on Docker Hub. |

---

## 📦 Image Management
### Docker images are templates used to create containers.
| Command | Description |
|---------|-------------|
| `docker pull <image_name>` | Pulls an image from a registry to your local machine. |
| `docker images` or `docker image ls` | Lists all locally stored images. |
| `docker build -t <tag_name> <image_name> .` | Builds an image from a Dockerfile in the current directory. |
| `docker rmi <image_id>` or `<image_name>` | Removes a specific image from local storage. |
| `docker image prune` | Removes all unused images. |
| `docker tag <CURRENT_IMAGE_NAME> <DESIRED_IMAGE_NAME>` | Create New image with desired image name. |

---

## 🚀 Container Management
### Containers are runnable instances of an image.
| Command | Description |
|---------|-------------|
| `docker run -it <image_name>` | Runs a new container. `-it` starts it interactively. |
| `docker ps` | Lists all running containers. |
| `docker ps -a` | Lists all containers, including stopped ones. |
| `docker start <container_id>` | Starts a stopped container. |
| `docker stop <container_id>` | Stops a running container gracefully. |
| `docker restart <container_id>` | Restarts a container. |
| `docker kill <container_id>` | Forcefully stops a running container.|
| `docker rm <container_id>` | Removes a specific container.|
| `docker logs <container_id>` | Fetches the logs of a container. |
| `docker exec -it <container_id> /bin/sh` | Executes a command inside a running container. This command opens a shell inside the container.|
| `docker port <container_id>` | Lists the port mappings for a container.|

---

## ⚙️ Docker Compose
### Docker Compose is used to define and run multi-container Docker applications.
| Command | Description |
|---------|-------------|
| `docker-compose up` | Builds and starts all services defined in a `docker-compose.yml` file. |
| `docker-compose down` | Stops and removes all containers, networks, and volumes created by `up`. |
| `docker-compose ps` | Lists the containers and their status. |
| `docker-compose logs` | Shows log output from all services. |

---

## 🔧 Other Useful Commands
| Command | Description |
|---------|-------------|
| `docker system prune -a` | Cleans the Docker environment by removing all containers and images. |
| `docker save <image_id> > <file_name>.tar` | Saves an image locally to a `.tar` file. |
| `docker load < <file_name>.tar.gz` | Loads an image from a `.tar` file. |

---
