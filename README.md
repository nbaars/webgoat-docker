# WebGoat Docker

## Introduction

Project which creates a Docker image for official release of WebGoat 7.1


## Run

The Docker image is available through Docker. You can run it with:

```
docker run -t
```


## Build


```
mvn install docker:build
```

## Publish

To publish the container to DockerHub, use the following commands:

```
docker tag webgoat/webgoat-7.1 webgoat/webgoat-7.1:7.1
docker login
docker push webgoat/webgoat-7.1

```