# eqmx-swarm-mode
### Prerequirements
You already have a docker swarm cluster

### Create a Docker Swarm Overlay Network 
```
$ docker network create --driver overlay emqx_network
```

### Deploy the Services
```
$ cd eqmx-swarm-mode
$ docker stack deploy -c docker-compose.yml emqx
```
