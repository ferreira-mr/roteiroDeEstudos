# The Docker Book - James Turnbull

<a href='(v18.09)%20James%20Turnbull%20-%20The%20Docker%20Book%20(2018).pdf'>(v18.09) James Turnbull - The Docker Book (2018).pdf</a>

[[DevSecOps]]

[Página do Livro](https://dockerbook.com)

## Commands

[Use the Docker command line | Docker Documentation](https://docs.docker.com/engine/reference/commandline/cli/)
[| Docker Documentation](https://docs.docker.com/engine/reference/run/)

```bash
	docker info
	docker run -i -t python
```

## Chapter 01 - Introduction

## Chapter 02 - Installing Docker

In this chapter, we’ve seen how install Docker on a variety of platforms. We’ve also seen how to manage the Docker daemon.
In the next chapter, we’re going star using Docker. We’ll begin with container basics to give you an introduction to backs Docker operation. If you’re all set up and ready to go then jump into Chapter 3.

## Chapter 03 - Getting Started with Docker

### Displayed Commands

```bash
docker start
docker ps
docker attach docker_name
docker run --name daemon_docker -d debian /bin/sh -c "while true; do echo hello world; skeep 1 done" 
docker logs daemon_docker
docker rm daemon_docker
docker logs -f daemon_docker
docker top daemon_docker
docker stats daemon_docker
docker exec -t -i daemon_docker /bin/bash
docker sotop daemon_docker
docker kill daemon_docker
docker run --restart=always --name daemon_alice -d ubuntu
docker run --restart=on-falure:5
docker inspect daemon_alice
docker inspect daemon_alince --format='{{ .State.Running }}'
docker rm daemon_alice
docker rm -f daemon_alice
docker rm -f 'docker ps -a -q
```

### Summary
We’ve now been introduced to the basic mechanics of how Docker containers work. This information will from the basis for hoe we’ll lean to use Docker in the rest of the book.
In the next chapter, we’re going to explore building or on Docker images and working with docker repositories and registries.

## Chapter 04 - Working with Docker images and repositories
	- What is a Docker image?
	- Listing Docker images
	- Pulling images
	- Searching for images
	- Building our own images
		- Using Docker comment to create images
		- Building images with a Dockerfile
	- What happens if an instruction fails?
	- Docker and the build cache
	- Using the build cache for templating
	- View our new image
	- Laughing a container from our new image
	- Dockerfile instrucitons
		- CMD
		- ENTRYPOINT
		- WORKDIR
		- ENV
		- VOLUME
		- ADD
		- COPY
		- LABEL
		- STOPSIGNAL
		- ARG
		- SHELL
		- ONBUILD

### Keywords
	- bootfs
		- kernel
		- cgroups
		- namespace
		- device manager
	- initrd
	- rootfs
	- union mount
	- image

### Commands
```bash
docker run -i -t --name another_container ubuntu /bin/bash
docker images
docker pull python:3
docker run -i -t --name docker_python python:3
docker search flask
docker build -t="repository_name/image_name:versao_da_imagem .
docker build -t="repository_name/image_name:versao_da_imagem github.com/usuario/repositorio
docker history python
docker run -d -p 5500 --name fask pyhon
docker ps -l
docker port flask
docker run -d -P --name flask python
docker run -d -p 5500:5500 --name flask_name debian 
docker history image_name
docker port container_name
docker inspect
docker build --build-arg build=123 -t ubuntu
sudo docker rmi repository_name/image_name
```

### Dockerfile
```dockerfile
FROM debian
LABEL maintaine="Marcos Ferreira"
LABEL version="1.0"
ENV REFRESED_AT 2019-10-05
ENV RVM_PATH /home/rvm/
WORKDIR /opt/webapp/db
RUN apt-get installl
CMD ["/bin/bash", "-l"]
ENTRYPOINT ["/usr/sbin/nginx", "-g", "daemon off;"]
VOLUME ["/opt/project"]
ADD software.lic /opt/appication/software.lic
COPY conf.d /etc/apache2/
ARG webapp_user=user
HEALTHCHECK --interval=10s --timeout=1m --restries=5 CMD curl://localhost || exit 1
ONBUILD ADD . /app/src
```

### Summary
In this chapter, we’ve seen how to use and interact with Docker images and basics of modifying, update, and uploading images to the Docker Hub. We’ve also learned about using a **Dockerfile** to construct our own custom images. Finnaly, we’ve discovered how to rum or own local Docker registry and some hosted alternative. This give us the bases for starting to build services which Docker.
We’ll use this knowledge in the next chapter to see how we can integrate Docker into a testing workflow and into a Continuous  Integration lifecycle

## Chapter 05 - Testing with Docker
	- Docker internal networking

```bash
docker run -d -p 80 --name website -v $PWD/website:/var/www/html/website nginx
docker run -d -p 80 --name website -v $PWD/website:/var/www/html/website:ro nginx
docker logs -f name_of_container
docker port name_of_container port_to_view
docker network create name_of_network
docker network inspect name_of_network
docker run -d --net=name_of_network --name name_of_container ubuntu
docker network disconnect name_of_container
```

### Summary
In this chapter, we’re seen how to use Docker as a core part of our development and testing workflow. We’ve like at developer-centric testing with Docker on a local workstation or virtual machine. We’ve also explored scaling that testing up to a continuous integration model using Jenkins CI as our tool. We’ve seen how to use Docker of both point testing and how to build distributed matrix jobs.
In the next chapter, we’ll start to see how we can use Docker in product to provide containerised, stackable, scalable, and resilient services.

## Chapter 06 - Building services with Docker
```bash
docker -run -d -h hostname_of_container --net name_of_netowork --name name_of_container debian
docker run -ti --rm --volumes-from path_to_volume_to_add ubuntu
```

### Summary 
In this chapter, we’ve seen how to build some example production service using Docker containers. We’ve seen a bit more about ow we build multi-container services and manage those stacks. We’ve combined features like Docker networking and volume and learned hoe to potentially extend those features to provide us with capabilities like losing and backups.
In the next chapter, we’ll look at orchestration with Docker using the Docker Compose, Docker Swarm and Consul tools.

## Chapter 07 - Docker Orchestration and Service Discovery
### Summary
In the chapter we’ve introduced you to orchestration with Compose. We’ve shown you how to add a Compose configuration file to create simple application stacks. We’ve shown you how to run Compose and build the stacks and how to perform vac management tasks on them.
We’ve also shown you a service discovery tool, Consul. We’ve installed Consul onto Docker and created a cluster of Consul nodes. We’ve also demonstrated how a simple distributed application might work on Docker.
We also took a look at Docker Swarm as a Docker clustering and scheduling tool. We say how to install Swarm, how to manage it and how to schedule workloads across it.
Finally, we’ve seen some of the other orchestration tools available to us in the Docker ecosystem.
In the next chapter we’ll look at the docker API, hoe we can use it, and hoe we  can secure connections to our Docker via TLS.

## Chapter 08 - Using the Docker API
#### Summary
In this chapter, we’ve  been introduced to the Docker Engine API. We’ve also seen how to secure the Docker Engine API via SSL/TSL certificates. We’ve explored the Docker API and dhow to use it to manage images and container. We’ve also seen how to use one of the Docker API client libraries to rewrite our Tprov application to directly use the Docker API.
In the next and last chapter, we’ll look at how you can contribute to Docker.

### Chapter 09 - Getting help and extending Docker
In this chapter, we’ve learned about how to get help with Docker and paces where useful Docker community menses and developers hang out. We’ve also learned about the best way to log an issue with Docker, including the sort of information you need to provide to get the best repose. 
We’ve also seen hoe to set up a development environment to work on the Docketing source or documentation and shoe to build and test inside this environment to ensure your fix or future works. Finally, we’ve learned about how to create a properly strutted and good-quality pull requests with you update.