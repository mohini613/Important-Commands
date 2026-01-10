# Login to Docker Hub
docker login

# Login to custom registry
docker login <registry-url>

# Logout from registry
docker logout

# Tag image for registry
docker tag <image> <registry>/<repository>:<tag>

# Push to registry
docker push <registry>/<repository>:<tag>

# Pull from registry
docker pull <registry>/<repository>:<tag>
