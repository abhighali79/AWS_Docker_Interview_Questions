1. What is `Docker`?
- `Docker` is an open-source container tool which is used to automate the deployment of an application in light weight containers.

2. What is a `container`?
- A `container` is a iscolated package which holds everything to run applications or softwares.

3. What is the difference between a `Docker container` and a `virtual machine (VM)`?
- `Container`: Shares the host OS kernel and is lightweight and fast.
- `VM`: Runs its own OS and requires more resources (heavier).

4. What is a `Docker image`?
- `Docker image` is template which contains software configurations to run docker containers.

5. What is the `Dockerfile`?
- `Dockerfile` is Special text file which contains software configurations to build Docker Image.

6. How do you `build a Docker image` from a Dockerfile?
- Use the following command to build a Docker image from a Dockerfile: `docker build -t <image_name> .`

7. What is `Docker-Compose`?
- `Docker-Compose` is a tool used to run multiple containers as a single service.

8. What is the purpose of the `docker run` command?
- The docker run command is used to create and start a new container from a specified image. Example: `docker run -d -p 8000:80 nginx`

9. What is `Docker Hub`?
- `Docker Hub` is a cloud-based registry service where you can find and share Docker images.

10. What is the difference between `docker pull` and `docker push`?
- `docker pull`: Downloads an image from a registry (e.g., Docker Hub).
- `docker push`: Uploads an image to a registry.

11. What is `Docker networking`?
- `Docker networking` allows containers to communicate with each other and the external world.

12. What is `Docker Swarm`?
- Docker Swarm is `Docker’s native orchestration tool` that allows you to manage a cluster of Docker engines (hosts) as a single virtual host. It handles tasks like scaling and load balancing.

13. How do you `list all Docker containers`?
- Use the following command: `docker ps` or `docker ps -a`

14. What is the purpose of `docker volume`?
- Docker volumes are used to `persist data` outside of the container. They can be shared between containers, allowing data to persist even if the container is removed or recreated.

15. What are `Docker tags`?
- A `Docker tag` is a label assigned to a specific version of an image (e.g., nginx:1.19). Tags allow you to manage different versions of an image.

16. What is the purpose of `docker logs`?
- The docker logs command is used to view the logs from a running or stopped container. Example: `docker logs <container_name>`

17. What is a `Docker registry`?
- A Docker registry is a repository which containes predefined docker images.
