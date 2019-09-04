# Example lab02 - Multiple Container

## Build docker image
```bash
docker build -t example/lab02-1 -f Dockerfile-1 .
docker build -t example/lab02-2 -f Dockerfile-2 .
```

## Running and mapping port container
```bash
docker run -d -p 8888:80 example/lab02-1
docker run -d -p 9999:80 example/lab02-2
```

## Check docker container process
```bash
docker ps
```

## Stop container
```bash
docker stop CONTAINER_NAME
```