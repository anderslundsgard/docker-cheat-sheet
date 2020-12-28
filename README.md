# docker-cheat-sheet

## List local images
```
docker images
```

## Build and tag image
Requires a **Dockerfile** in current directory.
```
docker image build -t anderslundsgard/repo:latest . 
```

## Push image to Docker Hub
```
docker image push anderslundsgard/repo:latest
```

## Remove local image
```
docker image rm anderslundsgard/repo:latest
```

## List running containers
```
docker container ls
```

## Run container
```
docker container run -d --name myapp -p 8000:8080 anderslundsgard/repo:latest
```

## Stop container
```
docker container stop myapp
```

## Start container
```
docker container start myapp
```

## Remove container
```
docker container rm myapp
```
