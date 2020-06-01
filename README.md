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
##Command

1. Now check the version of docker
```bash
sudo docker version
```
2.Now the Docker run command let's say you want to run an image name nginx, so the run command will be

```bash
docker run nginx
```
If you don't have this image locally it will download from [dockerhub](https://hub.docker.com/_/nginx)

3. Show the list of all the running container 
```bash
docker ps
```
4. To see all the container running or not running 
```bash
docker ps -a
```
