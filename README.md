# Deploy EMQX with docker swarm mode
### Prerequirements
You already have a docker swarm cluster

### Create a Docker Swarm Overlay Network 
```
$ docker network create --driver overlay emqx_network
```

### Deploy the Services
```
$ git clone https://github.com/duclinhfetel/emqx-swarm-mode.git
$ cd emqx-swarm-mode
$ docker stack deploy -c docker-compose.yml emqx
```
