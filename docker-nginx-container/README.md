# Docker Nginx Container

This project demonstrates running Nginx inside a Docker container.

Features:
- Custom Dockerfile
- HTML page served from container
- Docker volume mapping
- Port mapping

Commands used:

docker build -t my-nginx .

docker volume create mydata

docker run -d -p 8080:80 -v mydata:/usr/share/nginx/html --name web_my-nginx my-nginx
