## arm32v7/jenkins

Dockerfile to build a jenkins image for raspberry pi.

Create a container like this:

```
docker \
     run \
     -p 8080:8080 -p 50000:50000 \
     -v /var/run/docker.sock:/var/run/docker.sock \
     -v jenkins:/var/jenkins_home \
     image_name 
```
