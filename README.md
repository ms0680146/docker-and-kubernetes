# docker-and-kubernetes
## Preface
Recently, I watched freeCodeCamp.org youtube channel.The docker and kubernetes topic appeals to me.  
In that topic, I learned:
- creating docker images, running docker containers, docker volumes, container registry and docker architecture.   
- Kubernetes architecture, Kubernetes pods, services, config maps all the way to Kubernetes deployments.  

[Youtube Link](https://www.youtube.com/watch?v=Wf2eSG3owoA&ab_channel=freeCodeCamp.org)


## Introduction to Docker
### What is Docker
Docker is a tool for running applications in isolated environment.

### Docker Container vs VM
Container Benefits: 
1. Run container in seconds.
2. Less disk space.
3. Use less memory
4. Do not need full OS.
5. Deployment

![](https://i.imgur.com/CrrJzy8.png)

###  Installing Docker
Install Docker on macOS: https://docs.docker.com/docker-for-mac/install/  

###  Verify Installation  
```cmd
docker --version
```

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


