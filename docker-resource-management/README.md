# Docker Resource Management

This project shows how to apply CPU and memory limits on Docker containers and verify them using real-time monitoring.

---

# Why Use Resource Limits?

Prevent one container from consuming all resources

Avoid memory (OOM) and CPU issues

Protect critical services

Ensure stable performance in shared environments

**Implementation**
```
docker run -d \
  --name stress-test \
  --memory="256m" \
  --cpus="0.5" \
  progrium/stress --vm 1 --vm-bytes 300M
```
  
**validation**

```
docker ps
docker stats
docker inspect stress-test
```
![usage](Images/usage.png) 
