# Docker Nginx Container

This project demonstrates running an Nginx web server inside a Docker container using a custom Dockerfile.

---

## Dockerfile

![dockerfile](Images/dockerfile.png)

---

## Docker Image Build

![build](Images/build.png)

---

## Access Application

![access_url](Images/access_url.png)

---

## Commands Used

```bash
docker build -t my-nginx .

docker run -d -p 8080:80 --name web_my-nginx my-nginx
