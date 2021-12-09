# Docker Build and Run
    docker build -t <images_name_01> ./
    docker run -p 8001:80 <images_name_01>

# Remove
    docker rm -vf $(docker ps -aq);
    docker rmi -f $(docker images -aq);
    docker volume rm $(docker volume ls -q)

# Other
    docker-compose restart 
    docker-compose up --build
    docker-compose down
    docker-compose up -d
    docker-compose --env-file .env up --build
