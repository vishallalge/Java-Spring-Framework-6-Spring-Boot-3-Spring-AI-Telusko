
# Docker :


## What is Docker ? 

- Docker is an open-source platform that enables developers to build, package, and run applications in lightweight, portable containers that include everything the application needs to run (code, libraries, dependencies, and configuration).


## Why Docker ? 
- Docker is used because it makes applications portable, lightweight, and consistent across environments. It removes dependency issues, speeds up deployment, and allows easy scaling using containers.



## Virtualization :

- Virtualization lets you run multiple independent operating systems on a single physical machine by dividing its resources.


## Containerization : 

- Containerization is the process of packaging an application with all its dependencies, libraries, and configuration files into a single unit called a container, so it can run reliably on any environment.



## Docker Common Commands - 
```bash
docker --version                # Show Docker version
docker info                     # Display system-wide information
docker ps                       # List running containers
docker ps -a                    # List all containers (including stopped)
docker images                   # List all images
docker run hello-world          # Run a test container
docker run -it ubuntu bash      # Run container in interactive mode
docker start <container_id>     # Start an existing container
docker stop <container_id>      # Stop a running container
docker restart <container_id>   # Restart a container
docker rm <container_id>        # Remove a container
