# WebGoat Docker

## Introduction

Project which creates a Docker image for official release of WebGoat 7.1


## Run

The Docker image for WebGoat 7.1 is available through DockerHub. You can run it with:

```
docker run -p 8080:8080 webgoat/webgoat-7.1
```

Browse to http://localhost:8080/WebGoat and happy hacking...


## Build

In order to create the Docker image on your local machine, use the following command:


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