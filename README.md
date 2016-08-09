# wrk2-docker
Docker image for wrk2 using Alpine and published to DockerHub

## DockerHub
Grab the built image https://hub.docker.com/r/1vlad/wrk2-docker/

```
docker pull 1vlad/wrk2-docker
```

## How to

To use this container make sure to use the host's network or create a link
```
docker run --rm --net=host 1vlad/wrk2-docker -t1 -c1 -d90s -R50 --latency http://localhost
```

To hop inside the container
```
docker run -it --entrypoint=/bin/sh 1vlad/wrk2-docker
```
