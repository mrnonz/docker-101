# Example lab03 - Docker Network Communication

## Create network 
```bash
docker network create --driver bridge network03
```

## Running web server in network
```bash
docker run -d --network network03 --name myweb nginx:alpine
docker run -it --network network03 mrnonz/curl
```

## Testing connection between container
Inside curl's container
```bash
$ curl myweb  
```

## Check docker container process
```bash
docker ps
```

## Stop container
```bash
docker stop CONTAINER_NAME
```

---

## List docker network
```bash
docker network ls
```

## Inspect docker network
```bash
docker network inspect NETWORK_NAME
```