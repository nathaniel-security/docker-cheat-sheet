# Docker cheat sheet


## Build docker image

```
docker build -t myimage:1.0
```

## List docker Image
```
docker image ls
```

## Delete docker image
```
docker image rm alpine:3.4
```


## Pull an image from a registry 

```
docker pull myimage:1.0 
```
## Retag a local image with a new image name and tag
```
docker tag myimage:1.0 myrepo/myimage:2.0 
```
## Push an image to a registry 
```
docker push myrepo/myimage:2.0 
```

## Run a container
```
docker container run --name web -p 5000:80  alpine:3.9
```
## Stop a running container
```
docker container stop web
```
## Kill a running container

```
docker container kill web
```

## List container 
```
docker container ls
```
## Docker networks

```
docker network ls 
```
## DANGER: Delete all running and stopped containers 

```
docker container rm -f $(docker ps -aq)
```




