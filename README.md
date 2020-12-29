# docker-cheat-sheet

*Container: Isolated area of an OS with resource usage limits applied.*

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

## Run container detached
```
docker container run -d --name myapp -p 8000:8080 anderslundsgard/repo:latest
```
*-d* = *Detached, runs in background. Typical option for web server etc.*

## Run container interactive
```
docker container run -it --name testit alpine sh
```
*-it* = *Interactive, step into container*
*Tip: Exit from container but leave it running with \<Ctrl\> + P + Q*

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
