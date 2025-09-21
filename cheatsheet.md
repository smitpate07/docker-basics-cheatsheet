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
| Command | Description |
|---------|-------------|
| `docker pull <image_name>` | Pulls an image from a registry to your local machine. |
| `docker images` or `docker image ls` | Lists all locally stored images. |
| `docker build -t <tag_name> <image_name> .` | Builds an image from a Dockerfile in the current directory. |
| `docker rmi <image_id>` or `<image_name>` | Removes a specific image from local storage. |
| `docker image prune` | Removes all unused images. |

---

## 🚀 Container Management
| Command | Description |
|---------|-------------|
| `docker run -it <image_name>` | Runs a new container. `-it` starts it interactively. |
| `docker ps` | Lists all running containers. |
| `docker ps -a` | Lists all containers, including stopped ones. |
| `docker start <container_id>` | Starts a stopped container. |
| `docker stop <container_id>` | Stops a running container gracefully. |

---

## ⚙️ Docker Compose
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
