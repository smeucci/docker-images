## arm32v7/jenkins

Dockerfile to build a jenkins image for raspberry pi (arm32v7).

Create a container like this:

```
docker \
     run \
     -dit \
     -p 8080:8080 -p 50000:50000 \
     -v /var/run/docker.sock:/var/run/docker.sock \
     -v jenkins:/var/jenkins \
     --name container_name
     image_name 
```
