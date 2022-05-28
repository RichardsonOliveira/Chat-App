# Chat-App

# Change log
Dockerized backend creating a Dockerfile for its components and building the application using golang:alpine. Container insctructions to open port :8080 and connect to Redis server on a separate container.

Frontend also dockerized with node:alpine to work with an older version of React, as newer version do not supports certain code elements.

All changes made to this code were mande using separate Dockerfiles for each of the modules, and built with a Docker-compose.yml file.

# NOTE:
As this a test application, and its purpose is for testing environment and practice, it works only on localhost, each container is ponted to work on a local environment via .env file, also included.


# Requirements

To Run this application, you need:

Docker

For Windows or WSL:

https://docs.docker.com/desktop/windows/install/

For Linux:

https://docs.docker.com/desktop/linux/install/

Git

On your terminal, Install Git:

```bash
$ sudo apt install git
```

# Usage

Clone the repository:
```bash
$ git clone https://github.com/RichardsonOliveira/Chat-App.git
````

Go to App Folder:
```bash
$ cd Chat-App
```

To run the app:

```bash
$ docker-compose up
```

Check if all containers are up:
```bash
$ docker ps -a
```
If all containers are up, type localhost:3000 on your browser.
