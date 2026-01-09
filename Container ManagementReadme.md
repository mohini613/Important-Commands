to list all docker images <docker image>
to delete any image <docker rmi IMAGENAME>
if unable to dlete like container is still on then 
<docker stop containerID>
<docekr rm containerID>
<docker rmi containerID>

when container now starting 
<docker compose down > to stop
<docker compose up -d> to start

to check container status
<docker compose logs --tail-50> last 50 logs

reset everything and start fresh
<docker compose up -d>
<docker compose down -v>

check docker status fedora
<systemctl status docker>

restart docker service 
<sudo systemctl restart docker>

# Run containers
docker run <image>                    # Run a container
docker run -d <image>                 # Run in detached mode (background)
docker run -it <image>                # Run with interactive terminal
docker run --name <name> <image>      # Run with custom name
docker run -p 8080:80 <image>         # Map port (host:container)
docker run -v /host:/container <image> # Mount volume

# List containers
docker ps                             # List running containers
docker ps -a                          # List all containers (including stopped)
docker ps -q                          # List only container IDs

# Start/Stop containers
docker start <container>              # Start a stopped container
docker stop <container>               # Stop a running container
docker restart <container>            # Restart a container
docker kill <container>               # Force stop a container
docker pause <container>              # Pause a container
docker unpause <container>            # Unpause a container

# Remove containers
docker rm <container>                 # Remove a stopped container
docker rm -f <container>              # Force remove (even if running)
docker container prune                # Remove all stopped containers
docker rm $(docker ps -aq)            # Remove all containers

# Container info
docker logs <container>               # View container logs
docker logs -f <container>            # Follow logs in real-time
docker inspect <container>            # Detailed container info
docker stats                          # Live resource usage stats
docker top <container>                # Show running processes

# Execute commands in containers
docker exec <container> <command>     # Execute command in container
docker exec -it <container> bash      # Open interactive bash shell
docker attach <container>             # Attach to running container