this is continous of [[Docker]]
7. Demo Project Overview - Docker in Practice (Nodejs App with MongoDB and MongoExpress UI)
8. Developing with Containers
	1. ► JavaScript App (HTML, JavaScript Frontend, Node.js Backend)
	2. ► MongoDB and Mongo Express Set-Up with Docker
	3. ► Docker Network concept and demo
	
	
	make an node js app with mongo db and basic frontend with to show  user details
*Nodejs App with MongoDB and MongoExpress UI*

1. pull mongo image from docker hub
2. pull express image from docker hub
3. run mongo and express image in a container

### Docker Network

	docker creates own network to communicate with each other. 
	first run mongo and express in a single docker container which communicates with node out of docker network
	
	![[Pasted image 20240904215908.png]]
convert this to single image
	![[Pasted image 20240904220107.png]]
when running this image in container again, an other client communicate with using port
	![[Pasted image 20240904220236.png]]
 ***docker network ls

	this will list the network
	
***docker network create mongo-network***

	this will create mongo network
**run mongo and express in same network**

	1. run mongo with environment variable with contanier name detached network  with port
		[simple-js-app]$ #docker run -p 27017:27017 -d -e MONGO_INITDB_ROOT_USERNAME=admin -e MONGO_INITDB_ROOT_PASSWORD=password --name
mongo
[simple-js-app]$ docker run -d \
> -p 27017:27017 \
> -e MONGO_INITDB_ROOT_USERNAME=admin \
> -e MONGO
_INITDB_ROOT_PASSWORD=password \
> --name mongodb \
> --net mongo-network \
> mongo
ca2513b10a66620870eecac9c317485/efe032877f544deecec04a602985b
simple-is-app]S docker logs

	2. docker log to see port and network
	3. run docker express which will connect to mongodb on startup. for that there is set of configuration variable. so run docker image of express with that variable to connect with mongo db that previously run in same network
	4. [simple-js-app]$
***docker run -d***
> ***-p 8081:8081 \***
> ***-e ME_CONFIG_MONGODB_ADMINUSERNAME=admin \***
> ***-e ME_CONFIG_MONGODB_ADMINPASSWORD=passwor***
***(> --net mongo-network \***
***(> --name mongo-express \***
> ***-e ME_CONFIG_MONGODB_SERVER=mongodb \***
> ***mongo-express***

	5. connect node js with mongo db with host and port
	require monogdb client.
	connection string protocol
	create user-account database in mongodb
	 6. docker logs {{id }} | tail = latest logs
	 7. docker logs {{container id }} -f = to stream the logs
	 8. full fledged node app with mongo db

### Docker compose

1. to automate the start of container manuually, we compose the mongo-docker-compse.yaml
2. compose the file with
	1. version
	2. services
		1. image
		2. ports
		3. environment variable
		service for mongo db
			services:
				mongodb:
					image: mongo
					ports:
					- 27017:27017
					environment:
					- MONGO...USERNAME=admin
				mongo-express:
					image: mongo-express
					ports:
					- 8080:8080
					environment:
					- ME_CONFIG_MONGODB_A....
**docker compose takes care creating a common network**
3. mongo.yaml

	version: '3' 
		services:
			mongodb: 
				image: mongo
				ports:
					- 27017:27017
				environment:
					- MONGO_INITDB_ROOT_USERNAME=admin
					- MONGO_INITDB_ROOT_PASSWORD=password
			mongo-express:
				image: mongo-express
				ports:
					- 8080:8081
				environment:
					- ME_CONFIG_MONGODB_ADMINUSERNAME=admin
					- ME_CONFIG_MONGODB_ADMINPASSWORD=password
					- ME_CONFIG_MONGODB_SERVER=mongodb
4. how to start a contaner with compose file
5. if docker-compose is installed 
	1. this is the command to compose the container with yaml file
		docker-compose -f mongo.yaml	up
		**up** will start the container
![[Pasted image 20240904231319.png]]

create the network when compose 
 see it by docker network ls
when one is depends on other need to handle it logically
	for ex. mongo express is depend upon mongo db, so mongo db service should written before mongo express

	docker ps - will list the both container of mongo db and mongo express
	check it by localhost:8080
***docker volumes for data persistence***

for stop docker container
 docker-compose -f mongo.yaml down
	 will stop container and will stop network