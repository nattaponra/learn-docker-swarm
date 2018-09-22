learn-docker-swarm
#### Create VMs, using the VirtualBox driver:
```
docker-machine create --driver virtualbox myvm1
docker-machine create --driver virtualbox myvm2
```

#### List VMs

```
docker-machine ls
```

#### Initial docker swarm and add node 
``` 
docker-machine ssh myvm1 "docker swarm init --advertise-addr <myvm1 ip>"
```

