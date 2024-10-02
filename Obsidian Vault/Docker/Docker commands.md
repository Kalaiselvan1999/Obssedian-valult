**List all images**
- sudo docker images

**Build image with dockerfile**
- sudo docker build -t {{app-name}} .
	- - `-t fastapi-app` tags the image with the name "fastapi-app" (you can choose a different name).
	- The `.` specifies the build context, which is the current directory.

**Run image as a container**
- sudo docker run {{image-id}}
- sudo docker run {{image-name}}:{{tag-name}}
- sudo docker run -d {{image-id}}
- sudo docker run -d -p8000:8000 --name sample-app {{image-id}}

**Stop a container**
- sudo docker stop {{container-id}}

**Start a docker container**
- sudo docker start {{container-id}}

**List container logs**
- sudo docker logs {{container-id}}

**List running containers**
- sudo docker ps

**List all containers**
- sudo docker ps -a

**Get into dokcer**
- sudo docker exec -it {{container-id}} /bin/bash

**List docker networks**
- sudo docker network ls

**Start a container with compose file**
- sudo docker-compose -f {{yaml-file}} up

**Stop a container**
- sudo docker-compose -f {{yaml-file}} down
