Docker Compose & Swarm
Objective: The objective of this lab is to make sure that every student is able to create a Docker compose file that contains multiple services, deploys the stack, and removes the stack.

You will need to use the image that you created in Lab 2.  Please ensure that you have successfully completed Lab 2 before proceeding.

docker-compose.yaml
Using the image from Lab 2 build a docker-compose.yaml file that contains the following attributes.
Uses version 3.8 of the compose schema

* Deploys 2 services

* First Service:	
- Use image from Lab 2
- Map port 3000 to the proper container port
- Deploys 3 instances (replicas) of the service

* Second Service: 
- User image from Lab 2
- Map port 3001 to the proper container port
- Deploys 2 instances (replicas) of the service

* Ensure that you can perform the following on your local machine.
- Deploy the stack using your docker-compose.yaml file
- Scale out and scale in your services using the docker CLI
- Stop one of your containers and ensure that it starts up again
- Remove your stack

* Create a readme.md that shows the exact Docker command line (with options) for the following:
- Deploy your stack
- Scale out your first stack to 7 instances/replicas
- Scale in your first stack to 2 instances/replicas
- Remove your stack and delete your containers



docker ps -a   #shows all images
docker stop <app name>  #stop image
docker rm <app name>    #remove and release image