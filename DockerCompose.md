
# Start services
docker-compose up

# Start services in background
docker-compose up -d

# Stop and remove services
docker-compose down

# List services
docker-compose ps

# View logs
docker-compose logs

# Follow logs in real-time
docker-compose logs -f

# Build services
docker-compose build

# Restart services
docker-compose restart

# Stop services
docker-compose stop

# Start services
docker-compose start

# Execute command in service
docker-compose exec <service> <command>

# Scale services
docker-compose up -d --scale <service>=<number>

