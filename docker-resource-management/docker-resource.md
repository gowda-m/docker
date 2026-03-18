# Docker Resource Management (Production-Oriented)
This project demonstrates how to apply and validate resource limits (CPU & Memory) on Docker containers in a real-time environment. Proper resource control is critical in multi-container systems to ensure stability, prevent resource exhaustion, and maintain predictable performance.


----

**Real-Time Use Case**
```
In production environments, multiple containers run on the same host. Without limits:
One container can consume all memory → OOM issues
High CPU usage can degrade overall system performance
Critical services may get impacted
This project simulates and validates controlled resource allocation.
```

# Implementation

**Run Container with Limits**

```
docker run -d \
  --name stress-test \
  --memory="256m" \
  --cpus="0.5" \
  progrium/stress --vm 1 --vm-bytes 300M
```


✔ Memory limited to 256MB
✔ CPU limited to 0.5 core
✔ Stress tool used to simulate load

# Monitoring & Validation

**Check Running Container**
```
docker ps
```
![start_run](Images/start_run.png)


**Monitor Resource Usage**
```
docker stats
```
![usage](Images/usage.png) 

**Inspect Resource Limits**

![size1](Images/size1.png) 

![size2](Images/size2.png) 


**Inspect Resource Limits (Optional)**
```
docker inspect stress-test
```


**This command provides detailed**
```
Memory limits

CPU allocation

Runtime settings
```
