# Docker Projects

This repository contains practical Docker implementations covering containerization, storage, troubleshooting, and multi-container setups.

---

## Overview

The projects demonstrate:

- Running and managing containers
- Building custom Docker images
- Using volumes for persistent storage
- Debugging and troubleshooting containers
- Multi-container deployment using Docker Compose

---

## Projects Included

### 1. Nginx Container
- Basic container deployment using Nginx
- Custom HTML content served via container

---

### 2. Docker Volumes
- Persistent storage using Docker volumes
- Data retained across container restarts

---

### 3. Container Troubleshooting
- Log analysis using `docker logs`
- Container access using `docker exec`
- Inspecting configuration using `docker inspect`

---

### 4. Docker Compose (Nginx + MySQL)
- Multi-container setup using Docker Compose
- Default networking between services
- Data persistence using named volumes

---

## Prerequisites

Ensure Docker is installed and running.

Check version:

```
docker --version
docker compose version
```

---

## Common Commands

```
docker build -t <image_name> .
docker run -d -p <host_port>:<container_port> <image_name>
docker ps
docker logs <container_name>
docker exec -it <container_name> /bin/bash
docker stop <container_name>
docker rm <container_name>
docker rmi <image_name>
```

---

## Notes

- Docker Compose creates a default network for service communication
- Volumes are used for persistence and data safety
- Containers are lightweight and portable across environments

---

## Purpose

This repository is intended to showcase hands-on Docker experience for system administration and deployment use cases.
