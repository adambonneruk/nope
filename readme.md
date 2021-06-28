# "Number of Pink Elephants": Apache using Docker
"Number of Pink Elephants"/"NOPE" is a small example Dockerfile project designed to teach (and serve as my own reference for) building, running and hosting Dockerfile images on Github and Docker Hub). Leveraging the publically-maintained httpd image and inserting some .html code, this project documents the process here while being publically available for others to utilise and/or fork.

> The "NOPE" container image/dockerfile project is available on my [Docker Hub](https://hub.docker.com/repository/docker/adambonneruk/nope).


TBC

---
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
docker build -t nope .

# run the image
docker run -p 8080:80 nope:latest

```

### Usage (Docker.io)
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
