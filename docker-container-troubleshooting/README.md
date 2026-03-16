# Docker Container Troubleshooting

Commands used for debugging containers.

## Check running containers
docker ps

## Check container logs
docker logs web_my-nginx

## Enter running container
docker exec -it web_my-nginx bash

## Inspect container
docker inspect web_my-nginx

## Stop container
docker stop web_my-nginx
