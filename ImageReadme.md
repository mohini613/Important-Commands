# IMAGE MANAGEMENT

# List all images
docker images

# List all images (including intermediate)
docker images -a

# List only image IDs
docker images -q

# Download image from registry
docker pull <image>

# Upload image to registry
docker push <image>

# Search Docker Hub
docker search <term>

# Build image from Dockerfile
docker build -t <name> .

# Build with specific Dockerfile
docker build -t <name> -f <file> .

# Create image from container
docker commit <container> <image>

# Remove an image
docker rmi <image>

# Force remove image
docker rmi -f <image>

# Remove unused images
docker image prune

# Remove all unused images
docker image prune -a

# Remove all images
docker rmi $(docker images -q)

# Show image history/layers
docker history <image>

# Detailed image info
docker inspect <image>

# Tag an image
docker tag <source> <target>

# Save image to tar file
docker save <image> > image.tar

# Load image from tar file
docker load < image.tar
