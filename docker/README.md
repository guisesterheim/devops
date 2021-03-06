# Docker
Always look for images ready to use. Amazon and Google have many

## Useful Docker commands
* Use Ansible just when creating and provisioning the machine. After that, remove Ansible

<code>DOCKER RUN redis (will launch a docker with redis image)</code>

<code>Access the Redis of initiated redis: redis-cli -h <ip found with "docker ps"></code>

<code>DOCKER PS - lists all running containers</code>

<code>DOCKER INSPECT <id> - brings information about the container (grab CONTAINER_ID through "docker ps"</code>

<code>DOCKER RUN -rm --name redis redis </code>

<code>* rm parameter - kills the container image when it's cancelled</code>

<code>DOCKER STOP <id> - stops container execution</code>

<code>DOCKER START <id> - starts a container execution</code>

<code>DOCKER EXEC -it <id> BASH - SSH to the container</code>

<code>DOCKER RM <name> - << removes stopped container</code>

<code>DOCKER RUN --network=host --name jenkins -p 8282:8080 p- 50000:50000 -v /home/sesteheim/devops jenkins</code>

<code>* Parameter --network=host << Good for the network when having to use a VPN as example</code>

<code>* Parameter -p << maps container ports to the PC ports</code>

<code>* Parameter -v << maps container volumes to the PC volumes</code>

<code>DOCKER BUILD -t <image name: usually <company>/<image name> <path></code>

<code>* Used examlple: DOCKER BUILD -t guilherme/java8 . (do not forget the last dot)</code>

<code>DOCKER STATS << shows the hardware consumption of each container</code>

### Docker Compose:
<code>DOCKER COMPOSE UP -d</code>
