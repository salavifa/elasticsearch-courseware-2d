# Docker Setup Exercise #

* Install using Ubuntu repositories:
```
sudo apt install docker.io -y
```
* Alternatively, by downloading from <a href="latest version from download.docker.com" target="_blank">download.docker.com</a>
* Checking that docker cli (command line interface) is installed:
```
docker --version
```
* Checking that docker daemon is running:
```
sudo docker images
```
* Expected output is an empty list:  
```
REPOSITORY          TAG                 IMAGE ID            CREATED             SIZE

```
* Running your first container:
```
sudo docker run hello-world
```
* Expected output:
```
78445dd45222: Pull complete
Digest: sha256:c5515758d4c5e1e838e9cd307f6c6a0d620b5e07e6f927b07d05f6d12a1ac8d7
Status: Downloaded newer image for hello-world:latest

Hello from Docker!
This message shows that your installation appears to be working correctly.

To generate this message, Docker took the following steps:
 1. The Docker client contacted the Docker daemon.
 2. The Docker daemon pulled the "hello-world" image from the Docker Hub.
 3. The Docker daemon created a new container from that image which runs the
    executable that produces the output you are currently reading.
 4. The Docker daemon streamed that output to the Docker client, which sent it
    to your terminal.

To try something more ambitious, you can run an Ubuntu container with:
 $ docker run -it ubuntu bash

Share images, automate workflows, and more with a free Docker ID:
 https://cloud.docker.com/

For more examples and ideas, visit:
 https://docs.docker.com/engine/userguide/
```
* List your container:
```
sudo docker ps -a
```