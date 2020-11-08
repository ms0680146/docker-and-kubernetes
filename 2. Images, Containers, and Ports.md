## Images, Containers, and Ports
### Images & Containers
Docker Image:  
1. Image is a template for creating an environment for your choice.
2. Snapshot.
3. Has eveythong you need to run your app, including OS, software, code.

Docker Container:
1. Running Instance of an image.

### Pulling NGINX Image
You can go to [docker hub](https://hub.docker.com/) to pull image. 
```cmd
docker pull nginx
docker images
```

### Running Containers
```cmd
# run nginx image as a brand new container
docker run nignx:latest

# see what container run
docker container ls == docker ps

# run container in background
docker container run -d nginx:latest

# stop container
docker stop {containerId}
```

###  Exposing Ports
Mapping localhost 8080 port to container 80 port.  
![](https://i.imgur.com/5UJEHNd.png)
```cmd
docker container run -d -p 8080:80  nginx:latest
```

### Exposing Multiple Ports
Mapping localhost 8080 and 3000 to container 80 port. 
![](https://i.imgur.com/46Hg1vI.png)
```cmd
docker container run -d -p 8080:80 -p 3000:80 nginx:latest
```

### Managing Containers
```cmd
docker ps --help
-a: Show all containers (default shows just running)
-q: Only display numeric IDs

# remove container
docker rm {containerId}

# remove all container
docker rm $(docker ps -aq)
```

### Naming Containers
```cmd
# Using name to identify your container.
docker run --name website -d -p 8000:80 nginx:latest

docker stop website
docker start website
```
