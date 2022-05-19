# Chat-App

# Changes made
Dockerized backend using golang:alpine. Container insctructions to open port :8080 and connect to Redis server on a separate container.

Frontend also dockerized with node:alpine to work with an older version of React, as newer version do not suppor certain code elements.

All changes made to this code were mande using separate Dockerfiles for each of the modules, and built with a Docker-compose.yml file.

# NOTE:
As this a development application, and its purpose is for testing environments, it works only on localhost, each container is ponted to work on a local environment via .env file, also included.
