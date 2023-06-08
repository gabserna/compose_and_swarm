# myDockerImage build commands
To build this image, open a terminal in the directory to build the Dockerfile and run:

1. Build the Docker image: `docker build -t mydockerimage:latest .`
2. Run the image: `docker run -d --name mydockerimage -p 3535:3535 mydockerimage:latest`
3. Test: Browse to http://localhost:3535 in your browser.


0. docker-compose up -d
0. docker-compose up -d --scale firstwebsite=7
0. docker-compose up -d --scale secondwebsite=2
0. docker-compose down
0. docker system info
0. docker swarm init

0. Deploy the stack `docker stack deploy -c docker-compose.yaml  mydockerimage`
0. List the stacks that are running `docker stack ls`
0. List the history / state of the stack: `docker stack ps mydockerimage`
0. List the services that are running in the stack `docker stack services mydockerimage`
0. Remove the stack (by name) `docker stack rm myapp-stack` (All containers will be stopped and removed)