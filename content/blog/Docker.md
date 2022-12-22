---

description: Initial description.

author: "@Luigi"
---

- docker -v
- docker pull mongo (from docker hub)
- docker images | grep mongo
- docker run -p 27017:27107 mongo
- From another terminal run
	- mongo
- docker ps
- docker kill xxxx
-
- docker build -t hello-docker .
- docker run -dp 3000:3000 hello-docker
-
-
- Notes from https://dev.to/alexeagleson/docker-for-javascript-developers-41me
-
- With Docker you put a file called Dockerfile in a project so the project and its environment is packaged to be used altogether.
- Docker containers are hosted in DockerHub
- docker pull hello-world
- docker run hello-world (this runs this container that finishes very quickly)
- docker image -ls (you get the images existing, hello-world, etc)
- docker container -ls (the list of containers running, currently none)