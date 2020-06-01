Welcome to Docker-Command!
===================
I just tried to listed down the  various command of docker

## Docker Installation guide fo ubuntu

1. Visit the website [docker](https://docs.docker.com/engine/install/ubuntu/)

2. Go to the option Install using the convenience script and run the below two commands in your terminal
```bash
curl -fsSL https://get.docker.com -o get-docker.sh
sudo sh get-docker.sh
```
**Command**
Now check the version of docker
```bash
sudo docker version
```
Now the Docker run command let's say you want to run an image name nginx, so the run command will be
If you don't have this image locally it will download from [dockerhub](https://hub.docker.com/_/nginx)

```bash
docker run nginx
```
Show the list of all the running container 
```bash
docker ps
```
To see all the container running or not running 
```bash
docker ps -a
```
