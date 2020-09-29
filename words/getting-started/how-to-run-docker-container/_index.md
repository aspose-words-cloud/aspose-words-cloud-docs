---
title: "How to Run Docker Container"
type: docs
url: /getting-started/how-to-run-docker-container/
aliases: [/how-to-run-docker-container/]
description: "How to run Docker container"
weight: 100
---

The **Docker** technology is designed to automate the deployment of the applications by using lightweight containers. Developers can use a **Docker Container** to wrap up an application with all of its libraries and dependencies and deploy everything as a single package.

Aspose.Words Cloud team has published the Docker Container on [Docker Hub](https://hub.docker.com/r/aspose/words-cloud) to facilitate the Docker users. The following sections will guide you that how to run a Docker commands or write configuration in a Yaml file for Docker compose tool.

## Container configuration

### Required volumes

|Mount path in container|Description|
| :- | :- |
|/fonts|Folder with fonts, which will be used to render documents|
|/data|File storage folder|

### Parameters

|Name|Description|
| :- | :- |
|LicensePublicKey|Public key of the license|
|LicensePrivateKey|Private key of the license|
|User|Username|
|Password|Password|

If "License" parameters are omitted, the app will work in trial mode. If "User" parameter is set, each request requires "Authorization" header (JWT authentication). The URL to obtain token is "/connect/token".


### Run a Docker container using command line

You can simply run the following docker command after pulling the container from [Docker Hub](https://href.li/?https://hub.docker.com/r/aspose/words-cloud).

```JAVA
docker run   -e "LicensePublicKey=public_key" -e "LicensePrivateKey=private_key" -v "/fonts:/fonts" -v "/data:/data" aspose/words.cloud
```

### Configurations for Docker-Compose Tool

You can write the following configurations in your yaml file for Docker-Compose tool:

```JAVA
AsposeWordsCloud:
      image: aspose/words.cloud
      ports: ["8082:80"]
      volumes: [
        "./fonts:/fonts",
        "./storage:/data",
      ]
      environment:
        "User": "User"
        "Password": "Password"
        "LicensePublicKey": "yourKeyHere"
        "LicensePrivateKey": "yourKeyHere"
```
