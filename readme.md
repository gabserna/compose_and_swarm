# myDockerImage build commands
To build this image, open a terminal in the directory to build the Dockerfile and run:

1. Build the Docker image: `docker build -t mydockerimage:latest .`
2. Run the image: `docker run -d --name mydockerimage -p 3535:3535 mydockerimage:latest`
3. Test: Browse to http://localhost:3535 in your browser.
# myDockerImage run commands
- docker-compose up -d
- docker-compose up -d --scale firstwebsite=7
- docker-compose up -d --scale secondwebsite=2
- docker-compose down
- docker system info
- docker swarm init

- Deploy the stack `docker stack deploy -c docker-compose.yaml  mydockerimage`
- List the stacks that are running `docker stack ls`
- List the history / state of the stack: `docker stack ps mydockerimage`
- List the services that are running in the stack `docker stack services mydockerimage`
- Remove the stack (by name) `docker stack rm mydockerimage` (All containers will be stopped and removed)