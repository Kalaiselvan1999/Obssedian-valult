1. What is Docker?
	► What is a container and what problems does it solve?
	► Container repository - where do containers live?
2. What is a Container technically
	► What is a container technically? (layers of images)
	► Demo part (docker hub and run a docker container locally)
3. Docker vs Virtual Machine
4. Docker Installation
	► Before Installing Docker - prerequisites
	► Install docker on Mac, Windows, Linux
5. Main Docker Commands
	► docker pull, docker run, docker ps, docker stop, docker start, port mapping
6. Debugging a Container
	► docker logs, docker exec -it

### what is docker
	what is container
		way of package application with its dependencies
	where is container stored
		stored in container repository
		private repositories - organizations store it in private repos
		public container - publicly available container in docker hub
	dockerhub 
		more than 100,000 docker images
		search contaniers
	how containers improved application development
		before containers
			devs install each packages like postgres, redis...
			there are more chances on error happening
		after containers
			own isolated environment
			packaged with all configs
			one command to install app
	Application deployment
		configuration written by dev team
		operation will configure these in server
		information can be misguided between dev team and operation team
		pull the docker container and run it
	what is container technically
		layers of image
		base image
			alpine
				is started with linux base image and it is basically alphine
				beacuae alphine is lightweight
		application image
			postgres
	docker run postgres:9.1
	docker image vs docker container
		### docker image
			containes the configuration file, images layers (postgres...) and 
			start script
		### docker container
			actually starts the application
			container environment is created
			**running**
		container stared with docker run *command*
	**Docker vs Virtual machine**
		OS have 2 layers
			Kernel layer communicates with hardware
			application layer run on kernel layer
		*docker*
			virtualize the application layer
			uses the kernel of the host
		*VM*
			virtualize the application layer
			have its own kernel
			virtulize the whole os
		**size**
			docker is small
		**speed**
			docker is fast
		**compantibility**
			vm of any os can run on any OS host
			but linux based docker image can not run on windows
			overcome by docker toolbox
### Docker installation
	docker docs
		docker comminuty version
		docker toolbox
### **Docker commands**

**container**
	file system
	environment configs
	applications image - postgres, redis, mongo
	port binded - each container may port which is used to communicate with application
**images**
	in docker we can see a list of docker images
	***docker images***
		list the images in the system
	***docker run redis***
		run the image in a container
	***docker ps***
		list running containers
	***dokcer run -d redis***
		run the image in detached mode
	***docker stop 34683745***
		stops the container
	***docker start***
		starts the stopped contained
	***docker ps -a***
		list the history of docker containers
	***docker run***
		two commands in one docker pull and docker run
	**container port vs host port**
		docker runs on same port, but host runs on single port
		host must direct the port to container port
	![[Pasted image 20240902225412.png]]
		we can bind the ports by run command
		***docker run -p6000:6379 redis***
			port binding
			run the redis to 6000
	*docker log {{ID}}*
		to see the logs
	*docker run -d -p8080:8000 --name fast-api {{image}}*
		to run container in a name
	
	*sudo docker exec -it {{container-id}} /bin/bash*
		docker executable mode
	docker run vs docker start
	docker run
		create a new container from an image
		takes paras such as -p -d --name
	docker start
		work with containers rather than images
		docker start {{ID}}

### DEMO PROJECT

workflow with docker
![[Pasted image 20240903223030.png]]
