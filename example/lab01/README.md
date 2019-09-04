# Example lab01 - Single Container

## Build docker image
```bash
docker build -t example/lab01 .
```

## Running container
```bash
docker run -d example/lab01
```

## Check docker container process
```bash
docker ps
```

## Stop container
```bash
docker stop CONTAINER_NAME
```

## Running and mapping port container
```bash
docker run -d -p 8888:80 example/lab01
```