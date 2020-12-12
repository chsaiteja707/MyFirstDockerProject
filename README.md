# MyFirstDockerProject

1. ensure that the docker installed in the system.
2. create a docker network to make the containers communicate with each other using the command "sudo docker network create network1"
3. build the docker image with any tag in my case it is mong-app "docker build -t mong-app ."
4. run the docker image as a container with a specified name "docker run --name net-app -d  -p 3000:3000 --network network1 mong-app:latest"
5. using above command a docker container will be running in a detached mode with name net-app in external port 3000 using node image.
6. run the mongodb container using "sudo docker run -d --name mongodb --network network1 mongo"
7. using above command a docker container will be running in a detached mode with name mongodb using mongo image.
