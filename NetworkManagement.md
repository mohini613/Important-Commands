# Create a network
docker network create <name>

# List all networks
docker network ls

# Inspect network details
docker network inspect <network>

# Connect container to network
docker network connect <network> <container>

# Disconnect container from network
docker network disconnect <network> <container>

# Remove a network
docker network rm <network>

# Remove unused networks
docker network prune