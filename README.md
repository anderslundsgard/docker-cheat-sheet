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