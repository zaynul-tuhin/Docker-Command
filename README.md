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
**Add user on docker group and reboot your OS**
```bash
 sudo gpasswd -a user_name docker
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
To stop the running container use below command
```bash
docker stop container name/ container id 
docker stop 50f6*****( lets say nginx id is 50f6*****)
```
We want to remove a container
```bash
docker rm container name/ container id 
docker rm 50f6*****( lets say nginx id is 50f6*****)
```
List of docker images

```bash
docker images
```

Now let's as you are not using image "nginx" any more so want to remove the downloaded file as well

```bash
docker rmi container name
```
docker run command download image and run that image but let's say you want to just download the image
```bash
docker pull image name  //if the image name is nginx then use then it would be 
docker pull nginx

```
Let's say we have an aplication name simple_webapp and we need to run it pamenantly in that case we need to run in detach mode
```bash
docker run -d application_name(here it will be simple_webapp)
```
