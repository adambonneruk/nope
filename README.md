# nope (using Docker)
Dockerfile and associated files used to generate a small Apache image hosting a single .html page

> **_NOTE:_** NOPE >>> "Number Of Pink Elephants"

## Background
A small page can be served from a container, using Docker + Appache + HTML + JS. The page is pink, and gives you a random number fo pink elephants every time it loads. Docker image is available on my [Docker Hub](https://hub.docker.com/repository/docker/adambonneruk/nope).

## Prerequisites / Installation
```bash
# ububtu
sudo apt update
sudo apt-get install docker
```

## Usage
```bash
# build the image
docker build -t adambonneruk/nope .

# run the image
docker run -p 8080:80 adambonneruk/nope:latest

# push image to docker hub
docker push adambonneruk/nope:latest
```

## Future Ideas
* using PHP instead to load container IP address
