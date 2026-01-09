# CONTAINER MANAGEMENT

# Run a container
docker run <image>

# Run in detached mode (background)
docker run -d <image>

# Run with interactive terminal
docker run -it <image>

# Run with custom name
docker run --name <name> <image>

# Map port (host:container)
docker run -p 8080:80 <image>

# Mount volume
docker run -v /host:/container <image>

# List running containers
docker ps

# List all containers (including stopped)
docker ps -a

# List only container IDs
docker ps -q

# Start a stopped container
docker start <container>

# Stop a running container
docker stop <container>

# Restart a container
docker restart <container>

# Force stop a container
docker kill <container>

# Pause a container
docker pause <container>

# Unpause a container
docker unpause <container>

# Remove a stopped container
docker rm <container>

# Force remove container (even if running)
docker rm -f <container>

# Remove all stopped containers
docker container prune

# Remove all containers
docker rm $(docker ps -aq)

# View container logs
docker logs <container>

# Follow logs in real-time
docker logs -f <container>

# Detailed container info
docker inspect <container>

# Live resource usage stats
docker stats

# Show running processes in container
docker top <container>

# Execute command in container
docker exec <container> <command>

# Open interactive bash shell in container
docker exec -it <container> bash

# Attach to running container
docker attach <container>

# Copy files from container to host
docker cp <container>:/path/file.txt ./file.txt

# Copy files from host to container
docker cp ./file.txt <container>:/path/file.txt

# Export container to tar file
docker export <container> > backup.tar

# Import container from tar file
docker import backup.tar <image_name>

# Stop and remove all containers
docker stop $(docker ps -aq) && docker rm $(docker ps -aq)