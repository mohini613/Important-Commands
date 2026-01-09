#Image Management
# List images

docker images                        
 # List all images

docker images -a                     
 # List all images (including intermediate)

docker images -q                      
# List only image IDs
***********************************
# Pull/Push images

docker pull <image>                   
# Download image from registry

docker push <image>                   
# Upload image to registry

docker search <term>                  
# Search Docker Hub
********************************
# Build images

docker build -t <name> .              
# Build image from Dockerfile

docker build -t <name> -f <file> .    
# Build with specific Dockerfile

docker commit <container> <image>    
 # Create image from container
**************************************
# Remove images

docker rmi <image>                   
 # Remove an image

docker rmi -f <image>                
 # Force remove image

docker image prune                  
  # Remove unused images

docker image prune -a                
 # Remove all unused images

docker rmi $(docker images -q)       
 # Remove all images
****************************************
# Image info

docker history <image>            
# Show image history/layers

docker inspect <image>               
 # Detailed image info

docker tag <source> <target>       
   # Tag an image

