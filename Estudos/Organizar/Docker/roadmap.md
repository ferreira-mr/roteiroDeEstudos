# Docker

## Livros

- [x] [The Docker Book - James Turnbull]()
- [ ] [The Kubernetes Book - Nigel Poulton]()
- [ ] [Docker Deep Dive - Nigel Poulton]()

### Vídeos

- [ ] [Docker Tutorial for Beginners - A Full DevOps Course on How to Run Applications in Containers](https://www.youtube.com/watch?v=fqMOX6JJhGo&t=913s)

## Referências

- [Kode Kloud](https://kodekloud.com/)

### Conceitos chaves

- [ ] Stack memory
- [ ] Cgrups
- [ ] Linux kernel name space
- [ ] Union File System
- [ ] LNX

https://kodekloud.com/p/docker-labs

## Docker / SSH / VS Code

```bash
docker run --name python-exercicios -it  -v $(pwd)/:/home ubuntu
```

## Docker PostgreSQL

```bash
docker run --name some-postgres -e POSTGRES_PASSWORD=postgres -d -p 5432:5432 postgres
```

- [Docker Hub - PostgreSQL](https://hub.docker.com/_/postgres)
- [Dockerize PostgreSQL | Docker Documentation](https://docs.docker.com/engine/examples/postgresql_service/)
- [PostgreSQL + Docker: executando uma instância e o pgAdmin 4 a partir de containers](https://medium.com/@renato.groffe/postgresql-docker-executando-uma-inst%C3%A2ncia-e-o-pgadmin-4-a-partir-de-containers-ad783e85b1a4)
- [Dockerize an SSH service | Docker Documentation](https://docs.docker.com/engine/examples/running_ssh_service/)


## **LIVROS***




*# **DOCKER***

*## **INSTALAÇÃO***

[Passo a passo para instalação](_https://docs.docker.com/install/_)
[Pós instalação no Linux](_https://docs.docker.com/install/linux/linux-postinstall/_)

*## List Docker CLI commands*
docker
docker container —help

*## Display Docker version and info*
docker —version
docker version
docker info

*## Execute Docker image*
docker run hello-world

*## List Docker images*
docker image ls

*## List Docker containers (running, all, all in quiet mode)*
docker container ls
docker container ls —all
docker container ls -aq

```bash
docker build -t friendlyhello .  # Create image using this directory's Dockerfile
docker run -p 4000:80 friendlyhello  # Run "friendlyname" mapping port 4000 to 80
docker run -d -p 4000:80 friendlyhello         # Same thing, but in detached mode
docker container ls                                # List all running containers
docker container ls -a             # List all containers, even those not running
docker container stop <hash>           # Gracefully stop the specified container
docker container kill <hash>         # Force shutdown of the specified container
docker container rm <hash>        # Remove specified container from this machine
docker container rm $(docker container ls -a -q)         # Remove all containers
docker image ls -a                             # List all images on this machine
docker image rm <image id>            # Remove specified image from this machine
docker image rm $(docker image ls -a -q)   # Remove all images from this machine
docker login             # Log in this CLI session using your Docker credentials
docker tag <image> username/repository:tag  # Tag <image> for upload to registry
docker push username/repository:tag            # Upload tagged image to registry
docker run username/repository:tag                   # Run image from a registry
```


*### **DOCKER***

*#### **COMANDOS BÁSICOS***

- docker ps
- docker run -I -t docker_image_name
- docker ps -a (q)
- docker run -it —name [nome_escolhido] [nome_da_imagem]
- docker rm [id_da_docker]

*####**LIVROS***

] Containers com Docker - Daniel Romero, Casa do Código

- [ ] The Kubernetes Book - Nigel Poulton
- [ ] Docker Deep Dive - Nigel Poulton

https://training.play-with-docker.com/#dev
https://docs.docker.com/get-started/

*### **CLOUD***

*#### **AWS***

- [ ] S3
- [ ] CLI
- [ ] EC2
- [ ] Lambda

*##### Cursos*

[AWS Developer: Building on AWS](_https://www.edx.org/course/fundamentals-red-hat-enterprise-linux-red-hat-rh066x_)
[AWS Developer: Deploying on AWS](_https://www.edx.org/course/aws-developer-deploying-on-aws_)
[AWS Developer: Optimizing on AWS](_https://www.edx.org/course/aws-developer-optimizing-on-aws_)

*#### **Google CLoud***

*#### **Azure***
