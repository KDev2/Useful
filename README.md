# Useful
## Useful commands to work with Docker containers

#### Creating a new docker image based on the configuration in a specific file name ( apidocker.txt in this example. )
docker build  -t apimlsql -f apidocker.txt .

#### Starting a docker container from an image (counchdb1 in this example)
docker run -d -p 5984:5984 -t couchdb1

#### List the currenlty running containers
Docker Container ls -a

#### Restart a  previously created container which was stopped manually or  because you had to restart the  computer for some reason
Docker start containername

#### Access the shell prompt in a running container
Docker exex -it containername bash

#### removing a docker image 
docker image rm  dockermx

#### building a new docker image
docker build  -t dockermx -f Dockerfile.txt .

Docker container ls -a

#### Creating a docker container based on the image
docker run -t -d dockermx

#### updating a file in a container
Docker cp filename   containername:folder/filename 

#### Run  program in a container - start bash and run the program from the shell prompt
#### Run bash in dockermx container
docker exec  -it quizzical_euclid bash
#Python mxnetmodel.py


